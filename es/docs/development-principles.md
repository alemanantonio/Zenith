# Principios de desarrollo

Este documento define cómo se organizan y se desarrollan los proyectos open source de Zenith. Aplica a este catálogo y está destinado a ser respetado por cada repositorio de producto de Zenith. Las reglas específicas de un producto viven siempre en el repositorio de ese producto y prevalecen sobre cualquier cosa escrita aquí.

## Cada producto es un proyecto independiente

Cada producto es un repositorio independiente con su propia identidad, alcance y base de código. Los productos no comparten un monorepo, y el intercambio de código nunca es un requisito para contribuir a un producto o usarlo. Un cambio en un producto no debe forzar cambios en otro.

La independencia también significa independencia de decisiones: un producto puede elegir el stack, la licencia y la estructura que encajen con su problema, incluso cuando otro producto de Zenith eligió diferente.

## Cada repositorio gestiona su propio ciclo de desarrollo

El repositorio del producto es dueño de:

- Su hoja de ruta y las prioridades de sus mantenedores.
- Su esquema de versiones y sus releases.
- Sus dependencias y su cadencia de actualización.
- Su issue tracker y su definición de terminado.

No existe un calendario de releases compartido, ni versiones coordinadas entre productos, ni requisito de que los productos adopten una versión común de sus dependencias. Un retraso o un cambio mayor en un producto no dice nada sobre los demás.

## Las decisiones arquitectónicas pertenecen al repositorio del producto

La conversación sobre el diseño, el stack o la dirección de un producto ocurre en los issues y pull requests de ese producto, con las personas que lo mantienen y lo usan. Este catálogo no decide, respalda ni anula decisiones técnicas de ningún producto.

Las decisiones que afectan a los usuarios, como cambios incompatibles o el fin del soporte, se documentan en las notas de versión y el README del propio producto.

## Las contribuciones respetan la tecnología y las convenciones del producto

Una contribución a un producto debe funcionar dentro de las tecnologías, la estructura, los nombres y las convenciones ya establecidas en ese repositorio. Los contribuidores no deben introducir patrones tomados de otro producto de Zenith sin debatirlo en el repositorio donde aterriza el cambio. El flujo general de [../CONTRIBUTING.md](../CONTRIBUTING.md) describe cómo participar; el producto define cómo compilar, probar y formatear su código.

## La documentación vive junto al producto al que describe

La documentación del producto — README, guías, referencia de API, instrucciones de despliegue — se mantiene dentro del repositorio del producto, donde cambia junto al código.

Este catálogo central contiene solo material de catálogo: qué es Zenith, qué productos existen, su estado verificado y las políticas generales de contribución, seguridad y conducta. Enlaza con la documentación del producto en lugar de copiarla, e informa solo de datos que pueden verificarse en los repositorios.

## El autoalojamiento se documenta solo cuando es real

Un producto puede declarar que puede autoalojarse únicamente cuando su repositorio contiene realmente las instrucciones y los requisitos para hacerlo. Hasta entonces, el catálogo describe el autoalojamiento de ese producto como no documentado, no como soportado. Consulta [self-hosting.md](self-hosting.md).

## Fuera del alcance de Zenith en su conjunto

Para evitar ambigüedades, lo siguiente forma explícitamente parte de estos principios:

- Un monorepo obligatorio o una base de código compartida entre productos.
- Un único proceso de compilación, framework, lenguaje o suite de pruebas para todos los proyectos.
- Un calendario de releases compartido o versiones coordinadas entre productos.
- Dependencias obligatorias entre productos, en ninguna dirección.
- Aprobación central de la hoja de ruta técnica de un producto por parte de este repositorio de catálogo.
