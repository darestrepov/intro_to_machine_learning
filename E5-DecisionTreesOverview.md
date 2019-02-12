# E5 - Decision Trees Overview

Un árbol de decisión es una metodología asociada a inteligencia artificial, utilizada para el análisis estadístico y la toma de decisiones a partir de la evaluación de alguna métrica de referencia y la selección de una variable a evaluar y un límite para la decisión.  

Un árbol de decisión es una estructura de flujo de análisis, basada en nodos que denotan la prueba de un atributo. Son altamente usados para investigación de operaciones de cualquier tipo de proceso o negocio. Específicamente, se usan para análisis de decisión con miras a alcanzar un objetivo. 

A continuación se da una breve descripción de diferentes tipos de árboles de decisión:

-	ID3 (Iterative Dichotomiser 3): Este algoritmo está basado en la división de cada nodo en dos grupos de decisión, de manera que se va construyendo el árbol de decisión. En cada nivel, se evalua la entroía para llegar al atributo más dominante.   

-	C4.5 (successor of ID3): Se considera una evolución de del ID3 con la diferencia que no utiliza la ganancia como parámetro de evaluación, sino un ratio de la misma. Adicionalmente, transforma atributos continuos en nominales para maniputar datos continuos. Requiere gran uso de memoria.

-	CHAID (CHi-squared Automatic Interaction Detector): Este tipo de árbol es usado para resolver problemas de clasificación, apelando a la prueba chi cuadrada para determinar la mejor división a seguir en cada paso. Para resolver problemas de regresión, el algoritmo aplica pruebas F.

-	MARS: Extends decision trees to handle numerical data better.

-	CTree (Conditional Inference Trees): Este es un tipo de árboles de decisión no paramétricos orientado a modelos de regresión, aplicable a cualquier tipo de problema de regresión, incluyendo metodologías nominales, ordinales o numéricas, así como modelos de respuesta multivariada. 
