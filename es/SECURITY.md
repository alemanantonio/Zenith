# Política de seguridad

Este documento explica cómo reportar vulnerabilidades de seguridad en los proyectos de Zenith y qué esperar una vez recibido un reporte. Aplica a los repositorios listados en el [catálogo de productos](docs/projects.md).

## Cómo reportar una vulnerabilidad

Las vulnerabilidades de seguridad no deben reportarse en issues, discusiones, pull requests ni redes sociales públicas.

Repórtalas de forma privada, usando uno de estos canales:

1. **Reporte privado de vulnerabilidades de GitHub**, cuando esté habilitado en el repositorio afectado. Si la opción "Report a vulnerability" aparece en la pestaña de seguridad del repositorio, úsala.
2. **Un contacto privado publicado por los mantenedores**, cuando figure en este archivo o en el README del repositorio afectado.

**Pendiente:** aún no se ha publicado un contacto de seguridad dedicado. Hasta que exista, usa el reporte privado de vulnerabilidades del repositorio afectado cuando la opción esté disponible. Si no lo está, abre un issue sencillo solicitando un canal de contacto privado, sin incluir ningún detalle de la vulnerabilidad, y los mantenedores responderán con instrucciones.

## Qué incluir en un reporte

Incluye todo lo que puedas de lo siguiente:

- El repositorio afectado y la versión, etiqueta o commit donde ocurre la vulnerabilidad.
- Una descripción de la vulnerabilidad y su impacto potencial.
- Pasos para reproducirla, incluyendo cualquier configuración o dato requerido.
- Prueba de concepto, código de explotación o capturas de pantalla, si están disponibles.
- Correcciones o mitigaciones sugeridas, si las tienes.
- Si la vulnerabilidad ya se ha divulgado en algún lugar, y dónde.

Los reportes que permiten a un mantenedor reproducir el problema se atienden primero.

## Qué no debe publicarse

No incluyas lo siguiente en issues, pull requests, mensajes de commit o capturas de pantalla públicas:

- Credenciales, claves de API, tokens o cadenas de conexión.
- Datos personales de usuarios, clientes o terceros.
- Detalles de una vulnerabilidad explotable antes de que se acuerde una corrección o una divulgación coordinada.
- Información de infraestructura como nombres de host internos, direcciones IP o endpoints privados.

Cuando se necesiten registros o capturas, oculta los valores sensibles antes de publicarlos.

## Cómo se gestionan los reportes

Los proyectos de Zenith se mantienen con capacidad disponible limitada, y no se ha definido ningún tiempo de respuesta, plazo de corrección ni garantía de remediación. En general:

- Los reportes se leen y se clasifican según la capacidad disponible.
- Si el reporte se acepta, los mantenedores coordinarán con el reportero la divulgación y, cuando sea posible, una corrección y el crédito correspondiente.
- Si el reporte no se puede reproducir o está fuera de alcance, se informará al reportero cuando la comunicación sea posible.
- La severidad, la prioridad y las decisiones de release se toman en el repositorio del producto afectado.

Se pide al reportero mantener el asunto confidencial hasta que los mantenedores confirmen una corrección o acuerden una fecha de divulgación.

## Alcance

Esta política cubre vulnerabilidades del código y la configuración de los repositorios del [catálogo](docs/projects.md). No cubre:

- Vulnerabilidades en dependencias de terceros, que deben reportarse al proyecto correspondiente, aunque a los mantenedores les resulta útil enterarse para poder actualizarlas.
- Productos o servicios que no estén publicados en un repositorio de Zenith.
- Reportes de errores generales, que pertenecen al issue tracker público del repositorio (consulta [CONTRIBUTING.md](CONTRIBUTING.md)).
