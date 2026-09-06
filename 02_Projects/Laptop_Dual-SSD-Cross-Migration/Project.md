# Laptop Dual-SSD Cross-Migration

## Objetivo

Intercambiar las instalaciones de sistema operativo entre dos SSD del mismo
laptop, preservando ambos sistemas y dejando cada uno en el SSD definido como
estado final.

Estado objetivo:

* SSD de 120 GB → Windows 11 Pro
* SSD de 500 GB → Linux Mint 22.3 Cinnamon

Ambos sistemas operativos deben permanecer funcionales y poder iniciarse de
forma independiente después de la migración.

## Contexto

EOS está siendo desarrollado como un sistema de conocimiento y trabajo de
largo plazo para proyectos de ingeniería de interés a corto, mediano y largo
plazo.

El laptop utilizado actualmente dispone de un SSD de 120 GB con Linux Mint
22.3 Cinnamon. Existe además un SSD de 500 GB que anteriormente fue utilizado
en el mismo laptop y contiene una instalación funcional de Windows 11 Pro.

El espacio disponible en el SSD actual comienza a ser una limitación para el
desarrollo y almacenamiento de los distintos proyectos que forman parte de
EOS. Por esta razón se utilizará el SSD de 500 GB como unidad principal,
manteniendo ambos sistemas operativos disponibles.

El proyecto consiste, por tanto, en realizar el intercambio de las
instalaciones entre ambos SSD de manera controlada, verificable y recuperable.

Este proyecto constituye además un proyecto técnico real para validar la
arquitectura de EOS y su implementación mediante Obsidian.

## Estado Inicial

### SSD A

* Capacidad: 120 GB
* Sistema operativo: Linux Mint 22.3 Cinnamon
* Estado actual: unidad de sistema activa

### SSD B

* Capacidad: 500 GB
* Sistema operativo: Windows 11 Pro
* Estado actual: instalación previamente funcional utilizada en el mismo laptop

Configuración inicial:

```
SSD A → Linux Mint 22.3
SSD B → Windows 11 Pro
```

## Estado Objetivo

Configuración final:

```
SSD A → Windows 11 Pro
SSD B → Linux Mint 22.3 Cinnamon
```

Ambos sistemas deben iniciar correctamente y funcionar de manera independiente
después del intercambio físico de las unidades.

## Restricciones

* Ambos sistemas operativos deben conservarse.
* Ningún SSD debe ser sobrescrito antes de disponer de una ruta de recuperación
  verificada.
* La instalación de Windows debe poder ser trasladada al SSD de 120 GB.
* La instalación de Linux debe poder ser trasladada al SSD de 500 GB.
* Debe conservarse la capacidad de arranque de ambos sistemas.
* Las operaciones destructivas deben realizarse solamente después de verificar
  la información necesaria.
* El proceso debe ser recuperable ante una eventual falla.
* Los resultados y evidencias relevantes deben conservarse.
* El SSD de 500 GB debe quedar disponible como espacio principal para el
  desarrollo futuro de EOS y sus proyectos.

## Estado Actual

El proyecto se encuentra en fase de Discovery. No se ha modificado ninguno de los dos SSD. El objetivo de esta fase es determinar el estado real de ambas unidades antes de realizar cualquier operación de migración. Se debe inspeccionar y documentar, como mínimo:
* identificación física de las unidades;
* capacidad real;
* tabla de particiones;
* particiones EFI y de sistema;
* sistemas de archivos;
* espacio utilizado y disponible;
* estructura de arranque;
* configuración relevante de cada sistema operativo;
* cualquier condición que pueda afectar la migración.

No se realizará ninguna operación destructiva durante esta fase.

## Decisiones

* Se conservarán ambos sistemas operativos.
* El SSD de 120 GB contendrá finalmente Windows 11 Pro.
* El SSD de 500 GB contendrá finalmente Linux Mint 22.3 Cinnamon.
* No se realizará ninguna operación destructiva sin una ruta de recuperación
  verificada.
* La migración se realizará como un proceso controlado y por etapas.
* El SSD de 500 GB será utilizado como unidad principal para disponer de mayor
  capacidad de almacenamiento para EOS y sus proyectos futuros.

## Información Relacionada

[[Chronicle]]

## Estado

Discovery
