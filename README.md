# Estimación de la resistencia del concreto mediante regresión lineal

## Descripción del proyecto

Este proyecto desarrolla un análisis estadístico para estimar la resistencia a la compresión del concreto a partir de su composición y tiempo de curado.

Se comparan tres modelos de regresión: **OLS, Ridge y Lasso**, utilizando Python y las técnicas estudiadas en clase.

## Objetivo

Evaluar cuál de los tres modelos presenta un mejor desempeño para estimar la resistencia del concreto, medida en megapascales (MPa).

## Datos utilizados

- **Fuente:** UCI Machine Learning Repository.
- **Dataset:** Concrete Compressive Strength.
- **Observaciones:** 1.030.
- **Variables predictoras:** 8.
- **Variable objetivo:** resistencia del concreto (MPa).

[Consultar dataset original](https://archive.ics.uci.edu/dataset/165/concrete+compressive+strength)

## Metodología

1. Carga y exploración de los datos.
2. Análisis de correlaciones mediante un mapa de calor.
3. Entrenamiento de modelos OLS, Ridge y Lasso.
4. Evaluación mediante R² y RMSE.
5. Interpretación de resultados y conclusiones.

Se utiliza una división de 80 % para entrenamiento y 20 % para prueba, con `random_state=42`.

## Resultados

| Modelo | R² | RMSE (MPa) |
|:---|---:|---:|
| **Ridge** | **0,6276** | **9,7964** |
| OLS | 0,6275 | 9,7967 |
| Lasso | 0,5639 | 10,6008 |

Ridge presentó el mejor rendimiento numérico, aunque su diferencia respecto a OLS fue mínima en esta evaluación.

## Archivos del proyecto

- `Tarea_Resistencia_Concreto.ipynb`: desarrollo completo del análisis.
- `Concrete_Data.xls`: conjunto de datos original.

## Herramientas utilizadas

Python, Jupyter Notebook, pandas, NumPy, Matplotlib, Seaborn y scikit-learn.

## Fuente académica

Yeh, I-Cheng (1998). *Modeling of strength of high performance concrete using artificial neural networks*. Cement and Concrete Research, 28(12), 1797–1808.
