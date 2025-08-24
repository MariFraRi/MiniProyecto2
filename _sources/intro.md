# Introducción  

Este Jupyter Book presenta el **Proyecto Integrador de Aprendizaje Automático 3**, enfocado en la aplicación de **modelos supervisados de regresión y clasificación binaria** para el análisis de autos usados.  

El objetivo principal es construir un flujo de trabajo completo que permita:  

- **Predecir el precio de un vehículo usado** a partir de sus características técnicas, operativas y de mercado.  
- **Clasificar si un auto se encuentra en alta o baja demanda**, en función de una etiqueta creada con base en el precio mediano.  

El contexto de aplicación corresponde a **plataformas de compra-venta de autos usados**, donde los modelos predictivos pueden apoyar a compradores y vendedores en decisiones más informadas y transparentes.  

El proyecto se desarrolla con un **dataset real de autos usados** (ejemplo: Craigslist Cars & Trucks Dataset en Kaggle), e incluye las siguientes etapas:  

- **Preprocesamiento de datos**: manejo de valores faltantes, codificación categórica y escalado.  
- **Construcción de pipelines** que integran transformaciones y modelos (Ridge, Lasso y Logistic Regression).  
- **Búsqueda de hiperparámetros** mediante **GridSearchCV con validación cruzada**.  
- **Evaluación cuantitativa y visual** de los modelos de regresión (MAE, RMSE, R²) y clasificación (matriz de confusión, accuracy, precision, recall, F1-score, curva ROC y AUC).  
- **Análisis comparativo** de los resultados y reflexión sobre el impacto de la regularización y las variables más influyentes.  

El resultado esperado es un notebook/documento bien estructurado, con explicaciones claras, gráficos ilustrativos y justificación de cada decisión técnica, ideal como evidencia de integración de conocimientos en aprendizaje automático aplicado.  

```{tableofcontents}
```
