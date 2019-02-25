# E8 - Ensemble Trees Overview

Write at least 300 words explaining why ensemble is a succesful strategy in machine learning.


Los métodos de combinación de algoritmos de Machine Learning son meta-algoritmos que combinan técnicas de análisis predictivo para construir modelos más robustos reduciendo varianza, bias o mejorando las predicciones.

Bagging:

Algoritmo utilizado para incrementar los niveles de precisión de un modelo de Machine Learning, si se compara con modelos como árboles simples de decisión. También es muy útil en pro de reducir la varianza de la aplicación de un modelo para el análisis de un caso de uso. Este tipo de modelos se basa en el procesamiento de múltiples muestras aleatorias con reemplazo, por lo que las métricas de aplicación del modelo son el resultado de promediar la salida de todos los modelos de todas las muestras. Vale la pena aclarar que para el caso de árboles de decisión de clasificación se realiza un sistema de conteo de la salida con los resultados de las muestras analizadas.

Boosting:

Algoritmo utilizado para reducir la varianza de un modelo de aprendizaje automático. Su aplicación se basa en la combinación de múltiples modelos relativamente débiles, que balancean el peso de las variables de predicción a medida que se evalúan modelos, con el fin de obtener un análisis más robusto para las predicciones. El algoritmo más comúnmente usado para aplicación de Boosting es el AdaBoost.

Stacking:

Algoritmo utilizado para obtener mejoras considerables en la precisión del modelo. El algoritmo se basa en el entrenamiento de múltiples modelos usados como base, con el mismo set de entrenamiento, y la predicción de cada una de las salidas de dichos modelos. Posteriormente, el meta-algoritmo se entrena con un dataset basado en las múltiples salidas de los modelos base.

Random Forest:

Metodología utilizada para mejorar la varianza de un modelo predictivo a pesar un incremento significativo en el Bias. Este modelo se basa en la aleatoriedad de los factores que hacen parte de los modelos. Esto significa que cada modelo, además de aplicarse una aleatoriedad en la muestra a la que se aplica cada modelo base, también se seleccionan diferentes variables para cada modelo. En algunos casos incluso se incluye un nivel de aleatoriedad a los umbrales de partición del dataset entre train y test.


