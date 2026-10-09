# Autoalojamiento

## Qué significa autoalojarse

Autoalojarse (self-hosting) significa ejecutar un producto en una infraestructura que tú controlas — tus propios servidores, una máquina en casa o una cuenta en la nube que gestionas — en lugar de depender exclusivamente de un servicio operado por otra persona.

Autoalojarse te da normalmente control sobre la ubicación de los datos, el momento de las actualizaciones, la personalización y el coste a largo plazo. También te da responsabilidades: instalación, actualizaciones, copias de seguridad, parches de seguridad y disponibilidad. Si ese intercambio merece la pena depende por completo de cada producto, porque un producto debe publicar su código, sus requisitos y sus instrucciones de despliegue antes de que alguien pueda ejecutarlo.

Los productos de Zenith son proyectos independientes. Por eso, la posibilidad de autoalojarse se decide y se documenta por producto, nunca para la marca en su conjunto.

## Estado actual de los productos de Zenith

A 2026-10-09, ninguno de los repositorios de producto de Zenith contiene documentación de instalación, contenedores o despliegue. Este catálogo no afirma que ningún producto de Zenith pueda autoalojarse hoy.

| Producto | Documentación de autoalojamiento | Dónde vivirá |
| --- | --- | --- |
| [Zenith-SaaS](https://github.com/alemanantonio/Zenith-SaaS) | No disponible | En el repositorio del producto, cuando se publique |
| [Zenith-Inventario](https://github.com/alemanantonio/Zenith-Inventario) | No disponible | En el repositorio del producto, cuando se publique |
| [Zenith-Dashboard](https://github.com/alemanantonio/Zenith-Dashboard) | No disponible | En el repositorio del producto, cuando se publique |
| Zenith-Web | No aplica | Repositorio no accesible públicamente |
| [Zenith](https://github.com/alemanantonio/Zenith) (este catálogo) | No aplica | No contiene software ejecutable |

Tampoco está documentado todavía si alguno de estos productos es un servicio alojado que los usuarios no puedan desplegar, o software destinado a instalarse. Esa declaración en sí misma forma parte de la documentación que cada producto debe aportar a sus usuarios.

## Dónde debe vivir la documentación de autoalojamiento

Las instrucciones de autoalojamiento se mantienen en el propio repositorio del producto, junto a su código, para que puedan actualizarse en el mismo cambio que altere el comportamiento de despliegue. Ubicaciones típicas, cuando un producto admita autoalojamiento:

- El `README.md` del producto, con un resumen breve de la instalación.
- Un directorio `docs/` con una guía de despliegue.
- Definiciones de contenedor o despliegue (por ejemplo un archivo Dockerfile o de compose), solo si el producto las incluye realmente.
- Notas de versión, describiendo todo lo que afecte a instalaciones existentes al actualizar.

Este catálogo enlaza con esos documentos. No reproduce comandos, variables de entorno ni requisitos de infraestructura, porque esos detalles cambian con cada release y le pertenecen al producto.

## Información que cada producto debe publicar antes de que el autoalojamiento se anuncie

Un producto está listo para figurar como autoalojable en este catálogo cuando su repositorio documente:

- Sistemas operativos y arquitecturas soportados.
- Runtimes y versiones requeridos, y servicios externos necesarios como bases de datos o almacenamiento de objetos.
- Configuración: variables de entorno, archivos de configuración, secretos y sus valores por defecto.
- Pasos de compilación e instalación, desde una máquina limpia hasta una instancia en funcionamiento.
- Persistencia de datos: qué debe respaldarse y dónde se almacena.
- La ruta de actualización entre versiones, incluidas las migraciones.
- Expectativas de reverse proxy y TLS, si el producto sirve HTTP.
- Requisitos aproximados de recursos.
- Limitaciones conocidas y consideraciones de seguridad para despliegues expuestos.
- Los términos de licencia que aplican al autoalojamiento del producto.

Hasta que un producto documente estos puntos, el estado honesto es "no documentado", y este catálogo lo informará así.

## Si quieres autoalojar un producto de Zenith hoy

- Consulta primero el repositorio del producto: si existe documentación, estará allí, no aquí.
- Si no se ha publicado nada, puedes abrir un issue en el repositorio del producto solicitando documentación de despliegue, siguiendo [../CONTRIBUTING.md](../CONTRIBUTING.md).
- No infieras pasos de despliegue a partir de archivos parciales, y no asumas que un repositorio vacío puede instalarse.

## Para mantenedores

Cuando un producto adquiera soporte de autoalojamiento, publica la documentación en el repositorio del producto y después actualiza este archivo y la entrada del producto en [projects.md](projects.md), cambiando su estado de "no documentado" a la capacidad verificada, con un enlace a las instrucciones. Mantén este catálogo factual: declara solo lo que el repositorio del producto pueda demostrar.
