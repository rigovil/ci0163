
  

## Resumen de los temas estudiados

 El **análisis de flujos de datos** nace de la necesidad de estudiar y procesar datos mientras estos están cambiando constantemente con el fin de tomar deceisiones oportunas. Se caracterizan por ser datos de alto volumen y con alta volatilidad en el tiempo.
 El procesamiento de flujos de datos se da en tiempo real, no hay tiempo para almacenarlos y esto produce que no se pueda entrenar un modelo de aprendizaje automático por el tiempo que tarda, por lo que supone un cambio de paradigma.
 La cardinalidad de los datos se caracteriza por no tener fronteras, es decir, no existe un incio o un fin en los registros. La constitución de los datos son flujos que fluyen en el tiempo.
 El análisis de estos flujos produce resultados constantemente, su desempeño es de baja latencia, se procesan los datos en el momento y pueden provenir de transacciones, eventos en directo, colas de mensajes, etc.
Existe un concepto denominado *time lag*, el cual es el retraso que existe mientras un dato es capaz de ser procesado. Por esto se definen dos tiempos los cuales corresponde al tiempo de procesamiento y al tiempo real en el que van produciéndose datos nuevos.
Los datos en flujos suelen no estar ordenados lo que hace difícil analizarlos aún en contexto, por lo que existen cuatro enfoques para analizar estos datos:

**I. Time agnostic**: en este enfoque, el tiempo es irrelevante para el análisis pues se utiliza un elemento de filtrado.

**II. Approximation**: transforman los datos en algo similiar pero que conserve ciertas similitudes.

**III. Windowing**: toma el flujo de datos y divide en partes, las cuales conservan ciertas características del momento en el que fueron divididas.
**IIIa. Windowing by processing time**: agrupa los datos en un buffer durante un tiempo determinado, cada grupo creado es analizado posteriormente.
**IIIb. Windowing by event time**: los grupos creados reflejan el tiempo del evento y no de procesamineto. El tamaño del grupo es variables, por lo que el tiempo de procesamiento varía de un grupo a otro.

**IV. Tumbling window**: tipo de agrupamiento que se dispara cuando la ventana creada esté llena.

Los **filtros** son un tipo de selección de ventanas, que aceptan datos del flujo que cumplan cierta propiedad y descartar las que no lo cumplen, esto es útil cuando hay muchos datos y no hay suficiente memoria.
El filtro *bloom* consiste en un arreglo de n bits iniciados en 0, algunas funciones hash y un conjunto de valores. El filtro deja pasar datos del flujo donde los valores pertenzcan al conjunto y rechaza el resto.

## Comentarios

Considero que este paradigma de análisis de datos en tiempo real ha venido a incrementar y ayudar al desarrollo de dispositivos que pertenezcan al contexto de IoT. Las personas soms una fuente continua de datos y todos los artefactos que nos rodean pueden aprender de nosotros mismos para facilitarnos en las tareas del día a día.

  

## Dudas

No tengo dudas respecto a la materia.
  

## Posible uso como profesional y problemas a resolver
Implementación de artefactos IoT que analicen datos producidos por las personas o las acciones que realicen. Pueden ser datos biométricos, de posición geográfica, etc.