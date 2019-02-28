# E10 - Random Forest Performance Review

Read and comment the paper *Do we Need Hundreds of Classifiers to Solve Real World Classification Problems?*

### Reference:
http://jmlr.org/papers/volume15/delgado14a/delgado14a.pdf

El artículo ‘Do we Need Hundreds of Classifiers to Solve Real World Classification Problems?’ detalla la evaluación de desempeño efectuada sobre múltiples algoritmos de clasificación de diferentes familias y con diferentes características, en busca de determinar si existe algún algoritmo con tendencia a generar mejores resultados, específicamente enfocándose en la exactitud en el proceso de clasificación.

Con el fin de generar el mayor número de pruebas eficaces, el experimento consolidó una base inicial de 165 data sets usualmente utilizados para evaluar tareas de clasificación. Múltiples datasets fueron eliminados luego de un análisis previo, por razones como tamaño, disponibilidad, entre otras. Finalmente, la base de datasets sobre la cual se aplicaron los algoritmos quedó compuesta por 112 data sets. Un factor a rescatar de la base de data sets tiene que ver con que no se realizó ningún tipo de pre-adecuación de la información, para evitar que algún cambio favoreciera el rendimiento de algún algoritmo.

Para la prueba se utilizaron 179 algoritmos de clasificación implementados en C/C++, Matlab, R y Weka. Dentro de las principales familias de algoritmos utilizados se encuentran los SVM (Support Vector Machine), Random Forest, redes neuronales, árboles de decisión, boosting, bagging, entre otras.  

La metodología aplicada en el estudio consistió en la aplicación de cada uno de los 179 algoritmos de clasificación, a cada uno de los 112 data sets consolidados en la base. De esta manera, evaluando el rendimiento de cada algoritmo con cada data set, se llegó a conclusiones claras de la aplicación de estos algoritmos. Adicionalmente, para cada prueba se generaron sets de entrenamiento y prueba.

Los resultados del estudio evidencian que el algoritmo con mejor rendimiento fue el parRF_t (parallel random forest implemented in R using RandomForest and caret packages), con una exactitud promedio del 82.0% (+-16.3). También fue el algoritmo mejor clasificado por la prueba de Friedman. Los siguientes algoritmos clasificados en ambos ítems también están relacionados con la familia Random Forest, lo que permite concluir que esta familia, presenta en general muy buenos rendimientos en los modelos de clasificación de todo tipo. Aunque esta conclusión no es nueva, sí llama la atención que algoritmos mucho más recientes y sofisticados, siguen estando por debajo de los Random Forest, teniendo en cuenta que cada algoritmo brinda otro tipo de beneficios.
