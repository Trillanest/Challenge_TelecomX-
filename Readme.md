# 📊 Informe Final - Análisis de Evasión de Clientes (Churn) - TelecomX

## 🔹 Introducción

El presente análisis tiene como objetivo comprender los factores que contribuyen a la evasión de clientes (churn) en la empresa ficticia **TelecomX**, dedicada a ofrecer servicios de telefonía, internet y televisión. La retención de clientes es uno de los pilares del crecimiento sostenible de una empresa. Por ello, identificar patrones de comportamiento de los clientes que abandonan el servicio es crucial para diseñar estrategias efectivas de fidelización.

---

## 🔹 Limpieza y Tratamiento de Datos

Para garantizar la calidad de los análisis, se realizaron los siguientes pasos:

- 📁 Importación de datos desde el repositorio oficial del desafío.
- 🔍 Revisión de tipos de datos y nombres de columnas.
- 🧹 Estandarización de nombres de columnas para facilitar su uso en el código.
- 🔄 Conversión de la variable `Churn` a formato binario (`0` para clientes activos y `1` para clientes que abandonaron).
- 🧽 Eliminación de columnas irrelevantes o con datos inconsistentes si fue necesario.
- 💡 Conversión de columnas numéricas con formato de texto a tipo `float`, como `account_Charges_Total`.

---

## 🔹 Análisis Exploratorio de Datos (AED)

### ✅ Estadísticas descriptivas

Se usó `df.describe()` para comprender el rango, media, desviación estándar y valores extremos de las variables numéricas. Esto ayudó a identificar posibles outliers y entender el perfil promedio del cliente.

### ✅ Distribución de la variable objetivo `Churn`

Se realizó un gráfico de barras para visualizar cuántos clientes permanecieron (`No`) y cuántos se dieron de baja (`Sí`). Este gráfico reveló el desbalance de clases en los datos (más clientes permanecen que los que cancelan).

### ✅ Análisis de correlaciones y visualizaciones

- Se analizaron variables como:
  - **Tenencia del cliente (`customer_tenure`)**
  - **Tipo de contrato (`account_Contract`)**
  - **Servicios adicionales (seguridad, respaldo, soporte técnico)**
  - **Método de pago (`account_PaymentMethod`)**
- Se utilizaron gráficos de barras, histogramas y heatmaps para entender cómo estas variables se relacionan con el churn.

---

## 🔹 Conclusiones e Insights

📌 Entre los hallazgos más relevantes:

- Los clientes con contrato **mensual** presentaron una **tasa de evasión significativamente mayor** que aquellos con contratos anuales o por dos años.
- La mayoría de los clientes que abandonan **no cuentan con servicios adicionales** como respaldo en línea o soporte técnico.
- Los clientes con cargos mensuales más altos tienen una **mayor probabilidad de evasión**, especialmente si su permanencia es menor a un año.
- El método de pago también influye: clientes que pagan con tarjetas virtuales o medios electrónicos tienen una tasa de churn más elevada.

---

## 🔹 Recomendaciones

Con base en los análisis anteriores, se proponen las siguientes estrategias:

1. **Incentivar contratos a largo plazo** mediante descuentos o beneficios exclusivos.
2. **Promover la activación de servicios adicionales**, como soporte técnico y respaldo, destacando su valor en la experiencia del cliente.
3. **Revisar las tarifas mensuales** y ofrecer planes más flexibles para clientes con cargos elevados.
4. **Segmentar campañas de retención** enfocadas en clientes con menos de 6 meses de antigüedad.
5. **Optimizar métodos de pago** para hacerlos más amigables, seguros y confiables, promoviendo los que tienen mejor tasa de retención.

---

📌 Este análisis es solo el punto de partida. Un estudio más profundo con técnicas de Machine Learning podría prever el churn antes de que ocurra, permitiendo una acción proactiva por parte de TelecomX.
