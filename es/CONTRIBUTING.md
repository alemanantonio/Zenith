# Contribuir a Zenith

Zenith es un conjunto de proyectos open source independientes. Este documento explica cómo participar en ellos. Describe únicamente un flujo general: cada producto define dentro de su propio repositorio su proceso de compilación, su stack, sus herramientas y sus requisitos de pruebas, y esas definiciones prevalecen sobre cualquier cosa escrita aquí.

## Identificar el repositorio correcto

Cada producto vive en su propio repositorio. Las contribuciones pertenecen al repositorio que posee el código o la documentación que afectan:

| Si quieres... | Empieza aquí |
| --- | --- |
| Reportar un problema o proponer una función para un producto | El repositorio del producto (consulta el [catálogo](docs/projects.md)) |
| Mejorar el catálogo o los documentos de contribución, seguridad o conducta | [alemanantonio/Zenith](https://github.com/alemanantonio/Zenith) |
| Reportar un problema en más de un producto | Issues separados, uno por repositorio |

Si no estás seguro de dónde encaja algo, abre un issue en el repositorio que parezca más cercano y dilo. Los mantenedores pueden mover la conversación o indicarte dónde corresponde. No abras el mismo issue en varios repositorios.

## Antes de empezar

1. Lee el README del repositorio de destino. Debería describir el producto, su estado actual y su configuración de desarrollo.
2. Busca los issues y pull requests existentes de ese repositorio para evitar duplicar trabajo.
3. Comprueba si el repositorio tiene su propio `CONTRIBUTING.md`, estándares de código o guía de desarrollo. Si los tiene, síguelos en lugar de este documento.
4. Para cambios de gran tamaño, abre primero un issue para confirmar el alcance antes de invertir tiempo en una implementación.

## Reportar errores

Abre un issue en el repositorio del producto e incluye:

- El repositorio y, si corresponde, la versión, etiqueta o commit donde ocurre el problema.
- Los pasos para reproducir el problema, lo más concretamente posible.
- Qué esperabas y qué ocurrió realmente.
- Tu entorno: sistema operativo, runtime y versión, navegador u otros detalles relevantes.
- Registros, capturas de pantalla o mensajes de error que ayuden a reproducir el problema. Antes, elimina credenciales, tokens y datos personales (consulta [SECURITY.md](SECURITY.md)).

Un buen reporte de error debe poder reproducirse por otra persona sin necesidad de hacer preguntas de seguimiento.

## Proponer mejoras

Usa los issues para proponer:

- Un defecto que hayas confirmado.
- Una mejora concreta y acotada al comportamiento actual.
- Lagunas de documentación que hayas encontrado.

Describe el problema que resuelve el cambio y a quién afecta. Las ideas que no se vinculan con un problema concreto son más difíciles de evaluar. Las hojas de ruta, las versiones y las prioridades se deciden en el repositorio de cada producto, así que espera que la conversación ocurra allí.

## Buenas prácticas para issues

- Un problema o una propuesta por issue.
- Usa un título claro y específico: qué está mal o qué debe cambiar, no "bug" o "ayuda".
- Aporta el contexto solicitado arriba; los issues que no se pueden entender ni reproducir son difíciles de gestionar.
- Mantén la conversación en el issue, sobre el tema y de forma objetiva.
- No publiques vulnerabilidades de seguridad en issues públicos. Sigue [SECURITY.md](SECURITY.md).

## Buenas prácticas para pull requests

- Haz un fork del repositorio de destino y crea una rama a partir de su rama predeterminada.
- Mantén cada pull request limitado a un solo cambio o a un conjunto pequeño de cambios relacionados. Los arreglos sin relación van en un pull request aparte.
- Explica qué hace el cambio y por qué, y vincula el issue que aborda.
- Sigue el estilo de código, la estructura y las convenciones ya presentes en ese repositorio. No reformates, renombres ni refactorices código fuera del alcance del cambio.
- Añade o actualiza documentación y pruebas cuando las guías del repositorio lo exijan.
- Espera una revisión. Responde al feedback o explica por qué no estás de acuerdo.

## Requisitos de calidad

Todo cambio debe ser:

- **Comprensible.** El título, la descripción y el código dejan clara la intención sin contexto previo.
- **Acotado.** Toca solo lo necesario. Los refactors, las actualizaciones de dependencias y las funciones nuevas son contribuciones aparte.
- **Consistente.** Coincide con las convenciones del repositorio al que se dirige.
- **Completo.** No deja compilaciones rotas, referencias muertas ni documentación que contradiga el cambio.

## Respetar las decisiones de cada producto

Los productos difieren a propósito. El stack, la arquitectura, los nombres y las decisiones tomadas en el repositorio de un producto son decisiones deliberadas de ese proyecto. Contribuye dentro de ellas en lugar de importar las convenciones de otro producto de Zenith o de tus propios proyectos. Si discrepas de una dirección, planteala en un issue y argumenta el caso; no uses un pull request para imponer otro enfoque.

## Encontrar instrucciones específicas de cada producto

La configuración de desarrollo se documenta por producto, junto al producto:

- Empieza por el `README.md` del producto.
- Busca un `CONTRIBUTING.md`, un directorio `docs/` o una guía de desarrollo en ese repositorio.
- Consulta los issues y el tablero de proyectos del repositorio para ver el trabajo activo.

Este catálogo no publica comandos de compilación, listas de dependencias ni instrucciones de pruebas en nombre de los productos, porque esos detalles les pertenecen y cambian con cada uno.

## Lo que este documento no define

Para ser explícito: no existe un único proceso de compilación, framework, lenguaje, linter o suite de pruebas compartido por todos los proyectos de Zenith. Este documento no define ninguno a propósito. Consulta el repositorio al que contribuyes.
