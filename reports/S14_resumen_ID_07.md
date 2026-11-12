# S14 - Resumen del análisis (ID 07)

## Datos de partida

| Campo | Valor |
|---|---|
| ID estudiante | 07 |
| Semilla | 1007 |
| Huella de muestra | 3d3c38ac538c |
| Muestra | 35000 |
| Train | 24500 |
| Valid | 5250 |
| Test | 5250 |

## PCA (Tarea 1)

- Variables numéricas: 24
- Componentes conservadas: 15
- Varianza acumulada conservada: 0.9024
- Varianza fuera: 0.0976

## Experimentos A-D (Tareas 2 y 3)

| Experimento | Usa PCA | Componentes | Columnas | C | Accuracy | Precision | Recall | F1 | Average Precision | ROC-AUC | TN | FP | FN | TP | Predichos tardíos | Costo (R$) | Convergencia |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| A | False | - | 149 | 1.0 | 0.6688 | 0.1223 | 0.6292 | 0.2048 | 0.1685 | 0.7127 | 3287 | 1607 | 132 | 224 | 1831 | 17476 | True |
| B | True | 15 | 140 | 1.0 | 0.6516 | 0.1146 | 0.6152 | 0.1932 | 0.1445 | 0.6817 | 3202 | 1692 | 137 | 219 | 1911 | 18331 | True |
| C | True | 15 | 140 | 0.1 | 0.6535 | 0.1160 | 0.6208 | 0.1955 | 0.1427 | 0.6871 | 3210 | 1684 | 135 | 221 | 1905 | 18197 | True |
| D | True | 15 | 140 | 10.0 | 0.6520 | 0.1155 | 0.6208 | 0.1948 | 0.1445 | 0.6798 | 3202 | 1692 | 135 | 221 | 1913 | 18261 | True |

## Costo de referencia

- Costo referencia (R$): 12460

## Modelo elegido

- Experimento: A
- Costo (R$): 17476
- Recall: 0.6292
- F1: 0.2048
- Average Precision: 0.1685

## Prueba de Kolmogorov-Smirnov (Tarea 4)

- n entrenamiento: 24500
- n validación: 5250
- D: 0.018313
- p-valor: 0.108662
- alfa: 0.05
- Decisión mecánica: no se rechaza H0
- Ubicación de la máxima separación: 13.55

## Archivos generados en reports/

- S12_resultados_ID_07.json
- S14_varianza_PCA_ID_07.png
- S14_ECDF_flete_ID_07.png
- S14_experimentos_ID_07.csv
- S14_resumen_ID_07.json
- S14_resumen_ID_07.md

## Interpretación

Las conclusiones por tarea están en las celdas de conclusión del notebook S12_ML_Challenge.ipynb (sección Semana 14).
