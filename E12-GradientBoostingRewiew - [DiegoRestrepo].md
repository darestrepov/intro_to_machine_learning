# E12 - Gradient Boosting Review

El gradient boosting Classifier y el XGB Classifier hacen parte de los múltiples algoritmos de la familia boosting, que se caracteriza por la repetición iterada de aplicación de modelos adaptando cada repetición para atacar la mayor cantidad de vulnerabilidades del algoritmo inmediatamente anterior. Esto es posible gracias a una técnica de redefinición del peso de acuerdo a la exactitud de la predicción en la itración.

(1) [ Gradient Boosting Classifier ](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html)
El gradient boosting está basado en tres componentes principals:

-	Loss function
Depende del problema que se busque resolver y debe ser diferenciable, de manera que su versión genérica pueda usarse en todas las iteraciones.
-	Weak learner
Se utilizan árboles de decisión para aprender de las debilidades del modelo, que son escogidos a partir de la escogencia de puntos óptimos de Split basados en puntuaciones como Gini. 
-	Modelo aditivo
Los árboles se van añadiendo uno a la vez. Se utiliza entonces un proceso de gradient descent para minimizar el error tras la adición de cada árbol. Después de calcular el error, se hace una redefinición de los pesos, y esta optimización permite al algoritmo ir reduciendo el error entre una iteración y la siguiente.

(2) [ XGB Classifier ](https://xgboost.readthedocs.io/en/latest/python/python_intro.html)

eXtreme Gradient Boosting es una metodología asociada a boosting, muy usada para algoritmos de predicción, que está orientada a la optimización de los recursos computacionales para la ejecución de múltiples árboles. Dentro de los parámetros que el algoritmo puede modificar a nivel computacional para la ejecución del modelo están la paralelización de recursos (cores), optimización de la memoria caché, el uso de dispositivos externos (clusters), entre otros.

Se diferencia del GBM principalmente en la aplicación del modelo, pues XGB usa un modelo más formal para el control de sobredimensionamiento derivando en un mejor desempeño al algoritmo.

