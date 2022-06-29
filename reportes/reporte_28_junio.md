
## Resumen de los temas estudiados

**Análisis de asociación**  consiste en técnicas o métodos que descubren asociaciones entre atributos de datos que tienden a aparecer o a ocurrir de forma conjunta. Los datos son transaccionales el cual se identifica por un itemset, que corresponde a un producto, elemento, etc. A la cantidad de veces que aparece un itemset en una transacción se le denomina *frecuencia*.

Existen dos propiedades las cuales son **soporte**: usado para distinguir una regla de un evento aleatorio y **confianza**: medida de precisión que aumenta o disminuye la probabilidad de que un elemento aparezca en transacciones que contiene a otro elemento.

Para generar reglas se necesita encontrar los itemsets frecuentes y a partir de ellos, generar las reglas de asociación que satisfagan las dos propiedades anteriores. La cantidad de reglas puede ser exponencial debido a que el espacio de búsqueda puede ser muy grande. Pero esto se puede simplificar con el **principio a priori**, que indica que un subconjunto que contiene a un itemset frecuente también es frecuente, si un itemset no lo es, entonces sus subconjunto no son frecuentes.

Hay que considerar la forma en la que se puede presentar un atributo: binarios simétricos y asimétricos, categóricos, continuos, multidimensionales, multinivel y secuenciales.

Algunas reglas no son útiles, pues reflejan asociaciones lógicas, que no obedecen a una razón clara o que no posee valor real. Para esto existe una medida denominada *lift*, que le asocia un valor de utilidad a una regla.

Estas técnicas permiten encontrar patrones en sectores de datos (áreas locales).

Las **series de tiempo** es cuando una variable de respuesta es dependiente del tiempo, de forma que se puedan encontrar patrones de pasado para hacer predicciones del futuro. Formalmente, son una secuencia de valores que representan a esa variable. Pueden ser discretas o continuas.

Algunos componentes son la **tendencia**, que describe el comportamiento. La **temporalidad**, se refiere  a las fluctuaciones en la serie y **ruido**, que son fluctuaciones irregulares. La descomposición de una serie se refiere a identificar estos tres elementos, de manera que se pueda analizar la estructura de la serie y hacer predicciones futuras.

Las fluctuaciones irregulares se pueden eliminar mediante la técnica de *moving average*, aunque también puede ayudar a quitar la temporalidad y aproximar la tendencia.

## Comentarios

Las técnicas de asociación me parecieron interesantes porque le encuentro relación a las cadenas de markov que se vio en un curso anterior, en ese momento no entendía cómo se calculaban los valores de probabilidad para que se diera un evento A dado B, etc.

Las series de tiempo también me parecieron interesantes porque muchos datos están directamente relacionados con el tiempo, además de su posible uso o presencia en muchos dispositivos que utilicen sensores.
  

## Dudas
  
  En una serie de tiempo, ¿hay alguna forma de contemplar, en una predicción a futuro, eventos muy inusuales? Por ejemplo, que la pandemia fuera a afectar los comportamientos de los usuarios de X tienda antes de que siquiera se tuviera la noción de que empezara una pandemia.

## Posible uso como profesional y problemas a resolver

Tanto las series de tiempo como las técnicas de análisis de asociación se pueden utilizar para modelar el comportamiento de las personas, de un sistema, etc. lo cual es útil para empresas de mercadeo, de inversiones o para simulaciones de un sistema.