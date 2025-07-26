# Pronóstico de Demanda con IA y Métodos Tradicionales

# Demand Forecasting with AI and Traditional Methods

Este proyecto forma parte del Trabajo Fin de Máster (TFM) y tiene como objetivo comparar métodos clásicos
(SES, MA-3) con modelos de Inteligencia Artificial (Prophet, Random Forest, Keras) para pronosticar la demanda
semanal del producto *leche entera 1L* en un supermercado (Albert Heijn, Países Bajos) (datos simulados).


This project is part of the Master's Thesis (TFM) and aims to compare classical methods (SES, MA-3) 
with Artificial Intelligence models (Prophet, Random Forest, Keras) to forecast the weekly demand for the 1L 
whole milk product in a supermarket (Albert Heijn, Netherlands) (simulated data).

---

## Estructura del proyecto
## Project Structure
Pronostico
.
|-- README.md
|-- data
|   `-- demanda_semanal.csv
|-- deep_learning
|   |-- keras_ann.py
|   `-- keras_utils.py
|-- machine_learning
|   |-- feature_engineering.py
|   `-- random_forest.py
|-- main.py
|-- notebooks
|   `-- visualizaciones.ipynb
|-- prophet_model
|   `-- prophet_forecast.py
|-- requirements.txt
|-- results
|   |-- graficos
|   `-- metricas
|-- traditional_models
|   |-- ma3_model.py
|   `-- ses_model.py
`-- utils
    `-- utils.py

## Instalación del entorno
## Installing the environment

1. **Clona este repositorio**:
1. **Clone this repository**:

```bash
git clone https://github.com/Benja1512/pronostico_tfm.git


## Crea un entorno virtual 
## Create a virtual environment

python -m venv venv
source venv/bin/activate      # Linux/macOS
venv\Scripts\activate         # Windows

## Instala las dependencias
## Install dependencies

pip install --upgrade pip
pip install -r requirements.txt

## Modelos incluidos 
## Models included

| Tipo                    | Modelos                                          |
| ----------------------- | ------------------------------------------------ |
| Métodos tradicionales   | MA-3, SES (Simple Exponential Smoothing)         |
| Inteligencia Artificial | Prophet, Random Forest, Redes Neuronales (Keras) |

## Datos 
## Data

data/demanda_semanal.csv: contiene las series de demanda semanal simulada para entrenamiento y prueba.
data/demanda_semanal.csv: Contains the simulated weekly demand series for training and testing.


## Objetivos del Proyecto
## Project Objectives

- Comparar el rendimiento de modelos clásicos y de inteligencia artificial para predecir demanda semanal.
- Evaluar métricas como MAE y RMSE.
- Simular decisiones de inventario basadas en los resultados de pronóstico.

- Compare the performance of classical and artificial intelligence models for predicting weekly demand.
- Evaluate metrics such as MAE and RMSE.
- Simulate inventory decisions based on forecast results.


## Modelos Implementados
## Implemented Models

- **MA-3**: Media móvil simple de 3 períodos.
- **SES**: Suavizamiento exponencial simple (α configurable).
- **Prophet**: Modelo desarrollado por Meta, ideal para series temporales con estacionalidad.
- **Random Forest**: Ensamble de árboles de decisión, útil para capturar patrones no lineales.
- **Keras ANN**: Red neuronal artificial con capas densas para aprendizaje supervisado.

- **MA-3**: 3-period simple moving average.
- **SES**: Simple exponential smoothing (configurable α).
- **Prophet**: Model developed by Meta, ideal for time series with seasonality.
- **Random Forest**: Ensemble of decision trees, useful for capturing nonlinear patterns.
- **Keras ANN**: Artificial neural network with dense layers for supervised learning.

## Ejemplo de uso rápido 
## (Quick Start)


```bash
# Ejecutar el modelo tradicional SES
python traditional_models/ses_model.py

# Ejecutar Random Forest
python machine_learning/random_forest.py

# Ejecutar red neuronal
python deep_learning/keras_ann.py

```bash
# Run the traditional SES model
python traditional_models/ses_model.py

# Run Random Forest
python machine_learning/random_forest.py

# Run the neural network
python deep_learning/keras_ann.py


--------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------
## Licencia

Este proyecto fue desarrollado con fines académicos como parte del Trabajo Fin de Máster (VIU, 2025).  
No se autoriza su uso comercial sin consentimiento previo del autor.

## License

This project was developed for academic purposes as part of the Master's Thesis (VIU, 2025).
Commercial use is prohibited without prior consent from the author.

------------------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------------------

## Autor

**Benjamín Ford Ontiveros Ordinola**  

Correo Personal
benjamin.ontiveros@gmail.com

Correo Institucional
bontiveroso@student.universidadviu.com

Máster en Supply Chain Management y Logística - VIU (2025)


## Author

**Benjamín Ford Ontiveros Ordinola**

Personal Email
benjamin.ontiveros@gmail.com

Institutional Email
bontiveroso@student.universidadviu.com

Master's Degree in Supply Chain Management and Logistics - VIU (2025)

-------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------