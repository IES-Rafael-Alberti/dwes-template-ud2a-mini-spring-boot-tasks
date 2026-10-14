# Mini Spring Boot Tasks — repositorio de grupo

Este repositorio es el punto de partida de la práctica cooperativa **Mini Spring
Boot Tasks** de DWES. Cada grupo trabaja en su propio *fork* de este repositorio;
el código, los commits, las pruebas y los documentos requeridos se mantienen aquí.

## Empezar

1. Una persona del grupo hace **Fork** de este repositorio en su cuenta de
   GitHub. No uses «Use this template»: el fork conserva las etiquetas y el
   historial pedagógico.
2. Desde el fork del grupo, añade a las demás personas como colaboradoras y
   clónalo en los equipos de trabajo.
3. Usa `main` como rama de trabajo: contiene la versión **v4** y es la base del
   slice adicional. El historial también conserva `v1`, `v2`, `v3`, `v4` y
   `v4-extras`.
4. Explora las etapas sin trabajar en una etiqueta separada:

   ```bash
   git log --oneline --decorate --graph --all
   git tag --list
   git switch --detach v1
   git switch main
   ```

5. Implementa el slice acordado por el grupo sobre `main`. Cada integrante debe
   realizar y subir commits con su propia cuenta; no compartáis credenciales.
6. Ejecuta las pruebas con `mvn test`, confirma que están verdes y sube los
   cambios a **tu fork**.
7. Entrega en la tarea de Moodle únicamente la URL del fork. Moodle sirve para
   localizar el repositorio; todo lo que se evalúa debe estar dentro de él.

## Funcionalidad vertical (slice) adicional

Un *slice* es una funcionalidad pequeña completa de extremo a extremo, no una
capa aislada. Por ejemplo, filtrar tareas por estado recorre la petición HTTP, el
controlador, el servicio, la consulta del repositorio y la respuesta JSON; el
grupo añade una prueba que verifica ese comportamiento.

Sobre la versión `v4`, el grupo implementa una operación acotada de consulta o
modificación de tareas. Incluye controlador, servicio, repositorio JPA, DTO cuando
corresponda y prueba automatizada. La operación debe devolver respuestas HTTP
coherentes e incluir el caso de recurso inexistente. No se pide todavía una
migración versionada ni OpenAPI.

## Evidencias que deben quedar en este repositorio

- Código del slice y prueba(s) que lo verifican.
- `aprendizaje.md`, con las decisiones y responsabilidades de las capas.
- `equipo.md`, con integrantes, cuentas de GitHub y contribuciones.
- `declaracion-uso-ia.md`, cumplimentada tanto si se utilizó IA como si no.
- Historial de commits y ejecución reproducible de `mvn test`.

No entregues capturas ni documentos por separado en Moodle; conserva la evidencia
en los ficheros y el historial de este repositorio.

## Recursos y criterios

- `requests.http`: peticiones de ejemplo para las etapas de la API.
- `aprendizaje.md`: plantilla de reflexión del grupo.
- `equipo.md`: plantilla de integrantes y contribuciones.
- `declaracion-uso-ia.md`: declaración para completar.
- `rubrica.md` y `ra-ce.md`: criterios y evidencias de evaluación.
