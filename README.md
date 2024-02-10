# Segmentación de pie

Librerías utilizadas: `Pandas`, `Numpy`, `Matplotlib`, `Seaborn` y `Scikit-Learn`


El conjunto de datos de Segmentación de Piel está construido sobre el espacio de color B, G, R. El conjunto de datos de Piel y No Piel se genera utilizando texturas de piel de imágenes faciales de personas de diversas edades, géneros y razas.

El conjunto de datos de piel se recopila mediante el muestreo aleatorio de valores B, G, R de imágenes faciales de varios grupos de edad (jóvenes, adultos y ancianos), grupos étnicos (blancos, negros y asiáticos) y géneros obtenidos de la base de datos FERET y la base de datos PAL. El tamaño total de la muestra de aprendizaje es de 245057; de los cuales 50859 son muestras de piel y 194198 son muestras de no piel.  

Este conjunto de datos tiene una dimensión de 245057 * 4, donde las primeras tres columnas son valores de B, G, R (características x1, x2 y x3) y la cuarta columna es de las etiquetas de clase (variable de decisión y).

https://archive.ics.uci.edu/dataset/229/skin+segmentation

El propósito principal de este proyecto es emplear la regresión logística para clasificar las muestras y distinguir si estas corresponden a muestras auténticas de piel o a muestras de otra naturaleza. Para el entrenamiento del modelo, se empleó la validación cruzada con diez pliegues y la validación mediante muestreo aleatorio. Las métricas seleccionadas para evaluar el rendimiento del modelo fueron el accuracy, sensibilidad, especificidad, precisión y el F1-score.

Para correr el repositorio de forma local se debe crear un entorno virtual con el siguiente comando:

    Python3 -m venv nombre_entorno_virtual

Se debe activar el entorno virtual e instalar todas las librerías especificadas en el archivo “requirements.txt” con el siguiente comando:

    pip install -r requirements.txt
