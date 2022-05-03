# Tarea 1
### Dataset: Movies Dataset 
##### Preguntas de investigación
- Año de estreno de películas/series con mejor puntaje.
- Año con mayor participación de votantes.
- Año con mejor promedio de rating. 

##### Problemas en los datos
- La columna de año muestra el intervalo en el que la película/serie estuvo activa.
- Hay una gran cantidad de registros que no contienen información del ingreso obtenido en comparación con los que sí lo tienen.
- La información de director y estrellas está contenida en una sola columna.

##### Propuestas de corrección
- Deshacer el intervalo y dejar solo el año en que la película o serie fue estrenada.
- Eliminar la columna que contiene la información de ingresos pues no se puede deducir y no aporta información relevante para lo que se quiere analizar.
- Crear una columna para el director y otra para las estrellas.

##### Atributos de importancia
Todas las consultas tienen relación con el año de estreno de la serie o película, por tanto es importante considerar esta variable. De igual forma se deben considerar las variables *rating* y *votes* porque están implicadas en el análisis que se quiere realizar.
##### Transformaciones en el dataset
Se quitaron espacios en blanco no deseados al inicio de muchas de las celdas de la mayoría de las columnas. De igual forma, los atributos *rating*, *votes* y *runTime* fueron convertidos a datos números en lugar de datos de texto. Se quitó las palabras *"Director/Directors"* y *"Stars"* de todas las celdas en sus respectivas columnas, los registros que no tuvieran un director se llenaron con *"Not found"*. Por último, se eliminó más de 3000 duplicados y los registros que tuvieran en blanco los atributos *votes* y *rating* pues no servirían para el análisis, no se puede deducir el dato y buscarlos individualmente no es viable por la enorme cantidad de búsquedas que habría que hacer.