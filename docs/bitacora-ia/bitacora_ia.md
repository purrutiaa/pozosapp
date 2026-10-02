# Bitácora inicial de uso de IA

Esta bitácora registra usos reales de un agente de IA realizados durante la preparación del proyecto. El objetivo no es aceptar automáticamente las respuestas, sino dejar evidencia de cómo fueron revisadas y ajustadas por el equipo.

## Uso 1 - Revisión de requisitos del Avance 3

**Objetivo:** Identificar los archivos, carpetas y condiciones que debía cumplir el repositorio de GitHub para el Avance 3.

**Instrucción entregada:** Se adjuntaron las instrucciones oficiales del Avance 3 y se solicitó revisar qué debía prepararse para la entrega.

**Respuesta obtenida:** La IA organizó los requisitos en una lista de verificación: repositorio con ramas `main` y `dev`, estructura mínima de carpetas, README principal, entregables de la Unidad 1, bitácora de IA, archivo de estructura de datos, `.gitignore` y `.env.example`.

**Qué se aceptó y qué se corrigió:** Se aceptó la estructura general porque coincidía con las instrucciones. Se mantuvo explícitamente que en esta etapa no se debe inventar una aplicación ejecutable ni implementar todavía la base de datos. Además, se verificó que el trabajo debe pasar desde `dev` a `main` mediante pull request y que deben existir commits de más de un integrante.

**Cómo se verificó:** Se comparó punto por punto la propuesta con el documento oficial del Avance 3 antes de preparar los archivos.

---

## Uso 2 - Diseño preliminar de la estructura de datos

**Objetivo:** Proponer las entidades principales de la base de datos a partir del caso de uso ya definido por el equipo.

**Instrucción entregada:** Se adjuntó el archivo del Avance 2 para que la propuesta de datos se construyera desde el caso de uso y no desde supuestos externos al proyecto.

**Respuesta obtenida:** La IA propuso como entidades principales `USUARIO`, `POZO`, `DATO_MONITOREO`, `EVENTO`, `EVIDENCIA`, `GESTION` y `TICKET`, además de relaciones entre ellas.

**Qué se aceptó y qué se corrigió:** Se aceptaron las entidades porque representan conceptos que aparecen en el caso de uso. Se decidió usar una sola entidad `EVENTO` con el campo `tipo_anomalia`, en vez de mantener `EVENTO` y `ANOMALIA` como tablas separadas, para evitar duplicar información. También se mantuvo `GESTION` separada de `EVENTO` para conservar un historial de acciones realizadas. El equipo aclaró además que las páginas 1 y 2 del archivo corresponden al Avance 1 y las páginas restantes al Avance 2.

**Cómo se verificó:** Se revisó que cada entidad tuviera relación directa con el flujo del caso de uso: consultar eventos, revisar el pozo y su evidencia, validar la condición, registrar la gestión y asociar un ticket cuando corresponda.

---

## Uso 3 - Preparación de archivos del repositorio

**Objetivo:** Dejar una primera versión ordenada de los archivos necesarios para subir el Avance 3 a GitHub.

**Instrucción entregada:** Se solicitó preparar los archivos necesarios usando como base las instrucciones del Avance 3 y los avances ya desarrollados por el Equipo 7.

**Respuesta obtenida:** Se generaron el README principal, el README de `src/`, la bitácora de IA, el archivo `estructura_datos.md`, `.gitignore` y `.env.example`.

**Qué se aceptó y qué se corrigió:** Se mantuvo una estructura mínima y fácil de explicar, evitando agregar archivos que no fueran necesarios. No se incorporaron claves reales ni credenciales. La estructura de datos quedó declarada como preliminar, ya que la implementación de la base de datos corresponde a una etapa posterior.

**Cómo se verificó:** Se contrastó la carpeta final con los requisitos indicados en las instrucciones del Avance 3 y se revisó que todas las subcarpetas tuvieran contenido versionable.
