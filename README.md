# Predicción de Precios de Casas con Aprendizaje Automático

## Autores

- **Wellington Cortes Álvarez**
- **Fabio Alejandro Sastoque Rincón**

---

## Descripción del Proyecto

Este proyecto es una aplicación de técnicas de aprendizaje automático para la predicción de precios de casas, desarrollado como parte de la Maestría en Inteligencia Artificial y Ciencia de datos de la Universidad Autónoma de Occidente. El objetivo principal es analizar un conjunto de datos inmobiliarios, realizar un proceso completo de análisis y limpieza, y construir modelos predictivos que permitan estimar el valor de una vivienda a partir de sus características.

---

## Estructura del Proyecto

- `Final.ipynb`: Notebook principal con todo el flujo de trabajo, desde la carga de datos hasta la evaluación de modelos.
- `data_hause.csv`: Archivo de datos utilizado para el análisis y entrenamiento de los modelos.
- `requirements.txt`: Lista de dependencias necesarias para ejecutar el proyecto.
- `.gitignore`: Archivos y carpetas ignorados por git.
- `README.md`: Docuementación del proyecto.

---

## Flujo de Trabajo

### 1. **Carga y Exploración de Datos**
   - Se utiliza `pandas` para cargar el archivo `data_hause.csv`.
   - Se realiza una inspección inicial de los datos, visualizando las primeras filas y revisando los tipos de variables y la existencia de valores nulos.

### 2. **Preprocesamiento y Limpieza**
   - Conversión de fechas y renombramiento de columnas para facilitar el análisis.
   - Análisis descriptivo de las variables numéricas.
   - Visualización de la distribución de variables y detección de valores atípicos (outliers).
   - Eliminación de outliers utilizando el rango intercuartílico (IQR).
   - Eliminación de columnas irrelevantes para el modelo.

### 3. **Análisis Exploratorio de Datos**
   - Visualización de correlaciones entre variables mediante mapas de calor.
   - Gráficas de dispersión y boxplots para entender la relación entre variables y el precio.

### 4. **Preparación de Datos para Modelado**
   - Separación de variables predictoras (`X`) y variable objetivo (`y`).
   - División del conjunto de datos en entrenamiento y prueba.

### 5. **Modelado Predictivo**
   - **Random Forest Regressor:** Entrenamiento y evaluación de un modelo de bosque aleatorio.
   - **Regresión Lineal:** Entrenamiento y evaluación de un modelo de regresión lineal.
   - **Gradient Boosting Regressor:** Entrenamiento y evaluación de un modelo de boosting por gradiente.

### 6. **Evaluación de Modelos**
   - Se utilizan métricas como R², MAE y RMSE para comparar el desempeño de los modelos.
   - Visualización de resultados y comparación entre valores reales y predichos.

### 7. **Predicción con Nuevos Datos**
   - Se realizan predicciones con datos de ejemplo para validar la utilidad de los modelos entrenados.

---

## Requisitos

Para ejecutar este proyecto, asegúrate de tener instalado Python 3.11+ y las siguientes librerías:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Puedes instalar todas las dependencias ejecutando:

```sh
pip install -r requirements.txt
```

---

## Ejecución

1. Clona este repositorio.
2. Instala las dependencias.
3. Abre el archivo [Final.ipynb](Final.ipynb) en Jupyter Notebook o Visual Studio Code.
4. Ejecuta las celdas secuencialmente para reproducir el análisis y los resultados.

---

## Resultados

El proyecto demuestra cómo diferentes modelos de aprendizaje automático pueden ser aplicados para predecir precios de casas, mostrando sus ventajas y limitaciones. Se incluyen visualizaciones y métricas para facilitar la interpretación de los resultados.

---

