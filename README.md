# Comparación de modelos de Machine Learning para predicción de fallas en congeladores

## Autor
**David Díaz**  
Maestría en Inteligencia Artificial – Guatemala, 2025

---

## Descripción general
Este repositorio contiene el código fuente utilizado en el trabajo de graduación y se encuentra disponible en GitHub: https://github.com/daviddiaz012/David_Diaz_ComparativaDeModelosPdM.

El repositorio contiene el código fuente utilizado en el trabajo de graduación **“Comparación de modelos de Machine Learning para predicción de fallas en congeladores”**.  
El objetivo del proyecto es evaluar de forma comparativa distintos modelos de *Machine Learning* aplicados a la predicción de fallas en congeladores comerciales, utilizando datos históricos reales de operación, bajo un enfoque metodológico **CRISP-DM**.

El estudio se enfoca en un **horizonte de predicción de 30 días** y no contempla el desarrollo ni la implementación de una solución de software en ambiente productivo.

---

## Dataset
- **Nombre del dataset**: `Dataset_Congeladores_Para_Predicion_De_Fallas.csv`  
- **Origen**: Datos históricos reales de operación de congeladores comerciales (Helados Sarita, Guatemala).  
- **Tipo de datos**: Tabulares, heterogéneos y desbalanceados.  
- **Contenido general**:
  - Identificación del congelador
  - Variables operativas
  - Historial de fallas y mantenimientos
  - Variables derivadas (cuando aplica)
  
> ⚠️ **Nota**: El dataset no se incluye en el repositorio por motivos de confidencialidad.

---

## Estructura del proyecto

```
├── David_Diaz_Comparativa_De_Modelos_ML_PdM.ipynb
├── README.md
└── data/
    └── Dataset_Congeladores_Para_Predicion_De_Fallas.csv   (no incluido)
```

---

## Modelos evaluados
En el cuaderno se entrenan y comparan los siguientes modelos:

- Regresión Logística
- Árboles de Decisión
- Random Forest
- XGBoost (Extreme Gradient Boosting)
- Red neuronal densa (MLP)

---

## Metodología
El desarrollo experimental sigue la metodología **CRISP-DM**, abarcando las fases de:

1. Comprensión del negocio
2. Comprensión de los datos
3. Preparación de los datos
4. Modelado
5. Evaluación
6. Documentación de resultados

---

## Métricas de evaluación
Debido al desbalance de clases presente en el dataset, se utilizan métricas orientadas a la detección efectiva de fallas:

- Precision
- Recall
- F1-score
- AUC-ROC
- Matriz de confusión

El análisis prioriza la reducción de **falsos negativos**, dada su implicación operativa en el contexto del mantenimiento predictivo.

---

## Requisitos técnicos

### Librerías principales
- Python 3.x
- pandas
- numpy
- scikit-learn
- xgboost
- matplotlib
- seaborn

> El listado completo de librerías se encuentra documentado en el **Anexo B** del trabajo de graduación.

---

## Ejecución
1. Clonar el repositorio.
2. Colocar el dataset en la carpeta `/data`.
3. Abrir el archivo `David_Diaz_Comparativa_De_Modelos_ML_PdM.ipynb`.
4. Ejecutar las celdas de forma secuencial para reproducir el experimento.

---

## Resultados principales
Los resultados del estudio muestran que los modelos de ensamble basados en árboles de decisión, particularmente **XGBoost**, presentan el mejor equilibrio entre desempeño técnico y aplicabilidad operativa bajo las condiciones del dataset analizado.

---

## Notas finales
Este código forma parte de un trabajo académico y está orientado a la **reproducibilidad del experimento** y al análisis comparativo de modelos, no a su uso directo en producción.

---

## Licencia
Uso académico y educativo. No autorizado para uso comercial sin consentimiento del autor.

