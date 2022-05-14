## Resumen de los temas estudiados
Existen los denominados algoritmos de *machine learning*, los cuales se dicen que aprenden o se ajustan a un conjunto de datos específico para producir una salida, el cual se denomina **modelo** y a partir del cual se pueden hacer predicciones. Estos algoritmos pueden ser implementados en varios lenguajes de programación y abarcan tanto algoritmos de clasificación, regresión y segmentación; de cada uno varía la eficiencia, complejidad y efectividad.

Las técnicas de **clasificación** se utilizan para predecir si un dato pertenece a una clase. Los algoritmos de **regresión** sirven para predecir un valor numérico. Estas técnicas producen un modelo que debe ser entrenado/ajustado a partir de un conjunto de datos conocido. Esta etapa puede producir sesgos o varianza, los cuales son errores presentes en el modelo y conllevan a un subajuste y sobreajuste.

Un ejemplo de algoritmo útil para clasificación y regresión son los **árboles de decisión**. Estos se construyen a partir de los datos, seleccionan los atributos más importantes los cuales influyen en mayor medida sobre el valor de una variable que es la que se quiere predecir. De esta forma, cada nivel del árbol crea un flujo que es particionado por valores de los atributos seleccionados y que permiten al modelo hacer una predicción para un dato de entrada. También está expuesto a errores de subajuste y sobreajustado, los cuales ocurren por la presencia de ruido y por un ajuste muy cercano al conjunto de datos, respectivamente.

Un árbol de decisión puede agruparse con otros árboles y así crear lo que se conoce como *random forests*. Estos son un conjunto de árboles, que pueden llegar a ser diferentes entre sí, para que produzcan todos una predicción a partir de un mismo dato de entrada, al final, se pondera el resultado de todos los árboles para realizar una predicción final categórica o numérica. Se puede controlar el número de árboles, las muestras del conjunto de datos, las especificaciones de un *split*, etc.

Otra configuración son los *ensembles*, los cuales son árboles dispuestos de forma serial, de manera que un árbol corrija el error del árbol anterior, suelen ser más rápidos y más efectivos que un *random forest*.

## Comentarios

Considero que la técnica de árboles de decisión es una de las más intuitivas que he visto hasta ahora, pues se trata de clasificar un dato haciéndose preguntas de si/no (como un *split*) hasta llegar a una conclusión, y creo que inconscientemente una persona está acostumbrada a tomar decisiones de esta forma, siempre que sean decisiones racionales o pensadas. Me parece interesante la forma en que se crean y se van descubriendo nuevos algoritmos para clasificación o regresión y cómo con un conjunto de datos se pueden llegar a hacer predicciones medianamente decentes que pueden colaborar en muchas otras áreas más allá de la computación. 

## Dudas

En algunos tutoriales de las prácticas se menciona que los random forest son inmunes al overfitting, me queda la duda de por qué esto es así y por qué si esto sucede entonces no son la técnica más elegida para realizar modelos predictivos o por qué no tienen ventaja frente a otros algoritmos, en ese caso pensaría que el overfitting no es el mayor de los problemas y que tal vez existen otros que afectan más a un modelo.

## Posible uso como profesional y problemas a resolver

Cualquier trabajo que implique tomar decisiones a partir de datos se puede automatizar o apoyar en algoritmos de machine learning, desde predicción de condiciones climáticas hasta para elaborar un registro crediticio en un banco que permita decidir si es viable prestar dinero o no a un cliente.

