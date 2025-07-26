# Pronóstico de Demanda con IA y Métodos Tradicionales

Este proyecto forma parte del Trabajo Fin de Máster (TFM) y tiene como objetivo comparar métodos clásicos
(SES, MA-3) con modelos de Inteligencia Artificial (Prophet, Random Forest, Keras) para pronosticar la demanda
semanal del producto *leche entera 1L* en un supermercado (Albert Heijn, Países Bajos) (datos simulados).

---

## Estructura del proyecto
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

1. **Clona este repositorio**:

```bash
git clone https://github.com/Benja1512/pronostico_tfm.git
cd PronosticoTFM