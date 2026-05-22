## 📚ThreatFlow-ML
Clasificación Multiclase de Incidentes de Ciberseguridad con Machine Learning
ThreatFlow ML es un sistema de clasificación multiclase de incidentes de ciberseguridad basado en Machine Learning. El modelo utiliza características de tráfico de red del conjunto de datos UNSW-NB15 para predecir la categoría de ataque asociado a cada flujo de red.

El proyecto aborda un problema real de los equipos de ciberseguridad: la necesidad de clasificar grandes volúmenes de eventos y alertas de forma eficiente. Para ello, se desarrolló un pipeline completo de entrenamiento que incluye carga de datos, limpieza de la variable objetivo, tratamiento de valores faltantes, codificación de variables categóricas, escalado de variables numéricas, entrenamiento de modelos supervisados ​​y evaluación mediante métricas específicas para clasificación multiclase.

Se compararon modelos como Logistic Regression y Random Forest , seleccionando el mejor desempeño a partir de métricas como F1 Macro , especialmente relevantes en conjuntos de datos desequilibrados. Además, el sistema genera informes de clasificación, matriz de confusión y guarda el modelo entrenado para futuras predicciones.

## 📚Objetivo del proyecto

Desarrollar un modelo supervisado capaz de clasificar tráfico de red en múltiples categorías de ataque, aportando una base para soluciones de detección, priorización y análisis asistido de incidentes de ciberseguridad.

## 📚Problema que resuelve

En un entorno corporativo, los equipos de seguridad reciben grandes volúmenes de eventos provenientes de firewalls, endpoints, servidores, SIEM y herramientas de monitoreo. Muchos de estos eventos requieren clasificación, priorización y análisis.

## 📚Puntos destacados

Clasificación multiclase de incidentes de ciberseguridad
Pipeline completo de Machine Learning
Preprocesamiento automático de variables categóricas y numéricas
Comparación de modelos supervisados
Evaluación con métricas robustas para clases desbalanceadas
Visualización y guardado de matriz de confusión
Guardado del mejor modelo entrenado
Proyecto extensible hacia integración con SIEM, MITRE ATT&CK y agentes IA

## 📚Valor diferencial

Este proyecto no se limita a entrenar un modelo predictivo. Presenta una estructura reutilizable y profesional orientada a un caso real de ciberseguridad, con potencial evolución hacia:


## integración con SIEM
triage automático de alertas
mapeo con MITRE ATT&CK
enriquecimiento con threat intelligence
sistemas multiagente para respuesta a incidentes
generación automática de reportes ejecutivos y técnicos 
##



## 📚Tecnologías utilizadas
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Joblib
Machine Learning supervisado
Random Forest
Logistic Regression
One-Hot Encoding
StandardScaler
Classification Report
Confusion Matrix

## 📚Conjunto de datos

El proyecto utiliza UNSW-NB15 , un conjunto de datos ampliamente utilizado en investigación de ciberseguridad para detección de intrusiones y clasificación de ataques de red.

## La variable objetivo es:

`attack_cat`

## Clases utilizadas:

Normal
Generic
Exploits
Fuzzers
DoS
Reconnaissance
Analysis
Backdoor
Shellcode
Worms
Enfoque técnico

## 📚El pipeline desarrollado realiza:

1. Carga de datos de entrenamiento y prueba.
2. Limpieza y normalización de la variable attack_cat.
3. Separación entre variables predictoras y variable objetivo.
4. Eliminación de columnas con riesgo de fuga de información, como label.
5. Codificación de variables categóricas.
6. Imputación de valores faltantes.
7. Escalado de variables numéricas.
8. Entrenamiento de modelos supervisados.
9. Evaluación con métricas multiclase.
10. Selección del mejor modelo según F1 Macro.
11. Guardado del modelo entrenado.
12. Generación de matriz de confusión y reporte final.
Métricas utilizadas

## 📚 Se evaluó el rendimiento del modelo mediante:

Accuracy
Precision Macro
Recall Macro
F1 Macro
F1 Weighted
Classification Report
Confusion Matrix

## Se priorizó F1 Macro porque el conjunto de datos presenta desequilibrio entre clases, y esta métrica permite evaluar el desempeño considerando todas las categorías con el mismo peso.


