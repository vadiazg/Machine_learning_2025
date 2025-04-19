# Desarrollo de la tarea de reglas de asociación.


# 1. Aplicación de Algoritmos

Apriori
Este algoritmo genera combinaciones de productos frecuentes en pasos sucesivos. Solo combina productos si sus subconjuntos también son frecuentes, lo cual reduce la complejidad. Se usa cuando se quiere controlar el crecimiento de combinaciones, pero puede ser más lento con grandes volúmenes de datos.

FP-Growth
A diferencia de Apriori, no genera combinaciones repetidas. En su lugar, construye un árbol llamado FP-tree, lo que mejora mucho el rendimiento para grandes cantidades de datos. Es más rápido y eficiente en muchos casos.

# 2. Generación de Reglas de Asociación

Ambos algoritmos generan reglas como:

pan → mantequilla (confianza = 0.75, lift = 1.2)

Estas reglas indican la probabilidad de que se compre un producto si se compró otro.

Las métricas que usamos son:

-Soporte: frecuencia del conjunto en todas las transacciones.

-Confianza: cuántas veces ocurre B cuando ocurre A.

-Lift: mide si la ocurrencia conjunta es mayor a lo esperado por azar (lift > 1 es interesante).

# 3. Visualización y Comparación

Se hace una gráfica donde se comparan cuántos conjuntos frecuentes detecta cada algoritmo. Esto sirve para ver cuál es más efectivo o qué tan diferentes son en resultados.

# 4.Conclusión

Ambos algoritmos encuentran patrones útiles en los datos, pero:

*Apriori es más simple pero más lento en bases grandes.

*FP-Growth es más rápido y eficiente en muchos casos.

*Usar Polars permite integrar un enfoque moderno de procesamiento de datos.

Esta práctica demuestra cómo aplicar algoritmos clásicos de minería de datos a un caso realista de análisis de comportamiento del cliente.