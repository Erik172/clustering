# Clustering: k-means

- [Introducción](#introducción)
- [Implementación desde cero](#implementación)

## Introducción
K-means es un algoritmo de clustering, también conocido como agrupamiento, que se utiliza para clasificar un conjunto de datos en grupos o clusters. El objetivo del algoritmo es encontrar un conjunto de k centroides, donde k es el número de clusters deseados, y asignar cada punto de datos al centroide más cercano.

El proceso de k-means se realiza en varias iteraciones. En la primera iteración, se seleccionan k puntos aleatorios como centroides. Luego, se calcula la distancia entre cada punto de datos y cada centroide, y se asigna cada punto al centroide más cercano. Una vez que todos los puntos se han asignado a un centroide, se recalcula la posición de los centroides como la media de los puntos que pertenecen a cada centroide. Este proceso se repite hasta que los centroides dejen de moverse o se alcance un número máximo de iteraciones.

El algoritmo k-means es ampliamente utilizado en aplicaciones de minería de datos, aprendizaje automático y análisis de datos, como la segmentación de clientes, la clasificación de imágenes y la agrupación de noticias. Es un algoritmo rápido y eficiente, pero puede ser sensible a la inicialización aleatoria de los centroides y puede no funcionar bien con datos de alta dimensionalidad.

## Implementación

Notebook: [k-means_from_scratch.ipynb](k-means_from_scratch.ipynb)

K-means es un algoritmo de clustering que se puede implementar desde cero sin usar la biblioteca sklearn. El proceso se realiza en varias iteraciones y consta de los siguientes pasos:

1. Seleccionar k puntos aleatorios como centroides iniciales.
1. Calcular la distancia entre cada punto de datos y cada centroide y asignar cada punto al centroide más cercano.
1. Calcular la posición de los nuevos centroides como la media de los puntos que pertenecen a cada centroide.
1. Repetir los pasos 2 y 3 hasta que los centroides dejen de moverse o se alcance un número máximo de iteraciones.

Para implementar el algoritmo desde cero, se pueden seguir los siguientes pasos:

1. Definir el número de clusters k y los datos de entrada.
1. Seleccionar k puntos aleatorios como centroides iniciales.
1. Crear una función para calcular la distancia entre cada punto de datos y cada centroide. Esto se puede hacer utilizando la fórmula de distancia euclidiana.
1. Crear una función para asignar cada punto al centroide más cercano utilizando la función de distancia definida anteriormente.
1. Crear una función para calcular la nueva posición de los centroides como la media de los puntos que pertenecen a cada centroide.
1. Repetir los pasos 4 y 5 hasta que los centroides dejen de moverse o se alcance un número máximo de iteraciones.

Es importante tener en cuenta que la inicialización aleatoria de los centroides puede afectar el rendimiento del algoritmo. Por lo tanto, es recomendable realizar varias ejecuciones con diferentes inicializaciones aleatorias y seleccionar el modelo con el menor error.