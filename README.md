# Índice Global de Innovación (GII) - Modelos Predictivos y Explicabilidad XAI

El objetivo del repositorio es construir un modelo predictivo para el Índice Global de Innovación (GII) utilizando explicabilidad (XAI) para analizar sus predicciones.

---

## Contenido del Proyecto

### Objetivos
1. **Modelo Predictivo**: Desarrollar un modelo para predecir el GII basado en los indicadores proporcionados.
2. **Capacidad Predictiva**: Evaluar y discutir el rendimiento del modelo.
3. **Explicaciones Globales**: Proporcionar interpretaciones generales sobre el modelo.
4. **Explicaciones Locales**: Generar explicaciones específicas para un país asignado según el NIA.
5. **Comparación**: Analizar la posible desviación entre las explicaciones globales y locales.

### Archivos Principales
- **`data/Innova_2022.xlsx`**: Contiene datos de 132 países y 109 indicadores (medioambientales, educativos, energéticos, financieros, etc.).
- **`notebooks/`**: Notebooks Jupyter para preprocesamiento, desarrollo del modelo y análisis XAI.
<!-- - **`scripts/`**: Scripts de Python para entrenar modelos y generar explicaciones. -->
- **`README.md`**: Este archivo, que describe el propósito y contenido del repositorio.

---

## Requisitos
- Python 3.8 o superior
- Bibliotecas principales:
  - `pandas`
  - `scikit-learn`
  - `matplotlib`
  - `shap` (para interpretabilidad XAI)

Para instalar los requisitos:
```bash
pip install -r requirements.txt
```

---

## Estructura del Proyecto
- `data/`: Contiene los datos en formato Excel y sus versiones procesadas.
- `notebooks/`: Notebooks para cada etapa del proyecto:
    - Exploración de datos
    - Entrenamiento de modelos
    - Análisis de explicabilidad
- `scripts/`: Scripts reutilizables para análisis automatizados.
<!-- - `report/`: Resultados y discusión final en formato PDF. -->

## Explicabilidad Local
Para generar explicaciones locales para un país, utiliza el módulo 132 del NIA (100451342):
- NIA: 1000451342
- Cálculo: 1000451342 mod 132 = 2
- País: Angola (ID: 2)
El análisis local y global se encuentra documentado en el reporte final.
