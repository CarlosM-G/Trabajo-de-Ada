# Trabajo-de-Ada

Autores: Carlos Muñoz Gomez y Jorge Sanchez Doctor.

En nuestro caso estamos compilando y ejecutando el código a través de terminal con los comandos:
  
  Compilacion:
    
    gnatmake <nombrearchivoejecutable>

  Ejecución:
  
    ./<nombrearchivoejecutable>


Aun falta meter tanto el documento de diseño como el bug_log:

  Documento de diseño (6–8 páginas, sin contar portada)
    El documento debe abordar:
    
    1. Arquitectura y diagrama de diseño. Incluir al menos un diagrama que muestre los com-
    ponentes del sistema (tareas, objetos protegidos), sus relaciones y los mecanismos de co-
    municación empleados entre ellos (rendezvous, llamadas a entries, etc.).
    
    2. Decisiones de diseño (mínimo 2). Para cada una, indicar las alternativas consideradas,
    cuál se eligió y por qué.
    
    3. Análisis de interbloqueo e inanición. Qué riesgos existen en el diseño y cómo se previe-
    nen.
    
    4. Diseño alternativo. Elegir un componente de la solución y explicar cómo sería la imple-
    mentación con el mecanismo opuesto (p. ej., si se usó un objeto protegido, cómo sería con
    una tarea). ¿Qué se ganaría? ¿Qué se perdería? ¿Qué bugs nuevos podrían aparecer?
    
    5. Resultados de los escenarios de estrés. Captura de salida relevante y análisis breve de
    cada escenario.
    
    6. Instrucciones de compilación y ejecución. Debe ser posible compilar y ejecutar el pro-
    grama siguiendo únicamente estas instrucciones, incluyendo cómo configurar los pará-
    metros para reproducir cada escenario de estrés.

  Diario de bugs de concurrencia (1–2 páginas)
    Incluir como parte de la entrega un fichero bug_log.pdf con una tabla de 3–5 entradas sobre
    bugs de concurrencia encontrados durante el desarrollo, siguiendo este formato. Cada entrada
    puede ser un bug real o un análisis de un bug que se esperaba encontrar y no se produjo (véase
    más abajo):
    
    Bug: Ejemplo deadlock.
    Síntoma: Se cuelga tras 10s.
    Causa raíz: Adquisicion circular.
    Descubrimiento:8 trenes, 2 plataformas. 
    Corrección: Orden fijo: tramo primero.
