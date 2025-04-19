
# TkNN-Predict-the-numeric-variable-Study_Hours_per_Week_normalized-determine-the-error


## Desarrollo del segundo reto de Kaggle

* Predecir la variable numérica Horas de estudio por semana normalizadas, determinar el error para cada k y elegir el mejor k.

* Agregar nuevas variables que puedan mejorar el rendimiento.

_Resumen Rápido_

Se esta utilizando el algoritmo KNN para predecir la clase de las flores.

Se evaluo la precisión del modelo con un k=3 y calculo la precisión balanceada para ese valor de k.

Luego, se explora cómo cambia la precisión con diferentes valores de k (de 1 a 20) y graficaste esos resultados para elegir el mejor valor de k. texto en cursiva

_Este código es una técnica de ingeniería de características, que consiste en crear nuevas variables útiles y transformar otras para que los modelos de machine learning puedan aprender mejor y tener mejor rendimiento._

Aquí se esta calculando el área del sépalo y del pétalo, multiplicando largo por ancho. Estas áreas pueden contener más información que las dimensiones por separado y podrían mejorar la precisión del modelo.

Luego se aplico el logaritmo natural a las columnas SepalLength y PetalLength para:

*Suavizar valores extremos (outliers),

*Hacer que la distribución de los datos sea más simétrica,

*Mejorar el rendimiento de algunos modelos.

*Se sumas 1 para evitar errores con valores cero (log(0) no existe).