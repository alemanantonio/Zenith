# Zenith

Versión en inglés de este documento: [README.md](../README.md).

Zenith es una marca de software que ofrece servicios de desarrollo y mantiene un conjunto de productos desarrollados en abierto. Este repositorio es el catálogo central de los proyectos open source de Zenith: explica qué es Zenith, lista los productos disponibles y enlaza con el repositorio, la documentación y los canales de soporte de cada uno.

Cada producto se desarrolla de forma independiente en su propio repositorio, donde viven su código, su arquitectura, sus dependencias, sus versiones, sus releases, sus issues y su hoja de ruta. Este catálogo es un punto de entrada a esos proyectos. No duplica ni sustituye la documentación mantenida dentro de cada producto.

## Enfoque open source

Zenith publica sus productos como repositorios públicos para que cualquiera pueda inspeccionar el código, reportar problemas, proponer cambios y, cuando un producto lo permite, ejecutar el software en su propia infraestructura.

En la práctica, esto significa:

- El repositorio de cada producto es la fuente de verdad de su código, su documentación, sus issues y sus releases.
- El estado que se informa en este catálogo se limita a lo que puede verificarse en esos repositorios. Las funciones que no se han publicado no se describen como disponibles.
- Las licencias, las notas de versión y las instrucciones de instalación se definen por repositorio, no para la marca en su conjunto.

## Productos

Estado de los repositorios verificado el 2026-10-09 contra los repositorios públicos de [github.com/alemanantonio](https://github.com/alemanantonio).

| Producto | Descripción | Estado verificado | Repositorio |
| --- | --- | --- | --- |
| **Zenith** | Catálogo central y punto de entrada de los proyectos open source de Zenith. | Solo documentación de catálogo; sin código de producto. | [alemanantonio/Zenith](https://github.com/alemanantonio/Zenith) |
| **Zenith-SaaS** | Producto de software como servicio (SaaS). | Repositorio creado. | [alemanantonio/Zenith-SaaS](https://github.com/alemanantonio/Zenith-SaaS) |
| **Zenith-Inventario** | Sistema de gestión de inventario. | Repositorio creado. | [alemanantonio/Zenith-Inventario](https://github.com/alemanantonio/Zenith-Inventario) |
| **Zenith-Dashboard** | Dashboard y herramientas integradas. | Repositorio creado. | [alemanantonio/Zenith-Dashboard](https://github.com/alemanantonio/Zenith-Dashboard) |
| **Zenith-Web** | Sitio web público de la marca Zenith. | Repositorio creado. | [alemanantonio/Zenith-Web](https://github.com/alemanantonio/Zenith-Web) |

Las descripciones provienen del propietario del proyecto y aún no han sido corroboradas con código publicado. El detalle de cada producto se mantiene en [docs/projects.md](docs/projects.md).

### Instrucciones de instalación

Las instrucciones de instalación y de uso se enlazan aquí únicamente cuando existen en el repositorio del producto correspondiente. Ninguna está publicada en este momento. Consulta [docs/self-hosting.md](docs/self-hosting.md) para conocer el estado de la documentación de autoalojamiento.

## Documentación

| Documento | Contenido |
| --- | --- |
| [docs/projects.md](docs/projects.md) | Catálogo detallado: propósito, funcionalidad verificada, tecnologías, estado y enlaces de cada producto. |
| [docs/development-principles.md](docs/development-principles.md) | Principios que rigen cómo se organizan y se desarrollan los repositorios de Zenith. |
| [docs/self-hosting.md](docs/self-hosting.md) | Introducción al autoalojamiento y a la documentación que cada producto debe aportar. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Cómo reportar issues, proponer cambios y contribuir en los repositorios de Zenith. |
| [SECURITY.md](SECURITY.md) | Cómo reportar vulnerabilidades de forma responsable. |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) | Comportamiento esperado en los espacios de los proyectos de Zenith. |

## Contribuir

Las contribuciones se hacen en el repositorio del producto al que afectan, no en este catálogo. Antes de abrir un issue o un pull request, identifica el repositorio que posee el código o la documentación que quieres modificar; el flujo general se describe en [CONTRIBUTING.md](CONTRIBUTING.md), y las instrucciones específicas de desarrollo se mantienen dentro de cada repositorio de producto.

## Principios

- **Independencia de los productos.** Cada repositorio es un proyecto independiente con su propia base de código, sus decisiones y su identidad. No hay un monorepo compartido ni intercambio de código obligatorio entre productos.
- **Mantenibilidad.** Los cambios se mantienen dentro del alcance de un solo producto y siguen las convenciones ya establecidas en él.
- **Transparencia.** El desarrollo ocurre en público: los issues, las decisiones y los releases quedan registrados en el repositorio donde se desarrolla el producto.
- **Autoalojamiento cuando está soportado.** Un producto documenta instrucciones de autoalojamiento solo cuando realmente permite ejecutarse en una infraestructura que tú controlas.

Estos principios se describen con detalle en [docs/development-principles.md](docs/development-principles.md).

## Estado de este catálogo

La disponibilidad de los repositorios, los enlaces y el estado de este documento se comprobaron contra la API de GitHub el 2026-10-09. Actualiza esa fecha cada vez que se revise el catálogo, y elimina las entradas que ya no reflejen el estado de los repositorios.
