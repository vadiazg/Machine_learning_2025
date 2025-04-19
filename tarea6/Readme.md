# Desarrollo de algoritmo de KNN

Predecir la variable numérica Horas de estudio por semana normalizadas, determinar el error para cada k y elegir el mejor k.

Agregar nuevas variables que puedan mejorar el rendimiento


# 1. Importar librerías necesarias

*Dividir los datos en entrenamiento y prueba

*Crear un modelo de regresión logística

*Evaluar el modelo con una métrica especial para datos desbalanceados (precisión balanceada)

# 2. Preparar los datos

🔹 X es el conjunto de características (inputs)

🔹 y es la variable a predecir, en este caso la categoría de la flor (Category)

# 3. Dividir en entrenamiento y prueba

🔹 Dividir los datos en 70% para entrenar el modelo y 30% para probarlo.

🔹 random_state=42 asegura que siempre te dé la misma división (por reproducibilidad).

# 4. Entrenar el modelo

🔹 Crear un modelo de regresión logística.

🔹 max_iter=1000 indica que el modelo puede hacer hasta 1000 iteraciones para aprender correctamente.

🔹 Luego, entrenas el modelo con los datos de entrenamiento.

# 5. Hacer predicciones

🔹 Usar el modelo entrenado para predecir las categorías de las flores del conjunto de prueba.

# 6. Evaluar el modelo

🔹 Se muestran cuántas flores hay de cada tipo en el conjunto de prueba.

🔹 Esto ayuda a ver si hay clases desbalanceadas (por ejemplo, muchas setosa y pocas virginica).

# 7. Calcular precisión balanceada

🔹 La precisión balanceada evalúa qué tan bien predices cada clase, sin importar si hay muchas o pocas muestras de esa clase.

🔹 Es útil cuando hay desequilibrio en las clases.