# Predicción de Precios de Vivienda - House Prices: Advanced Regression Techniques

Proyecto desarrollado en el marco del curso Modelos y Simulación II del programa de Ingeniería de Sistemas de la Universidad de Antioquia. El objetivo es construir un sistema de predicción de precios de vivienda mediante técnicas de aprendizaje supervisado, comparando distintos algoritmos de regresión sobre el dataset House Prices: Advanced Regression Techniques disponible en Kaggle.

## Descripción del problema

El dataset corresponde a propiedades residenciales ubicadas en Ames, Iowa, e incluye 1460 observaciones de entrenamiento y 1459 de prueba descritas mediante 81 variables de tipo numérico y categórico. La variable objetivo `SalePrice` es de tipo continuo, por lo que el problema se aborda como una tarea de regresión bajo el paradigma de aprendizaje supervisado.

Enlace al dataset original: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques

## Integrantes del grupo

- Cristian Alberto Agudelo Marquez — cristian.agudelo1@udea.edu.co
- Brandon Duque García — brandon.duque@udea.edu.co
- Jorge Luis Rodriguez Jimenez — jorge.rodriguezj@udea.edu.co

## Estructura del repositorio

```
.
├── data/
│   ├── train.csv
│   └── test.csv
├── notebooks/
│   └── house_prices_analysis.ipynb
├── reporte/
│   └── Informe_Modelos_II.pdf
├── requirements.txt
└── README.md
```

- `data/` contiene los archivos originales del dataset descargados desde Kaggle.
- `notebooks/` incluye el cuaderno Jupyter con el análisis exploratorio, el preprocesamiento y la evaluación de modelos.
- `reporte/` almacena el informe del proyecto en formato PDF, elaborado bajo la plantilla IEEE Transactions.
- `requirements.txt` lista las dependencias necesarias para reproducir los resultados.

## Requisitos

- Python 3.10 o superior
- Jupyter Notebook o JupyterLab
- Las librerías indicadas en `requirements.txt`

## Instalación

Clonar el repositorio:

```bash
git clone https://github.com/usuario/house-prices-modelos-ii.git
cd house-prices-modelos-ii
```

Crear un entorno virtual e instalar las dependencias:

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

En Windows, activar el entorno con:

```bash
venv\Scripts\activate
```

## Reproducción de los resultados

1. Descargar los archivos `train.csv` y `test.csv` desde la página de la competencia en Kaggle y ubicarlos en la carpeta `data/`.
2. Iniciar Jupyter:

```bash
jupyter notebook
```

3. Abrir el archivo `notebooks/house_prices_analysis.ipynb` y ejecutar las celdas en orden.

El cuaderno está organizado en las siguientes secciones: carga de datos, análisis exploratorio, preprocesamiento, ingeniería de características, entrenamiento de modelos, validación y comparación de resultados.

## Modelos considerados

El proyecto contempla la evaluación comparativa de los siguientes algoritmos de regresión:

- Regresión lineal (modelo base)
- Regresión Lasso
- K-Nearest Neighbors
- Random Forest
- Gradient Boosting
- Red neuronal multicapa
- Máquinas de vectores de soporte

## Métricas de evaluación

El desempeño de los modelos se evalúa mediante las siguientes métricas: error absoluto medio (MAE), error cuadrático medio (MSE), raíz del error cuadrático medio (RMSE) y coeficiente de determinación (R²).

## Referencias

[1] R.-T. Mora-Garcia, M.-F. Cespedes-Lopez y V. R. Perez-Sanchez, "Housing price prediction using machine learning algorithms in COVID-19 times," Land, vol. 11, no. 11, p. 2100, 2022.

[2] I. Moreno-Foronda, M.-T. Sánchez-Martínez y M. Pareja-Eastaway, "Comparative analysis of advanced models for predicting housing prices: A review," Urban Science, vol. 9, no. 2, p. 32, 2025.
