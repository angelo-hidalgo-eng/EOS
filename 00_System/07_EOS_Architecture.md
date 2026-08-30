### Arquitectura del Engineering Operating System

| Campo                     | Valor                                                      |
| ------------------------- | ---------------------------------------------------------- |
| **Estado del documento**  | Baseline                                                   |
| **Estado arquitectónico** | Architectural Baseline 1.0 — Operacional                   |
| **Propósito**             | Describir la arquitectura conceptual y estructural del EOS |
| **Establecido**           | Agosto de 2026                                             |
| **Origen del EOS**        | 21 de julio de 2026                                        |
| **Naturaleza**            | Documento arquitectónico                                   |
| **Idioma**                | Español — edición original                                 |
| **Autor**                 | Ing. Luis Angelo Hidalgo Arancibia                         |


---

# 1. Propósito

Este documento describe la arquitectura del **Engineering Operating System (EOS)**.

Su objetivo es responder:

> **¿Cómo está estructurado EOS para cumplir su Foundation, avanzar hacia su Vision, ejecutar su Mission y respetar su Constitution?**

No pretende explicar nuevamente por qué EOS existe ni narrar su evolución histórica.

Es la descripción de la **estructura conceptual resultante**.

---

# 2. Definición arquitectónica

El **Engineering Operating System** es una arquitectura de conocimiento orientada a preservar, contextualizar, relacionar y reutilizar conocimiento de ingeniería a través del tiempo.

Su arquitectura se fundamenta en un conjunto pequeño de entidades conceptuales y en las relaciones que existen entre ellas.

La arquitectura no intenta representar cada posible tipo de información mediante una categoría específica.

Su objetivo es proporcionar:

> **un modelo conceptual estable capaz de representar múltiples dominios de ingeniería sin perder significado.**

---

# 3. Principio arquitectónico central

La arquitectura puede resumirse en una regla:

> ## **Pocas entidades. Relaciones significativas. Contexto suficiente.**

Esto significa que la complejidad del sistema no debe crecer principalmente mediante la creación de nuevas categorías.

Debe crecer mediante la capacidad de expresar correctamente las relaciones entre los elementos existentes.

---

# 4. Arquitectura conceptual

En su nivel más abstracto, EOS puede representarse como:

```
                    ┌────────────────────┐
                    │      CONTEXTO      │
                    └─────────┬──────────┘
                              │
                              ▼
┌──────────────┐      ┌─────────────────┐      ┌──────────────┐
│   PROYECTOS  │─────▶│   CONOCIMIENTO  │◀────│   EVIDENCIA  │
└──────┬───────┘      └────────┬────────┘      └──────────────┘
       │                       │
       │                       ▼
       │                ┌──────────────┐
       └───────────────▶│  DECISIONES  │
                        └──────┬───────┘
                               │
                               ▼
                        ┌──────────────┐
                        │  ARTEFACTOS  │
                        └──────────────┘
```

El diagrama no debe interpretarse como una secuencia obligatoria.

Representa un **sistema de relaciones**.

---

# 5. Las entidades fundamentales

La arquitectura utiliza un conjunto pequeño de entidades conceptuales.

En la Baseline actual se reconocen como núcleo:

1. **Proyecto**
2. **Conocimiento**
3. **Evidencia**
4. **Decisión**
5. **Artefacto**
6. **Contexto**

Estas entidades no representan todas las cosas que pueden existir en un proyecto.

Representan **puntos de anclaje conceptuales** suficientemente generales para organizar información heterogénea.

---

# 6. Proyecto

Un **Proyecto** representa una iniciativa, problema, trabajo o línea de actividad dentro de la cual ocurre experiencia de ingeniería.

Un proyecto proporciona:

- propósito;
- alcance;
- contexto;
- actividad;
- resultados;
- y una trayectoria temporal.

El proyecto constituye uno de los principales lugares donde se genera conocimiento.

Sin embargo:

> **El conocimiento producido por un proyecto no pertenece exclusivamente al proyecto.**

Puede trascenderlo y ser reutilizado en otros contextos.

---

# 7. Conocimiento

**Conocimiento** representa una comprensión que ha adquirido suficiente significado, contexto o utilidad como para ser preservada.

Puede surgir de:

- experiencia;
- evidencia;
- experimentación;
- análisis;
- decisiones;
- resultados;
- documentación;
- o combinación de éstos.

El conocimiento no debe confundirse con un documento.

Un documento puede contener conocimiento.

Pero el conocimiento puede estar relacionado con múltiples documentos, evidencias y experiencias.

---

# 8. Evidencia

**Evidencia** representa aquello que permite sustentar, cuestionar, validar o comprender una afirmación o conclusión.

Puede adoptar diversas formas:

- medición;
- experimento;
- registro;
- observación;
- prueba;
- resultado;
- documentación técnica;
- código;
- fotografía;
- captura;
- u otro artefacto verificable.

La arquitectura no presupone que toda evidencia sea definitiva.

Una evidencia puede ser posteriormente:

- reinterpretada;
- contradicha;
- complementada;
- o reemplazada.

---

# 9. Decisión

Una **Decisión** representa una elección significativa realizada dentro de un contexto determinado.

Una decisión puede estar relacionada con:

- un problema;
- una restricción;
- alternativas;
- evidencia;
- conocimiento;
- una implementación;
- y un resultado.

Cuando sea relevante, la arquitectura debe permitir conservar su **Decision Lineage**.

Es decir:

> **la relación entre la situación que originó una decisión y las consecuencias que produjo.**

---

# 10. Artefacto

Un **Artefacto** representa una manifestación concreta del trabajo.

Puede ser:

- código;
- circuito;
- esquema;
- diseño;
- documento;
- fotografía;
- modelo;
- configuración;
- medición registrada;
- archivo;
- prototipo;
- o cualquier otro resultado material o digital.

El artefacto no es necesariamente conocimiento.

Puede ser:

> **evidencia del conocimiento, resultado de una decisión, fuente de evidencia o material utilizado para producir conocimiento.**

Su significado depende de sus relaciones.

---

# 11. Contexto

**Contexto** representa las condiciones necesarias para interpretar correctamente otros elementos.

Puede incluir:

- circunstancias;
- restricciones;
- entorno;
- propósito;
- condiciones técnicas;
- estado del proyecto;
- periodo temporal;
- dependencias;
- antecedentes.

El contexto no debe convertirse en una categoría utilizada para almacenar indiscriminadamente información contextual.

Su función es conservar aquello necesario para mantener el significado.

---

# 12. Las relaciones

Las entidades constituyen los nodos.

Las relaciones constituyen gran parte del significado.

Algunas relaciones fundamentales pueden expresarse conceptualmente como:

```
Proyecto
   ├── produce ────────▶ Artefacto
   ├── genera ─────────▶ Evidencia
   ├── contiene ───────▶ Decisiones
   └── produce ────────▶ Conocimiento

Evidencia
   └── sustenta ───────▶ Conocimiento

Conocimiento
   └── informa ────────▶ Decisión

Decisión
   ├── afecta ────────▶ Artefacto
   └── produce ───────▶ Resultado

Contexto
   └── contextualiza ──▶ cualquiera de los anteriores
```

Estas relaciones son conceptuales.

La implementación concreta puede cambiar.

---

# 13. La arquitectura es un grafo de conocimiento

La representación más adecuada del EOS no es exclusivamente jerárquica.

Puede entenderse mejor como un **grafo de conocimiento contextualizado**.

```
                 ┌─────────────┐
                 │  Contexto   │
                 └──────┬──────┘
                        │
                        ▼
┌─────────┐       ┌───────────┐       ┌──────────┐
│ Proyecto│──────▶│ Evidencia │──────▶│Conocimiento│
└────┬────┘       └───────────┘       └────┬─────┘
     │                                      │
     │                                      ▼
     │                               ┌────────────┐
     └──────────────────────────────▶│  Decisión  │
                                     └──────┬─────┘
                                            │
                                            ▼
                                     ┌────────────┐
                                     │  Artefacto │
                                     └────────────┘
```

La representación jerárquica seguirá siendo útil para navegar y organizar archivos.

Pero la **estructura conceptual** es relacional.

---

# 14. El principio de relación

Una entidad aislada puede contener información.

Una entidad relacionada puede contener significado.

Por ello, EOS debe favorecer:

> **relaciones explícitas cuando aporten comprensión.**

No todas las relaciones posibles deben registrarse.

Deben conservarse aquellas que permitan:

- recuperar contexto;
- comprender procedencia;
- explicar decisiones;
- establecer causalidad;
- identificar dependencia;
- reconstruir evolución;
- o facilitar reutilización.

---

# 15. El tiempo como dimensión arquitectónica

EOS no es únicamente espacial.

También es temporal.

Un mismo conocimiento puede evolucionar:

```
Conocimiento A
      │
      │ nueva evidencia
      ▼
Conocimiento B
      │
      │ nueva experiencia
      ▼
Conocimiento C
```

Por ello, la arquitectura debe poder representar:

- estado;
- evolución;
- precedencia;
- vigencia;
- y relaciones históricas.

No significa versionar absolutamente todo.

Significa conservar la historia cuando ésta sea necesaria para comprender el conocimiento.

---

# 16. La dimensión histórica

La arquitectura incorpora una dimensión histórica porque:

> **el conocimiento tiene historia.**

Una decisión actual puede depender de decisiones anteriores.

Una arquitectura actual puede ser resultado de varias iteraciones.

Un conocimiento vigente puede haber reemplazado otro.

La historia proporciona contexto explicativo.

Por tanto, cuando tenga valor, el sistema debe permitir navegar:

```
Antes
  ↓
Cambio
  ↓
Después
```

---

# 17. Proveniencia

EOS debe poder representar, cuando sea relevante, la procedencia de conocimiento.

Conceptualmente:

```
Experiencia
    ↓
Evidencia
    ↓
Interpretación
    ↓
Conocimiento
    ↓
Decisión
    ↓
Resultado
```

La proveniencia permite responder:

> **¿De dónde salió este conocimiento?**

Y también:

> **¿Qué ocurrió después de utilizarlo?**

---

# 18. El ciclo de conocimiento

La arquitectura soporta el ciclo fundamental definido en la Mission:

```
EXPERIENCIA
     ↓
EVIDENCIA
     ↓
CONOCIMIENTO
     ↓
DECISIÓN
     ↓
IMPLEMENTACIÓN
     ↓
RESULTADO
     ↓
NUEVA EXPERIENCIA
```

EOS actúa como memoria entre ciclos.

Por eso puede transformar una sucesión de proyectos independientes en una trayectoria acumulativa.

---

# 19. Separación entre conocimiento y artefactos

Uno de los principios arquitectónicos importantes es no confundir:

> **el objeto que contiene o representa algo**

con:

> **el conocimiento que ese objeto permite preservar.**

Por ejemplo:

Un archivo de código puede ser un artefacto.

El conocimiento de por qué una determinada arquitectura de software fue elegida es otra cosa.

Una fotografía puede ser un artefacto.

La conclusión obtenida a partir de esa fotografía puede ser conocimiento.

Esta separación permite evitar que EOS quede limitado a una arquitectura documental.

---

# 20. Arquitectura independiente del dominio

El modelo debe poder representar proyectos de naturaleza muy diferente.

Por ejemplo:

### Hardware

```
Proyecto
 → medición
 → evidencia
 → decisión
 → circuito
```

### Software

```
Proyecto
 → prueba
 → evidencia
 → decisión
 → código
```

### Carpintería

```
Proyecto
 → medición
 → diseño
 → decisión
 → pieza construida
```

La estructura fundamental permanece.

Lo que cambia es el contenido.

Esta es una de las validaciones principales de la arquitectura.

---

# 21. Arquitectura independiente de la herramienta

La arquitectura conceptual no depende de:

- Obsidian;
- Git;
- GitHub;
- Markdown;
- VS Code;
- Linux;
- bases de datos;
- ni ninguna aplicación concreta.

Estas herramientas forman parte de la **implementación**.

Conceptualmente:

```
EOS Architecture
        ↓
Implementation Model
        ↓
Tools
```

Una modificación en el nivel inferior no debería obligar automáticamente a rediseñar el nivel superior.

---

# 22. Capas de arquitectura

EOS puede entenderse mediante varias capas:

```
┌─────────────────────────────────────┐
│        PRINCIPIOS CONSTITUCIONALES  │
├─────────────────────────────────────┤
│         MODELO CONCEPTUAL           │
├─────────────────────────────────────┤
│             ENTIDADES               │
├─────────────────────────────────────┤
│             RELACIONES              │
├─────────────────────────────────────┤
│        ESTRUCTURA DOCUMENTAL        │
├─────────────────────────────────────┤
│           IMPLEMENTACIÓN            │
├─────────────────────────────────────┤
│              HERRAMIENTAS           │
└─────────────────────────────────────┘
```

Cada capa tiene una responsabilidad distinta.

---

# 23. Principios antes que estructura

La arquitectura debe seguir una dirección descendente:

```
Principio
   ↓
Significado
   ↓
Entidad
   ↓
Relación
   ↓
Estructura
   ↓
Implementación
   ↓
Herramienta
```

Esto evita que las limitaciones de una herramienta determinen prematuramente el modelo conceptual.

---

# 24. La estructura documental

La implementación inicial del EOS utilizará documentos y archivos para representar el conocimiento.

Sin embargo:

> **la estructura documental es una representación de la arquitectura, no la arquitectura misma.**

Esto permite que:

- una nota pueda convertirse en otra forma de representación;
- una herramienta pueda cambiar;
- un repositorio pueda reorganizarse;
- o incluso una tecnología futura pueda reemplazar completamente la implementación actual.

Mientras las relaciones conceptuales puedan conservarse, la arquitectura puede sobrevivir.

---

# 25. El principio de mínima estructura

EOS debe utilizar la menor estructura necesaria para expresar correctamente el conocimiento.

Esto significa:

> **No crear una entidad cuando una relación sea suficiente.**

Y también:

> **No crear una relación cuando no aporte significado.**

La arquitectura debe evitar tanto:

- submodelización;

como:

- sobre-modelización.

---

# 26. Evolución arquitectónica

La arquitectura actual es una **Baseline**, no una declaración de perfección.

Puede evolucionar cuando exista evidencia suficiente.

El ciclo de evolución es:

```
Uso real
   ↓
Problema
   ↓
Análisis
   ↓
Necesidad
   ↓
Propuesta
   ↓
Validación
   ↓
Cambio arquitectónico
```

Los cambios importantes deben conservar su razonamiento mediante los mecanismos históricos correspondientes.

---

# 27. Criterio para nuevas entidades

Una nueva entidad fundamental sólo debería introducirse cuando:

1. existe una necesidad real;
2. la necesidad es recurrente o arquitectónicamente significativa;
3. las entidades existentes no pueden expresarla adecuadamente;
4. una relación no es suficiente;
5. y la nueva entidad aporta capacidad proporcional a la complejidad introducida.

Esto protege el núcleo arquitectónico.

---

# 28. El núcleo debe permanecer pequeño

Una arquitectura destinada a durar décadas necesita un núcleo estable.

Por ello:

> **El número de entidades fundamentales debe crecer mucho más lentamente que el conocimiento que representan.**

Esto permite que el sistema aumente enormemente su contenido sin aumentar proporcionalmente su complejidad estructural.

---

# 29. Arquitectura y reutilización

La reutilización depende de que el conocimiento pueda ser separado de su proyecto de origen sin perder su significado.

Por ello, EOS debe permitir:

```
Proyecto A
    ↓
Conocimiento
    ↓
Contexto relevante
    ↓
Proyecto B
```

Esto transforma el conocimiento local en conocimiento transferible.

---

# 30. Arquitectura y memoria institucional

Aunque EOS pueda utilizarse individualmente, su estructura también permite preservar conocimiento que de otro modo podría perderse cuando cambian las personas.

La arquitectura puede conservar:

- decisiones;
- criterios;
- precedentes;
- errores;
- aprendizajes;
- historia.

Así puede disminuirse la dependencia de la memoria individual.

---

# 31. Arquitectura y continuidad

La arquitectura debe permitir que una persona pueda regresar a un proyecto después de:

- meses;
- años;
- o incluso décadas,

y reconstruir razonablemente:

- qué se estaba haciendo;
- por qué;
- qué se había aprendido;
- qué decisiones se habían tomado;
- y qué quedaba pendiente.

Esta capacidad de **reentrada contextual** es una propiedad importante del sistema.

---

# 32. Arquitectura y recuperación

El valor de conservar conocimiento depende parcialmente de poder recuperarlo.

Pero recuperación no significa simplemente:

> "encontrar un archivo."

Significa poder encontrar:

> **el conocimiento pertinente y suficiente para comprender una situación.**

Por eso, las relaciones y el contexto son tan importantes como la ubicación física del documento.

---

# 33. Arquitectura y simplicidad

La simplicidad arquitectónica no se obtiene eliminando información.

Se obtiene evitando representar de manera independiente aquello que puede expresarse correctamente mediante relaciones.

Por ello:

> **La simplicidad es una consecuencia de una correcta abstracción.**

Y:

> **La profundidad del conocimiento no requiere necesariamente profundidad estructural.**

---

# 34. Propiedad fundamental del modelo

Una propiedad esencial de la arquitectura es:

> **el contenido puede crecer mucho más rápidamente que el modelo.**

Esto es deseable.

Si cada nuevo conocimiento exige:

- una nueva categoría;
- una nueva estructura;
- una nueva herramienta;
- y nuevas reglas,

la arquitectura no escala.

En cambio:

```
Modelo pequeño
      +
Muchas relaciones
      +
Contenido creciente
```

permite una expansión mucho más sostenible.

---

# 35. Arquitectura como sistema abierto

EOS debe poder incorporar nuevas:

- disciplinas;
- tecnologías;
- proyectos;
- tipos de evidencia;
- formas de trabajo;
- herramientas.

La incorporación no debería requerir reconstruir el núcleo.

Esto convierte la **extensibilidad** en una propiedad arquitectónica importante.

---

# 36. Vista resumida de la arquitectura

La arquitectura puede resumirse así:

```
                         EOS
                          │
             ┌────────────┴────────────┐
             │                         │
        MODELO CONCEPTUAL          MEMORIA
             │                         │
       ┌─────┼─────┐             ┌─────┴─────┐
       │     │     │             │           │
   Entidades Relaciones       Historia    Contexto
       │     │     │             │           │
       └─────┼─────┘             └─────┬─────┘
             │                         │
             └──────────┬──────────────┘
                        │
                        ▼
                CONOCIMIENTO
                        │
                        ▼
                 CAPACIDAD FUTURA
```

---

# 37. Definición arquitectónica resumida

> **EOS es una arquitectura de conocimiento basada en un núcleo pequeño de entidades fundamentales y un conjunto de relaciones significativas que permiten representar experiencia, evidencia, conocimiento, decisiones, artefactos y contexto a través del tiempo.**

> **La arquitectura está diseñada para que el conocimiento pueda conservarse independientemente de su proyecto de origen, mantener el contexto necesario para su comprensión, preservar su evolución histórica y regresar posteriormente a la práctica de ingeniería.**

> **Su estructura debe permanecer simple, extensible, independiente de herramientas y capaz de evolucionar mediante evidencia de uso.**

---

# 38. La arquitectura en una frase

> ## **Un modelo pequeño y estable capaz de representar una gran cantidad de conocimiento mediante relaciones significativas a través del tiempo.**

Y quizás la frase que mejor conecta este documento con todo lo anterior:

> ## **Pocas entidades. Relaciones correctas. Contexto suficiente. Evolución controlada.**

---

# 39. Relación con el núcleo documental

Con `07 — EOS Architecture` ya tenemos una separación muy limpia:

|Documento|Función|
|---|---|
|**04 — Constitution**|Define lo que debe protegerse|
|**06 — Architect's Notes**|Explica por qué la arquitectura llegó a ser así|
|**07 — EOS Architecture**|**Describe la arquitectura resultante**|
|**08 — Operating Principles**|Explicará cómo operar dentro de ella|

Esto es importante porque evita mezclar **arquitectura** con **procedimiento**.

---

# 40. Cierre

La arquitectura del EOS puede parecer pequeña.

Y **eso es precisamente una de sus virtudes**.

No intenta construir un modelo diferente para cada tipo de ingeniería.

Busca encontrar las estructuras que permanecen cuando cambia el dominio.

No intenta almacenar todo.

Busca conservar aquello que permite que el conocimiento sobreviva.

No intenta eliminar la complejidad del conocimiento.

Busca evitar que la complejidad del conocimiento se convierta innecesariamente en complejidad de la arquitectura.

Y por encima de todo:

> **la arquitectura no debe crecer al mismo ritmo que el conocimiento.**

Debe permitir que **el conocimiento crezca mucho más rápido que la estructura que lo sostiene**.

Ese es uno de los criterios que determinarán si EOS realmente puede acompañarnos durante décadas.

>  **Pocas entidades. Relaciones significativas. Contexto suficiente.**

> **Construimos conocimiento para construir mejor.**

**EOS — Architecture**  
**Agosto de 2026**  
**Architectural Baseline 1.0 — Operacional**  
**Edición original en español**
