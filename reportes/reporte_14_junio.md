## Resumen de los temas estudiados
**Clustering** es una técnica de algoritmo no supervisado para dividir un dataset en segmentos o grupos. La idea es que estos grupos estén compuestos por datos entre los cuales se comparte alguna naturaleza sobre ellos, de forma que la agrupación tenga un significado y permita hacer análisis, comparaciones y toma de decisiones. 
Esta técnica de segmentación necesita de una métrica de similitud, es decir, establecer bajo qué parámetros y en qué nivel un dato se parece a otro, los atributos categóricos deben estar codificados y se debe transformar los atributos numéricos. También, se debe tener claro cuántos clusters se están buscando, esto depende de la naturaleza de los datos.
Existen algunos métodos de segmentación: **particionamiento**: se basa en mediciones de distancia, es útil cuando no hay muchos datos, los segmentos son excluyentes entre sí. Hay varios algoritmos como *k-means*, *k-modes*, *k-medois*, etc. **Jerárquicos**: se refiere a descomposiciones jerárquicas, algunos algoritmos son *birch* y *chameleon*. De **densidad**: los clusters son densos en el espacio y su separación de otros clusters está dada por regiones de baja densidad. Aquí están los algoritmos *dbscan*, *optics* y *denclue*. Los de **rejilla**: se procesan rápidamente y no depende del número de puntos, algunos algoritmos son *sting* y *clique*.
Algunos otros conceptos son, **centroide**: se refiere a la media de todos los puntos en un cluster, puede no necesariamente ser un punto que exista. **Prototipo**, se refiere al objeto que representa al cluster y lo diferencia del prototipo de otro cluster.

Características de algunos algoritmos de clustering:
1. K-Means: recibe como entrada un número *k* clusters, el algoritmo inicialmente elige *k* centroides y se repite hasta que estos no cambien. Este número *k* es arbitrario. No se garantiza conseguir el número adecuado de clusters, además se parte que los clusters tienen el mismo tamaño. 

2. DBSCAN: forma clusters de regiones muy densas, estos clusters están separados por regiones donde hay muy poca densidad de puntos. Se puede visualizar como grupos en el espacio donde no hay nada alrededor y todo los puntos están dentro de cada grupo. Tiene dos parámetros, *min_samples*, para indicar el tamaño mínimo deseado para los clusters. Y *eps*, el cual es la distancia máxima entre dos puntos, donde los valores pequeños suelen ser más útiles, aunque puede dejar por fuera de los clusters a algunos puntos.

La naturaleza de los datos puede afectar la técnica de clustering, por ejemplo: si el dataset es muy grande, si hay mucha dispersión de los datos, la presencia de outliers y una gran escala en los datos.
Algunas propiedades para evaluar un cluster son: homogeneidad, completitud, *rag bag* y la preservación de clusters pequeños. Matemáticamente se puede utilizar la métrica de *silhouette*, que es para cada punto y utiliza la distancia de un punto con su cluster y con el centro del cluster más cercano.

## Comentarios

Como se explicó, la técnica de clustering viene a apoyar el proceso natural de las personas de clasificar todo lo que lo rodea en grupos o categorías, algo que suele hacerse a través de la vista, pero que con ayuda de la capacidad computacional, los datos, objetos o, en general, cualquier cosa pueden agruparse de formas en las que quizás a las personas no se les facilita a través de los sentidos o que intuitivamente no está a simple vista. Lo importante es conocer la naturaleza de los datos para poder escoger el algoritmo más adecuado de segmentación, así como de importante es visualizar de qué manera los datos están distribuidos en el espacio, preferiblemente en dos o tres dimensiones para que la comprensión sea más sencilla. 

## Dudas
Cuando los datos se visualizan en más de tres dimensiones, ¿qué formas o técnicas hay para saber de antemano cuántos clusters podrían haber? Por ejempl, tal vez en un plano cartesiano es fácil visualizarlo, pero cuando hay más de tres dimensiones esto se dificulta.

¿Los datos, vistos como puntos en un espacio, que compartan ciertas características con otros datos, siempre van a estar naturalmente agrupados? O, ¿podría pasar que puntos similares entre sí estén distribuidos por todo el espacio?

¿Se puede hacer clustering con imágenes?

## Posible uso como profesional y problemas a resolver

Algunas que se han mencionado en clase, como clasificar clientes de bancos o cualquier entidad. Clasificar especies de animales o plantas a partir de ciertas características. 