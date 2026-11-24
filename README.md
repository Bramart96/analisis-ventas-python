# Análisis de ventas con Python | 2024

Desarrollé un análisis exploratorio de ventas para un escenario de pequeña empresa, utilizando **Python, pandas y Matplotlib**. Organicé el procesamiento, calculé indicadores comerciales y generé una visualización de evolución diaria.

## Dataset

Trabajé con `sales_sample_2024.csv`, un conjunto de ejemplo con **366 registros diarios de 2024** y las columnas `id`, `sales_date` y `sales_amount`.

El script original lee los datos desde una URL pública, por lo que esa ejecución necesita conexión a Internet. Incluí además una copia de referencia en `datos/`.

## Trabajo realizado

- Cargué y examiné el dataset con pandas.
- Calculé ventas totales, promedio diario y valores máximo y mínimo.
- Convertí y ordené las fechas para representar correctamente la serie temporal.
- Agrupé las ventas por día y generé el gráfico en Matplotlib.
- Guardé la evidencia visual en `resultados/grafico_ventas.png`.

## Resultados comprobados

| Indicador | Valor |
|---|---:|
| Registros procesados | 366 |
| Ventas totales | 1.812.114 |
| Promedio diario | 4.951,13 |
| Venta máxima | 8.960 |
| Venta mínima | 1.003 |

Los importes pertenecen al dataset de ejemplo; no les atribuí una moneda que la fuente no especifica.

![Evolución de ventas diarias en 2024](resultados/grafico_ventas.png)

## Ejecución

Desde la raíz del repositorio:

```bash
python -m pip install pandas matplotlib
python scripts/analisis_ventas.py
```

El script escribe el gráfico en la carpeta `resultados/`.

## Organización y trazabilidad

```text
datos/sales_sample_2024.csv   Copia del dataset
scripts/analisis_ventas.py    Cálculos y gráfico
scripts/revision_tecnica.txt  Revisión documentada
resultados/grafico_ventas.png Resultado visual
```

Realicé el trabajo como ejercicio de gestión de versiones con **Git, GitHub y Jira**, utilizando roles de líder, desarrollo y revisión para organizar las tareas. Conservé la trazabilidad de las actividades en el historial de commits.
