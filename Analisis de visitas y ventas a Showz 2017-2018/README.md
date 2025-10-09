**<h1>🎟️ **Proyecto: Análisis de Visitas y Ventas — Showz (2017–2018)**</h1>**
📘 **Descripción General**

Este proyecto analiza el comportamiento de los usuarios y la rentabilidad de las campañas de marketing de Showz, una empresa dedicada a la venta de entradas para eventos.

El objetivo principal es comprender cómo los visitantes interactúan con el sitio web, cuándo realizan sus compras y cómo las campañas de marketing afectan las ventas y la rentabilidad de la empresa.

🎯 **Objetivos del Proyecto**

1. Analizar el comportamiento de usuarios y sus patrones de compra.

2. Evaluar la eficacia de las estrategias de marketing mediante métricas financieras clave.

3. Calcular el LTV (Lifetime Value) y el CAC (Customer Acquisition Cost).

4. Identificar puntos de equilibrio entre ingresos y gastos de adquisición.

5. Recomendar estrategias para optimizar la inversión publicitaria y maximizar el retorno (ROMI).

🧩 **Plan de Trabajo**

1. Preparación y limpieza de datos: verificación de formatos, duplicados y tipos de variables.

2. Análisis exploratorio (EDA): tendencias de tráfico, comportamiento de compra y duración de sesiones.

3. Cálculo de métricas clave:

4. Visitantes únicos diarios, semanales y mensuales.

5. Duración promedio de las sesiones.

6. Conversión por fuente y dispositivo.

6. ROMI, CAC y LTV.

7. Comparación de estrategias de marketing: identificación de las más rentables.

8. Segmentación temporal: análisis de estacionalidad y picos de demanda.

9. Conclusiones y recomendaciones.

🧾 **Descripción de los Datos**

Los datos abarcan el periodo de enero de 2017 a diciembre de 2018, incluyendo tres fuentes principales:

- Tipo de Datos	Descripción
- Visitas web	Información sobre usuarios, dispositivos y duración de sesiones.
- Pedidos	Registros de compras, ingresos y fechas.
- Campañas publicitarias	Gastos, estrategias de marketing y fuentes de adquisición.
📊 **Resultados Principales**
🔹 **Tráfico y comportamiento de usuarios**

- Promedio de 907.9 visitantes únicos diarios, 5716.2 semanales y 23,228 mensuales.

- La similitud entre visitantes únicos y número de sesiones sugiere que la mayoría de usuarios visita el sitio una vez al día.

- Cerca del 10 % de las sesiones duraron 0 segundos, lo cual podría indicar errores de registro o rebotes inmediatos.

- En promedio, las sesiones duraron 643 segundos, aunque se observaron valores atípicos hasta 84,480 segundos.

🔹 **Patrones de compra**

- La mayoría de los usuarios realizan su primera compra el mismo día que su primera sesión, lo que indica compras impulsivas.

- Los meses con mayores ventas fueron octubre, diciembre, febrero y abril, coincidiendo con festividades y eventos de temporada.

- Cada compra tuvo un valor promedio de USD $5, y el gasto total promedio por usuario fue de USD $6.9.

🔹 **Eficiencia de campañas de marketing**

- La estrategia 4 atrajo más clientes (14,253), seguida de la estrategia 3 (13,846).

- Sin embargo, la estrategia 3 fue la más costosa (USD $141,321) y generó pérdidas, ya que su inversión superó los ingresos obtenidos.

- La estrategia 1 mostró el mayor ROMI (Return on Marketing Investment).

- La estrategia 9 fue la más eficiente en costo por visitante (CAC), aunque con una inversión muy baja.

📈 **Conclusiones**

1. La empresa Showz es rentable, pero existen desequilibrios en la asignación del presupuesto publicitario.

2. Se recomienda reducir o reevaluar la estrategia 3, debido a su baja rentabilidad.

3. Las estrategias 1 y 9 tienen alto potencial: se sugiere aumentar la inversión en ambas para incrementar el retorno global.

4. Las ventas presentan estacionalidad: los picos en meses festivos reflejan la influencia de las campañas y la demanda del mercado.

5. Se recomienda investigar la causa de las sesiones con duración 0 s para mejorar la calidad del seguimiento analítico.

💡 **Recomendaciones**

- Implementar un sistema de seguimiento de conversiones más detallado (por fuente y dispositivo).

- Ajustar el presupuesto de marketing según el ROMI y CAC histórico.

- Optimizar las campañas previas a las temporadas altas (octubre–diciembre y febrero–abril).

- Realizar A/B testing entre estrategias para validar su eficacia antes de incrementar inversión.


💻 **Tecnologías Utilizadas**

- Python 3.11:

  Pandas, NumPy

  Matplotlib, Seaborn

- Jupyter Notebook
