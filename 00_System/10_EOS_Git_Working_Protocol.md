# EOS Git Working Protocol

| Campo                    | Valor                                                          |
| ------------------------ | -------------------------------------------------------------- |
| **Estado del documento** | Operational Baseline                                           |
| **Versión**              | Git Working Protocol 1.0                                       |
| **Propósito**            | Definir el uso práctico de Git para proteger y evolucionar EOS |
| **Establecido**          | Septiembre de 2026                                             |
| **Naturaleza**           | Documento operativo                                            |
| **Idioma**               | Español — edición original                                     |

---

# 1. Propósito

Git es el mecanismo de control de versiones utilizado por EOS para preservar, revisar y recuperar la evolución del sistema.

Su función no es introducir burocracia.

Su función es:

* preservar estados válidos;
* registrar cambios significativos;
* permitir recuperar estados anteriores;
* aislar cambios cuando sea necesario;
* y mantener una historia técnica comprensible.

> **Git debe proteger EOS, no convertirse en una carga para evolucionarlo.**

---

# 2. Principio de `main`

La rama `main` representa un estado:

* válido;
* coherente;
* recuperable;
* y razonablemente utilizable de EOS.

`main` no necesita representar un sistema terminado o perfecto.

Debe representar un estado en el que sea razonable continuar trabajando.

---

# 3. Principio de proporcionalidad

La complejidad del procedimiento Git debe ser proporcional al impacto del cambio.

EOS utiliza tres niveles operativos.

### Level A — Cambio trivial

Para cambios como:

* correcciones ortográficas;
* ajustes menores de formato;
* pequeñas correcciones documentales;
* cambios sin impacto estructural.

Flujo:

```text
Editar
  ↓
git diff
  ↓
git add
  ↓
git diff --cached
  ↓
commit
  ↓
push
```

---

### Level B — Cambio significativo

Para cambios que requieren aislamiento y revisión antes de incorporarse a `main`.

Flujo:

```text
main
  ↓
crear branch
  ↓
trabajar
  ↓
git diff
  ↓
staging
  ↓
git diff --cached
  ↓
commit
  ↓
volver a main
  ↓
merge
  ↓
push
  ↓
eliminar branch
  ↓
verificar
```

---

### Level C — Cambio estructural o experimental

Para cambios que pueden modificar la estructura, organización o comportamiento del EOS.

Flujo:

```text
main
  ↓
crear branch
  ↓
desarrollar / experimentar
  ↓
validar
  ↓
commit
  ↓
merge
  ↓
push
  ↓
tag si corresponde
  ↓
eliminar branch
  ↓
verificar
```

El Level C puede utilizar un tag cuando el resultado represente un estado histórico relevante de EOS.

---

# 4. Principio de inspección

Ningún cambio debe convertirse en commit sin haber sido inspeccionado.

Antes de registrar un cambio:

```bash
git status
git diff
```

Después de preparar el cambio:

```bash
git status
git diff --cached
```

La revisión debe responder:

> **¿Estoy registrando exactamente lo que creo estar registrando?**

---

# 5. Principio de commit

Un commit debe representar:

> **una intención lógica identificable.**

El mensaje debe permitir comprender posteriormente qué se modificó y con qué propósito.

Debe evitarse agrupar cambios independientes únicamente para reducir el número de commits.

---

# 6. Principio de aislamiento

Cuando un cambio pueda poner en duda la validez de `main`, debe utilizarse una rama.

Regla práctica:

> **Si el cambio puede ser experimental, estructural o suficientemente significativo como para requerir revisión, aislarlo.**

Las ramas son herramientas temporales de aislamiento.

No constituyen estructura permanente del EOS.

---

# 7. Principio de integración

Una vez validado un cambio desarrollado en una rama, debe integrarse nuevamente en `main`.

Cuando no existen cambios divergentes, un `fast-forward` es una forma válida y simple de integración.

El objetivo es que la historia permanezca comprensible sin introducir complejidad innecesaria.

---

# 8. Principio de publicación

Después de integrar un cambio válido en `main`, debe publicarse en el repositorio remoto:

```bash
git push
```

El estado operativo normal de EOS debe ser:

```text
main = origin/main
working tree = clean
```

Esto proporciona una referencia remota actualizada y recuperable.

---

# 9. Principio de limpieza

Una rama temporal debe eliminarse una vez que su trabajo haya sido correctamente integrado y publicado.

El ciclo normal es:

```text
crear
  ↓
trabajar
  ↓
integrar
  ↓
publicar
  ↓
eliminar
```

La existencia de ramas no utilizadas no aporta valor por sí misma.

---

# 10. Principio de tags

Los tags no deben utilizarse para cada commit.

Deben reservarse para estados que merezcan una referencia histórica clara, por ejemplo:

* un baseline;
* una versión estable;
* una reorganización estructural;
* una etapa importante de evolución;
* o un estado que deba poder recuperarse inequívocamente.

> **Un tag identifica un estado; no simplemente un momento.**

---

# 11. Regla de decisión

La decisión fundamental para determinar el nivel de trabajo es:

> **Si el cambio puede poner en duda la validez de `main`, utilizar una rama.**

De lo contrario, un cambio directo sobre `main` puede ser suficiente.

Esta regla permite mantener el procedimiento proporcional al riesgo.

---

# 12. Estado esperado

Al finalizar un ciclo normal de trabajo, EOS debe procurar volver a:

```text
main
  ↓
working tree clean
  ↓
origin/main synchronized
```

No debe quedar trabajo parcialmente integrado sin una razón explícita.

---

# 13. Regla de simplicidad

Git debe utilizarse con la mínima complejidad necesaria para proteger el conocimiento y la evolución de EOS.

No se crearán:

* ramas;
* commits;
* tags;
* revisiones;
* ni procedimientos

simplemente porque Git los permita.

> **No Git por Git.**

---

# 14. Regla de recuperación

La historia Git debe permitir recuperar estados anteriores de EOS cuando sea necesario.

Un estado importante debe poder:

* identificarse;
* recuperarse;
* inspeccionarse;
* y comprenderse.

La recuperación forma parte de la preservación del conocimiento.

---

# 15. Regla fundamental

El propósito final del protocolo es mantener una evolución controlada sin impedir la evolución.

```text
Preservar
    ↓
Inspeccionar
    ↓
Registrar
    ↓
Integrar
    ↓
Publicar
    ↓
Recuperar cuando sea necesario
```

> **EOS debe poder evolucionar sin perder la historia que explica cómo llegó a ser lo que es.**
