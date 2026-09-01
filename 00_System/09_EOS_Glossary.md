### Glosario y lenguaje común del Engineering Operating System

|Campo|Valor|
|---|---|
|**Estado del documento**|Baseline|
|**Versión**|Glossary Baseline 1.0|
|**Propósito**|Establecer el vocabulario común y las definiciones fundamentales de EOS|
|**Establecido**|Agosto de 2026|
|**Origen del EOS**|21 de julio de 2026|
|**Naturaleza**|Documento de referencia|
|**Idioma**|Español — edición original|
| **Autor**| Ing. Luis Angelo Hidalgo Arancibia|


---

# 1. Propósito

El **EOS Glossary** establece el vocabulario utilizado para describir, construir, operar y evolucionar el _Engineering Operating System_.

Su propósito es evitar que conceptos fundamentales sean interpretados de manera diferente con el paso del tiempo.

En EOS:

> **Una palabra importante debe conservar un significado estable.**

El glosario constituye, por tanto, una parte de la arquitectura conceptual del sistema.

---

# 2. Cómo utilizar este documento

Las definiciones de este glosario deben interpretarse dentro del contexto del EOS.

Cuando una palabra posea un significado específico dentro de EOS, dicho significado prevalece sobre interpretaciones informales.

El glosario no pretende definir todo el lenguaje de la ingeniería.

Define solamente los conceptos necesarios para comprender y operar EOS.

---

# 3. EOS — Engineering Operating System

**Engineering Operating System (EOS)**

Arquitectura de conocimiento destinada a preservar, contextualizar, relacionar, recuperar, reutilizar y evolucionar conocimiento de ingeniería a través del tiempo.

EOS no es simplemente:

- un repositorio;
- un sistema documental;
- una aplicación;
- una colección de notas;
- ni una herramienta.

Es una **arquitectura de conocimiento**.

---

# 4. Arquitectura

**Arquitectura**

Estructura conceptual que define las entidades fundamentales de EOS, sus relaciones y los principios que permiten que el sistema evolucione sin perder coherencia.

La arquitectura es independiente de la implementación concreta.

---

# 5. Modelo conceptual

**Modelo conceptual**

Representación abstracta de los elementos y relaciones fundamentales que EOS utiliza para representar conocimiento.

El modelo conceptual precede a:

- estructura documental;
- herramientas;
- automatizaciones;
- implementación.

---

# 6. Entidad

**Entidad**

Elemento conceptual que posee identidad suficiente para ser representado y relacionado dentro de EOS.

Las entidades fundamentales de la arquitectura actual incluyen:

- Proyecto;
- Conocimiento;
- Evidencia;
- Decisión;
- Artefacto;
- Contexto.

---

# 7. Relación

**Relación**

Vínculo explícito entre dos o más elementos que aporta significado.

Una relación puede expresar, entre otras cosas:

- procedencia;
- dependencia;
- causalidad;
- evolución;
- influencia;
- validación;
- reutilización;
- contradicción.

En EOS:

> **Las relaciones son parte del conocimiento, no solamente elementos de navegación.**

---

# 8. Contexto

**Contexto**

Conjunto de condiciones necesarias para comprender correctamente un conocimiento, decisión, experiencia, proyecto o artefacto.

Puede incluir:

- propósito;
- restricciones;
- circunstancias;
- entorno;
- estado;
- antecedentes;
- condiciones técnicas;
- momento histórico.

---

# 9. Conocimiento

**Conocimiento**

Comprensión derivada de experiencia, evidencia, análisis, razonamiento o combinación de éstos, que posee suficiente significado o utilidad para ser preservada.

El conocimiento no es equivalente a información.

---

# 10. Información

**Información**

Datos o contenidos organizados que poseen significado, pero que no necesariamente han sido interpretados o convertidos en conocimiento reutilizable.

Relación conceptual:

```
Dato
 ↓
Información
 ↓
Interpretación
 ↓
Conocimiento
```

No toda información necesita convertirse en conocimiento.

---

# 11. Dato

**Dato**

Representación de una observación, medición, valor o hecho sin necesariamente incluir su interpretación.

Ejemplo:

> `3,3 Volts`

es un dato.

El significado que posee ese valor dentro de un circuito pertenece al contexto y al conocimiento asociado.

---

# 12. Evidencia

**Evidencia**

Elemento que permite sustentar, cuestionar, validar o comprender una afirmación, hipótesis, decisión o conclusión.

Puede ser:

- experimental;
- documental;
- observacional;
- cuantitativa;
- cualitativa;
- física;
- digital.

---

# 13. Artefacto

**Artefacto**

Resultado concreto, físico o digital, producido, utilizado o modificado durante una actividad de ingeniería.

Ejemplos:

- código;
- circuito;
- esquema;
- documento;
- fotografía;
- configuración;
- prototipo;
- modelo;
- archivo.

Un artefacto puede contener, representar o proporcionar evidencia de conocimiento.

---

# 14. Proyecto

**Proyecto**

Iniciativa delimitada por un propósito, problema, objetivo o conjunto de actividades dentro de la cual se genera experiencia y conocimiento.

Un proyecto posee normalmente:

- contexto;
- trayectoria;
- decisiones;
- artefactos;
- resultados;
- aprendizajes.

---

# 15. Experiencia

**Experiencia**

Conocimiento potencial generado mediante la interacción directa con un problema, sistema, herramienta, proyecto o situación.

La experiencia puede permanecer tácita o convertirse en conocimiento explícito mediante reflexión y documentación.

---

# 16. Conocimiento tácito

**Conocimiento tácito**

Conocimiento que reside principalmente en la experiencia, intuición, habilidades o modelos mentales de una persona y que todavía no ha sido expresado de manera suficientemente explícita.

El EOS busca reducir la pérdida de conocimiento tácito significativo mediante su transformación progresiva en conocimiento preservable.

---

# 17. Conocimiento explícito

**Conocimiento explícito**

Conocimiento expresado de una forma que puede ser almacenada, comunicada, recuperada y reutilizada.

Ejemplos:

- una explicación;
- un principio;
- una decisión documentada;
- un procedimiento;
- un modelo;
- una conclusión.

---

# 18. Decisión

**Decisión**

Elección realizada entre alternativas dentro de un contexto determinado.

Una decisión importante debe conservar, cuando sea relevante:

- problema;
- contexto;
- alternativas;
- criterios;
- evidencia;
- elección;
- consecuencias.

---

# 19. Decision Lineage

**Decision Lineage — Linaje de decisión**

Trazabilidad histórica que conecta una decisión con:

- el problema que la originó;
- su contexto;
- las alternativas consideradas;
- la evidencia utilizada;
- y sus consecuencias.

Su propósito es conservar el **por qué**, no solamente el **qué**.

---

# 20. Proveniencia

**Proveniencia**

Historia que permite identificar el origen y transformación de un elemento de conocimiento.

Puede responder:

> ¿De dónde provino este conocimiento?

> ¿Qué evidencia lo originó?

> ¿Qué interpretaciones sufrió?

> ¿Qué decisiones derivaron de él?

---

# 21. Historia

**Historia**

Secuencia de estados, acontecimientos, decisiones y transformaciones que permite comprender cómo se llegó al estado actual.

En EOS:

> **La historia es parte del conocimiento cuando explica su significado.**

---

# 22. Contexto histórico

**Contexto histórico**

Conjunto de condiciones, circunstancias, decisiones y conocimientos disponibles en un momento determinado que permiten comprender por qué algo ocurrió de determinada manera.

El contexto histórico evita evaluar decisiones antiguas únicamente con conocimiento adquirido posteriormente.

---

# 23. Temporalidad

**Temporalidad**

Dimensión que permite representar el momento, secuencia o evolución de acontecimientos y conocimientos.

La temporalidad permite distinguir entre:

- antes;
- durante;
- después;
- vigente;
- reemplazado;
- obsoleto.

---

# 24. Vigencia

**Vigencia**

Condición que indica si un conocimiento, decisión, configuración o principio continúa siendo aplicable dentro de un contexto determinado.

Un conocimiento histórico puede conservarse aunque ya no esté vigente.

---

# 25. Obsolescencia

**Obsolescencia**

Estado de un conocimiento, tecnología, decisión o artefacto que ha dejado de ser aplicable o recomendable debido a cambios en contexto, tecnología, evidencia o necesidades.

Obsoleto no significa inútil.

Puede conservar valor histórico.

---

# 26. Hipótesis

**Hipótesis**

Proposición provisional utilizada para explicar o predecir un fenómeno y que requiere validación mediante evidencia.

Una hipótesis no debe registrarse como conocimiento confirmado mientras su grado de incertidumbre sea relevante.

---

# 27. Conclusión

**Conclusión**

Interpretación derivada de evidencia y razonamiento dentro de un contexto determinado.

Una conclusión puede posteriormente convertirse en conocimiento consolidado si demuestra utilidad y estabilidad.

---

# 28. Resultado

**Resultado**

Consecuencia observable de una acción, decisión, experimento, implementación o proyecto.

Un resultado puede confirmar, cuestionar o modificar conocimiento existente.

---

# 29. Aprendizaje

**Aprendizaje**

Cambio significativo en la comprensión, capacidad o criterio producido por una experiencia.

El aprendizaje constituye uno de los principales mecanismos mediante los cuales EOS convierte experiencia en conocimiento acumulativo.

---

# 30. Patrón

**Patrón**

Regularidad identificada mediante la observación de múltiples experiencias o casos suficientemente relacionados.

Un patrón no debe confundirse automáticamente con una regla universal.

---

# 31. Principio

**Principio**

Regla conceptual suficientemente general y estable que orienta decisiones o comportamiento.

Dentro de EOS, un principio debe ser:

- comprensible;
- justificable;
- suficientemente general;
- y estable frente a cambios de implementación.

---

# 32. Regla

**Regla**

Criterio explícito que determina cómo debe actuarse en una situación determinada.

Una regla suele ser más concreta que un principio.

---

# 33. Procedimiento

**Procedimiento**

Secuencia definida de acciones para alcanzar un resultado específico.

Los procedimientos pertenecen principalmente al nivel operativo y pueden cambiar con las herramientas y condiciones.

---

# 34. Baseline

**Baseline — Línea base**

Estado formalmente reconocido de una parte del EOS que sirve como referencia para futuras modificaciones.

Una baseline no significa perfección.

Significa:

> **un estado conocido, identificado y deliberadamente establecido.**

---

# 35. Evolución

**Evolución**

Proceso mediante el cual el EOS, su conocimiento o sus estructuras cambian como consecuencia de nueva experiencia, evidencia, necesidades o comprensión.

La evolución debe conservar continuidad histórica cuando ésta tenga valor.

---

# 36. Cambio arquitectónico

**Cambio arquitectónico**

Modificación que afecta la estructura conceptual o las reglas fundamentales de EOS.

Debido a su impacto, debe justificarse mediante evidencia o necesidad significativa.

---

# 37. Núcleo

**Núcleo**

Conjunto mínimo de conceptos y principios que define la identidad y estabilidad fundamental de EOS.

El núcleo debe cambiar lentamente.

---

# 38. Periferia

**Periferia**

Conjunto de componentes, herramientas, estructuras y mecanismos que pueden evolucionar alrededor del núcleo sin modificar necesariamente la identidad del EOS.

La periferia es el principal espacio para la experimentación.

---

# 39. Implementación

**Implementación**

Forma concreta en que la arquitectura conceptual de EOS se materializa mediante estructuras, archivos, herramientas, sistemas y procesos.

La implementación puede cambiar sin necesariamente cambiar la arquitectura.

---

# 40. Herramienta

**Herramienta**

Software, hardware o servicio utilizado para implementar, administrar, producir o acceder al EOS.

Ejemplos actuales pueden incluir:

- Obsidian;
- Git;
- GitHub;
- Markdown;
- scripts;
- sistemas operativos.

Las herramientas no forman parte de la identidad conceptual del EOS.

---

# 41. Repositorio

**Repositorio**

Espacio estructurado destinado a almacenar y versionar artefactos y conocimiento de EOS.

Un repositorio es una implementación, no el EOS completo.

---

# 42. Fuente de verdad

**Fuente de verdad**

Referencia principal que representa el estado autorizado de un determinado conocimiento, artefacto o configuración.

Su propósito es evitar ambigüedad entre múltiples copias.

---

# 43. Versionado

**Versionado**

Mecanismo mediante el cual diferentes estados de un artefacto o conocimiento pueden identificarse y recuperarse.

El versionado permite conservar evolución.

No todo contenido requiere el mismo nivel de versionado.

---

# 44. Reutilización

**Reutilización**

Aplicación de conocimiento previamente adquirido en un contexto diferente.

La reutilización correcta requiere conservar las condiciones bajo las cuales el conocimiento original resultó válido.

---

# 45. Transferencia de conocimiento

**Transferencia de conocimiento**

Proceso mediante el cual conocimiento desarrollado en un contexto puede ser comprendido y utilizado en otro.

La transferencia requiere algo más que copiar información.

Requiere conservar significado y contexto.

---

# 46. Reentrada

**Reentrada**

Capacidad de regresar a un proyecto, problema o cuerpo de conocimiento después de un periodo de ausencia y reconstruir suficientemente su contexto para continuar trabajando.

La reentrada es una propiedad importante de un EOS de larga duración.

---

# 47. Memoria institucional

**Memoria institucional**

Conjunto de conocimientos, decisiones, experiencias, criterios y contexto preservados para permitir continuidad más allá de las personas o circunstancias que los originaron.

EOS puede actuar como infraestructura de memoria institucional.

---

# 48. Bus Factor

**Bus Factor**

Indicador informal del grado en que un sistema depende del conocimiento exclusivo de una o pocas personas.

Un Bus Factor bajo indica alta vulnerabilidad ante la pérdida de esas personas.

EOS busca reducir esta vulnerabilidad mediante la preservación de conocimiento significativo.

---

# 49. Ruido

**Ruido**

Información almacenada que no aporta suficiente valor futuro, contexto o capacidad de comprensión para justificar su conservación dentro de una estructura determinada.

El ruido puede dificultar la recuperación de conocimiento.

---

# 50. Señal

**Señal**

Información o conocimiento que posee relevancia suficiente para mejorar comprensión, decisión, aprendizaje o acción futura.

EOS busca maximizar la relación:

> **Señal / Ruido**

sin sacrificar contexto necesario.

---

# 51. Fricción

**Fricción**

Esfuerzo adicional necesario para capturar, mantener, recuperar o utilizar conocimiento dentro de EOS.

Una fricción excesiva reduce la probabilidad de uso correcto del sistema.

---

# 52. Reversibilidad

**Reversibilidad**

Propiedad de una decisión o implementación que permite modificarla o deshacerla sin consecuencias desproporcionadas.

Las decisiones experimentales deberían favorecer la reversibilidad cuando sea posible.

---

# 53. Conocimiento provisional

**Conocimiento provisional**

Conocimiento actualmente considerado útil o plausible, pero cuyo grado de certeza, generalidad o vigencia todavía puede cambiar.

Debe poder evolucionar sin perder su historia.

---

# 54. Conocimiento consolidado

**Conocimiento consolidado**

Conocimiento que ha adquirido suficiente evidencia, experiencia o estabilidad como para ser considerado una referencia confiable dentro de un contexto definido.

Consolidado no significa universalmente verdadero.

---

# 55. Preservación

**Preservación**

Conjunto de acciones destinadas a mantener conocimiento accesible y comprensible a través del tiempo.

La preservación incluye:

- contenido;
- contexto;
- relaciones;
- integridad;
- y posibilidad de recuperación.

---

# 56. Recuperación

**Recuperación**

Capacidad de localizar y comprender conocimiento previamente preservado cuando éste vuelve a ser necesario.

Recuperar no significa simplemente encontrar un archivo.

Significa recuperar:

> **información suficiente para reconstruir significado.**

---

# 57. Recuperabilidad

**Recuperabilidad**

Propiedad de un sistema de conocimiento que permite localizar, acceder y comprender información previamente preservada.

Un conocimiento que no puede recuperarse cuando se necesita posee un valor práctico significativamente menor.

---

# 58. Integridad

**Integridad**

Condición en la cual el conocimiento y sus relaciones se mantienen completos y no han sufrido modificaciones o pérdidas no autorizadas.

---

# 59. Resiliencia

**Resiliencia**

Capacidad del EOS para continuar preservando y proporcionando conocimiento frente a:

- fallas;
- pérdida de herramientas;
- cambios tecnológicos;
- cambios organizacionales;
- o discontinuidades humanas.

---

# 60. Portabilidad

**Portabilidad**

Capacidad de trasladar conocimiento y estructura entre herramientas o plataformas sin pérdida significativa de significado.

---

# 61. Ingeniería

**Ingeniería**

Dentro del contexto EOS, disciplina práctica de comprender problemas, diseñar soluciones, construir sistemas, experimentar, medir resultados y aprender de ellos.

El término se utiliza deliberadamente en un sentido amplio.

---

# 62. Engineering Chronicle

**Engineering Chronicle — Crónica de Ingeniería**

Registro histórico destinado a conservar acontecimientos, decisiones, aprendizajes y evolución significativa del trabajo de ingeniería.

La Chronicle proporciona continuidad temporal al EOS.

---

# 63. ADR

**ADR — Architecture Decision Record**

Registro estructurado de una decisión arquitectónica significativa.

Un ADR normalmente conserva:

- contexto;
- problema;
- alternativas;
- decisión;
- consecuencias.

Dentro de EOS, los ADR constituyen una herramienta para preservar **Decision Lineage**.

---

# 64. Postmortem

**Postmortem**

Registro realizado después de un evento significativo —especialmente un fallo o resultado inesperado— para comprender qué ocurrió y qué puede aprenderse.

Un postmortem correctamente utilizado transforma un evento pasado en conocimiento futuro.

---

# 65. Knowledge Lineage

**Knowledge Lineage — Linaje del conocimiento**

Historia que permite reconstruir cómo un conocimiento fue:

```
Generado
   ↓
Observado
   ↓
Interpretado
   ↓
Validado
   ↓
Utilizado
   ↓
Modificado
```

Es la dimensión histórica del conocimiento.

---

# 66. Decision Lineage vs. Knowledge Lineage

Ambos conceptos están relacionados, pero no son equivalentes.

### Decision Lineage

Pregunta:

> **¿Por qué tomamos esta decisión?**

### Knowledge Lineage

Pregunta:

> **¿Cómo llegamos a saber esto?**

Pueden converger:

```
Evidencia
   ↓
Conocimiento
   ↓
Decisión
   ↓
Resultado
   ↓
Nuevo conocimiento
```

---

# 67. Contexto vs. Historia

Estos conceptos tampoco son equivalentes.

### Contexto

Explica:

> **¿Qué condiciones rodeaban algo?**

### Historia

Explica:

> **¿Cómo llegó a existir o evolucionar?**

El contexto puede ser instantáneo.

La historia requiere temporalidad.

Ambos son necesarios para comprender conocimiento de larga duración.

---

# 68. Conocimiento vs. Documentación

**Documentación** es la representación escrita, gráfica, digital o estructurada de información y conocimiento.

**Conocimiento** es el significado comprendido y reutilizable que esa documentación puede preservar.

Por tanto:

> **La documentación es un medio. El conocimiento es el propósito.**

---

# 69. Datos vs. conocimiento

La diferencia fundamental puede expresarse:

```
DATOS
  ↓
INFORMACIÓN
  ↓
CONTEXTO
  ↓
INTERPRETACIÓN
  ↓
CONOCIMIENTO
  ↓
DECISIÓN
  ↓
ACCIÓN
```

EOS se interesa principalmente por preservar los niveles superiores sin perder los inferiores necesarios para comprenderlos.

---

# 70. Arquitectura vs. implementación

**Arquitectura** responde:

> ¿Qué estructura conceptual debe existir?

**Implementación** responde:

> ¿Cómo materializamos esa estructura?

Una arquitectura puede sobrevivir a múltiples implementaciones.

---

# 71. Principio de vocabulario estable

Las definiciones de este glosario no deben modificarse casualmente.

Una modificación significativa de un término fundamental puede alterar la interpretación histórica de EOS.

Por ello, los cambios importantes de definición deben conservar:

- definición anterior;
- nueva definición;
- motivo del cambio;
- fecha;
- contexto.

---

# 72. Evolución del Glossary

El Glossary es un documento vivo.

Puede incorporar nuevos términos cuando:

1. aparezca un concepto recurrente;
2. exista ambigüedad significativa;
3. el concepto pase a formar parte del modelo;
4. o su definición sea necesaria para preservar comprensión.

No debe convertirse en un diccionario infinito.

---

# 73. Regla para incorporar términos

Antes de agregar un término debe preguntarse:

> **¿La ausencia de una definición común podría provocar una interpretación diferente del sistema?**

Si la respuesta es no, probablemente el término no pertenece al núcleo del Glossary.

---

# 74. Lenguaje como infraestructura

El lenguaje no es una capa superficial del EOS.

Las palabras determinan cómo pensamos sobre el conocimiento.

Si:

> "decisión"

significa una cosa hoy y otra cinco años después,

la trazabilidad se deteriora.

Si:

> "conocimiento"

se utiliza indistintamente para dato, archivo, conclusión y principio,

la arquitectura pierde precisión.

Por ello:

> **El vocabulario es infraestructura conceptual.**

---

# 75. Principio de estabilidad semántica

EOS debe preservar la estabilidad semántica de sus conceptos fundamentales.

Esto significa que:

> **las palabras que forman parte del modelo deben cambiar de significado mucho más lentamente que el contenido que describen.**

Esta propiedad es esencial para un sistema diseñado para décadas.

---

# 76. Glosario mínimo del núcleo

Si todo el Glossary tuviera que reducirse a un núcleo mínimo, éste sería:

```
EOS
│
├── Proyecto
├── Contexto
├── Evidencia
├── Conocimiento
├── Decisión
├── Artefacto
│
├── Relación
├── Historia
├── Proveniencia
├── Decision Lineage
└── Knowledge Lineage
```

Estos conceptos constituyen el vocabulario estructural principal de EOS.

---

# 77. Definición compacta del lenguaje EOS

Podemos resumir el lenguaje fundamental así:

> **Los proyectos generan experiencias.**

> **Las experiencias producen evidencia.**

> **La evidencia, interpretada dentro de un contexto, puede producir conocimiento.**

> **El conocimiento informa decisiones.**

> **Las decisiones producen acciones y artefactos.**

> **Los resultados producen nueva evidencia y nueva experiencia.**

> **La historia y las relaciones permiten que todo ello pueda ser comprendido posteriormente.**

---

# 78. El lenguaje como memoria

El Glossary cumple finalmente una función más profunda.

No solamente define palabras.

Preserva:

> **la forma en que EOS entiende el mundo de la ingeniería.**

Con el paso de los años, podrán cambiar:

- las herramientas;
- las tecnologías;
- los proyectos;
- las metodologías;
- incluso las disciplinas.

Pero mientras el vocabulario fundamental permanezca comprensible, será posible reconstruir la arquitectura intelectual que sostiene EOS.

---

# 79. Declaración final

> **El Glossary define el lenguaje mediante el cual EOS piensa, documenta y preserva conocimiento.**

> **Su propósito no es restringir el lenguaje, sino evitar que los conceptos fundamentales pierdan significado con el paso del tiempo.**

> **Las palabras constituyen las unidades del pensamiento; las relaciones entre ellas constituyen parte de la arquitectura del conocimiento.**

Y por ello:

> ## **Un sistema de conocimiento que pierde su lenguaje termina perdiendo parte de su memoria.**

El EOS conservará su vocabulario fundamental con el mismo cuidado con que conserva sus decisiones, evidencias y aprendizajes.

> ## **Construimos conocimiento para construir mejor.**

---

**EOS — Glossary**  
**Agosto de 2026**  
**Glossary Baseline 1.0**  
**Edición original en español**
