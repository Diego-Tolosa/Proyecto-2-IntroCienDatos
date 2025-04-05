# 🧪 Análisis Descriptivo del Dataset – Avocado Prices 🥑

## 📄 Descripción General del Dataset

El dataset contiene información sobre los precios promedio de aguacates en distintas regiones de Estados Unidos, a lo largo del tiempo. Algunas de las columnas principales son:

- `Date`: Fecha de recolección del dato.  
- `AveragePrice`: Precio promedio del aguacate.  
- `type`: Tipo de aguacate (convencional u orgánico).  
- `region`: Región donde se recolectó el dato.  
- `Total Volume`: Volumen total vendido.  
- Además, incluye columnas desglosadas por tipo de aguacate y tamaño (4046, 4225, 4770).

El dataset cuenta con más de **18,000 registros**, lo cual lo hace adecuado para tareas de machine learning.

---

## 📊 Estadísticas Descriptivas

- El precio promedio del aguacate oscila entre **0.44 y 3.25 dólares**, con una media cercana a **1.40 USD**.
- Algunas variables presentan **amplia dispersión**, como el volumen de ventas.
- No se identificaron **valores nulos** en las columnas principales (`AveragePrice`, `Total Volume`, `type`, etc.).

---

## 📈 Visualizaciones e Insights

### 🔹 Histogramas

- Las distribuciones de `AveragePrice` y `Total Volume` están **sesgadas a la derecha**: hay más precios bajos y pocos casos con valores extremos.
- Las columnas de volumen por tipo de aguacate muestran comportamiento similar: **muchas observaciones con ventas bajas** y unos pocos valores muy altos.

### 🔹 Boxplots

- Se observaron varios **outliers** en las variables de volumen (`Total Volume`, `4046`, `4225`, `4770`), lo cual es esperado por la naturaleza del negocio (ventas muy altas en ciertas fechas o regiones).
- La variable `AveragePrice` tiene algunos valores atípicos altos, pero no excesivos.

### 🔹 Correlaciones

- Existe una **fuerte correlación positiva** entre:
  - `Total Volume` y `4046`, `4225`: tiene sentido, ya que son subconjuntos del volumen total.
- `AveragePrice` tiene **baja correlación** con el volumen total o las demás variables, lo que indica que el precio no depende directamente de la cantidad vendida.

### 🔹 Comparación por tipo

- El **aguacate orgánico** suele tener un **precio promedio mayor** que el convencional, lo que confirma su percepción como un producto premium.

### 🔹 Evolución temporal

- Los precios fluctúan con el tiempo, mostrando cierta **estacionalidad** (picos en algunos meses o años).
- A partir de 2017, se observan precios promedio ligeramente más altos.

---

## 🧠 Conclusiones del Análisis

- El dataset está **bien estructurado y completo** para aplicar modelos predictivos.
- Existen diferencias importantes entre **tipo de aguacate** y **región**, que probablemente influirán en el modelo.
- Se identifican variables numéricas con outliers, que podrían necesitar tratamiento en la fase de limpieza.
- El **precio promedio** es una buena variable objetivo para predecir, ya que está disponible en todos los registros y es continua.

