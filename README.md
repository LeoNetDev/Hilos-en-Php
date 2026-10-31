PROCESAMIENTO DE DOCUMENTOS CON HILOS

Materia: Sistemas Operativos

Integrantes
- Mateo
- Lucas
- Juan
- Valentin

Descripcion

En esta practica se realizo un programa en Python para procesar 24 documentos utilizando cuatro hilos de ejecucion. Cada hilo representa a un trabajador encargado de realizar diferentes tareas.

Objetivo

Comprender como funcionan los hilos y como se pueden repartir los trabajos utilizando una cola y mecanismos de sincronizacion.

Herramientas utilizadas

- Python
- Google Colab
- threading
- queue
- time
- random

Desarrollo

El programa realiza las siguientes actividades:

1. Crea una cola con 24 documentos.
2. Genera cuatro hilos con los nombres de los integrantes.
3. Cada trabajador procesa seis documentos.
4. Registra los documentos y su tamaño.
5. Utiliza Lock para proteger los resultados compartidos.
6. Utiliza join para esperar que todos los hilos terminen.
7. Muestra un resumen con los resultados obtenidos.

Resultados

Se realizaron cuatro ejecuciones para comprobar el funcionamiento del programa.

En las pruebas se verifico lo siguiente:

- Se procesaron los 24 documentos.
- No existieron documentos repetidos.
- No quedaron documentos pendientes.
- Cada trabajador proceso seis documentos.
- Los cuatro hilos finalizaron correctamente.

Interpretacion

En cada ejecucion cambio la distribucion de los documentos entre los trabajadores. Esto se debe a que los hilos trabajan de forma concurrente y pueden terminar sus tareas en diferentes momentos.

Tambien se observaron pequeñas diferencias en los tiempos de procesamiento de cada prueba.

Preguntas de la practica

1. ¿Por que queue.Queue es apropiada para compartir trabajos?**

Porque permite organizar los 24 documentos en una cola y repartirlos entre los cuatro trabajadores. Cada uno toma un documento diferente y asi evitamos que se repita el trabajo.

2. ¿Que protege Lock y que pasaria si se actualizara el resumen sin el?**

Lock protege los resultados que comparten los trabajadores. Sin el podrian ocurrir errores cuando varios hilos intenten guardar sus resultados al mismo tiempo.

3. ¿Que cambiarias si cada documento tuviera que guardarse en un archivo real?**

Agregaria instrucciones para abrir y guardar cada documento en la computadora. Tambien controlaria que dos trabajadores no modifiquen el mismo archivo al mismo tiempo.

 Evidencias

Se adjunta un archivo PDF con las cuatro capturas de las ejecuciones y sus respectivas interpretaciones.
