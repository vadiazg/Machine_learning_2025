
# Desarrollo de la tarea del problema del viajero con algoritmo Hopfield con el problema dado en clase y el otro problema que es con el algoritmo PCA visualizando en 2D una base de datos de MNIST


# PASO 1: Definimos el número de ciudades y la matriz de distancias

Cada ciudad tiene una coordenada, y la matriz distancias[i][j] nos dice qué tan lejos está la ciudad i de la j. ¡Esto será clave para minimizar la ruta total!

# PASO 2: Parámetros de la red Hopfield
Queremos un sistema que diga:


“No repitas ciudad”
“No pongas 2 ciudades en el mismo lugar”
“Escoge caminos cortos” Y eso lo hacen los pesos A, B, C, y D

# PASO 3: Creamos la matriz de pesos W (interconexiones neuronales)

Estamos conectando todas las neuronas entre sí (menos consigo mismas) y agregando penalizaciones inteligentes con los pesos A, B y D .

# PASO 4: Vector de umbrales (theta)

Este sesgo ayuda a que las neuronas no se activen todas al tiempo. Ayuda a la estabilidad

# PASO 5: Actualización del estado (dinámica de la red)
La red evoluciona cambiando poco a poco los valores de las neuronas hasta llegar a un equilibrio. Eso se llama estado estable o de mínima energía.

# PASO 6: Evaluamos si el estado final es un recorrido válido
Este paso revisa si el resultado de la red cumple las reglas del TSP. Si no, volvemos a intentarlo con otra condición inicial.

# PASO 7: Visualizamos el recorrido
Aquí se grafican las ciudades como puntos y el camino en rojo. Si hay un recorrido válido, lo mostramos.