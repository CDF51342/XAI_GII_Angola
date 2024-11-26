# Índice Global de Innovación (GII) - Modelos Predictivos y Explicabilidad XAI

El objetivo del repositorio es construir un modelo predictivo para el Índice Global de Innovación (GII) utilizando explicabilidad (XAI) para analizar sus predicciones.

---

## Contenidos del README
- [Contenido del Proyecto](#contenido-del-proyecto)
  - [Objetivos](#objetivos)
  - [Archivos Principales](#archivos-principales)
- [Requisitos](#requisitos)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Explicabilidad local](#explicabilidad-local)

---

## Contenido del Proyecto

### Objetivos
1. **Modelo Predictivo**: Desarrollar un modelo para predecir el GII basado en los indicadores proporcionados.
2. **Capacidad Predictiva**: Evaluar y discutir el rendimiento del modelo.
3. **Explicaciones Globales**: Proporcionar interpretaciones generales sobre el modelo.
4. **Explicaciones Locales**: Generar explicaciones específicas para un país asignado según el NIA.
5. **Comparación**: Analizar la posible desviación entre las explicaciones globales y locales.

### Archivos Principales
- **`data/`**: Contiene datos de 132 países y 109 indicadores (medioambientales, educativos, energéticos, financieros, etc.) en formato *xlsx* ([Innova_2022.xlsx](data/Innova_2022.xlsx)) y *csv* ([Innova_2022.csv](data/Innova_2022.csv)). A su vez, en el directorio [models/](data/models) se encuentran los modelos de Random Forest obtenidos en los notebooks.
- **`notebooks/`**: Notebooks Jupyter para preprocesamiento ([EDA.ipynb](notebooks/EDA.ipynb)), desarrollo del modelo ([Random_Forest.ipynb](notebooks/Random_Forest.ipynb)) y análisis XAI ([XAI.ipynb](notebooks/XAI.ipynb)).
- **`images/`**: Imágenes obtenidas en el preprocesamiento ([EDA/](images/EDA)), creación del modelo ([RF/](images/RF)) y XAI ([XAI/](images/XAI)).
- **`README.md`**: Este archivo, que describe el propósito y contenido del repositorio.

---

## Requisitos
- Python 3.10 o superior
- Bibliotecas principales:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
  - `pickle`
  - `shap` (para interpretabilidad XAI)

Para instalar los requisitos:
```bash
pip install -r requirements.txt
```

---

## Estructura del Proyecto
- `data/`: Contiene los datos en formato Excel y CSV, junto con los modelos implementados.
- `notebooks/`: Notebooks para cada etapa del proyecto:
    - Exploración de datos
    - Entrenamiento de modelos
    - Análisis de explicabilidad
<!-- - `report/`: Resultados y discusión final en formato PDF. -->

## Explicabilidad Local
Para generar explicaciones locales para un país, utiliza el módulo 132 del NIA (100451342):
- NIA: 1000451342
- Cálculo: 1000451342 mod 132 = 2
- País: Angola (ID: 2)
El análisis local y global se encuentra documentado en el reporte final.
