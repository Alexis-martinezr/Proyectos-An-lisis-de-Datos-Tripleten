# 🛒 Optimización de Ingresos y Análisis de Test A/B

## 📘 Introducción
Este proyecto aborda el **análisis y priorización de hipótesis** para optimizar los ingresos de una tienda online, así como la **evaluación de un experimento A/B**.

En la primera fase, se dispone de nueve hipótesis con información sobre **alcance (Reach)**, **impacto (Impact)**, **confianza (Confidence)** y **esfuerzo (Effort)**. El objetivo es priorizarlas utilizando los frameworks **ICE** y **RICE**, comparando los resultados y explicando las diferencias entre ambos enfoques.

En la segunda fase, se analizan los resultados de un **test A/B** que incluye datos de pedidos y visitas por grupo. Se estudian métricas como **ingresos acumulados**, **tamaño promedio de pedido**, **tasas de conversión** y se identifican valores atípicos. Posteriormente, se realiza un análisis estadístico para determinar si las diferencias entre grupos son significativas, permitiendo tomar decisiones sobre la prueba.

---

## 📂 Datasets Utilizados

### 1. `hypotheses_us.csv`
Contiene nueve hipótesis para aumentar ingresos:  
- `Hypotheses`: breve descripción de la hipótesis.  
- `Reach`: alcance del usuario (1–10).  
- `Impact`: impacto en usuarios (1–10).  
- `Confidence`: confianza en la hipótesis (1–10).  
- `Effort`: esfuerzo requerido para probar la hipótesis (1–10).

### 2. `orders_us.csv`
Contiene información de pedidos:  
- `transactionId`: identificador del pedido.  
- `visitorId`: identificador del usuario.  
- `date`: fecha del pedido.  
- `revenue`: ingreso generado por el pedido.  
- `group`: grupo del test A/B.

### 3. `visits_us.csv`
Contiene visitas diarias por grupo:  
- `date`: fecha.  
- `group`: grupo del test A/B.  
- `visits`: número de visitas en la fecha especificada.

---

## 🧠 Análisis de Hipótesis: ICE y RICE

### 🔹 Resultados del framework ICE
Las hipótesis con mayor puntuación ICE fueron:  
1. Hipótesis 8 → ICE: 16  
2. Hipótesis 0 → ICE: 13.3  
3. Hipótesis 7 → ICE: 11.2  

### 🔹 Resultados del framework RICE
Las hipótesis con mayor puntuación RICE fueron:  
1. Hipótesis 7 → RICE: 112  
2. Hipótesis 2 → RICE: 56  
3. Hipótesis 0 → RICE: 40  

> La diferencia se debe a que el RICE considera el **alcance (Reach)**, favoreciendo hipótesis que impactan a un mayor número de usuarios. Por ejemplo, la hipótesis 7 afecta a todos los usuarios, aunque su impacto podría no ser positivo para todos (como un formulario de suscripción obligatorio en la página principal).

---

## 📊 Análisis del Test A/B

### 🔹 Ingreso acumulado por grupo
- El **grupo B** presentó un mayor ingreso acumulado que el grupo A.  
- La diferencia se incrementó con el tiempo.

### 🔹 Tamaño promedio de pedido acumulado
- El **grupo B** tuvo un mayor tamaño promedio acumulado durante la mayor parte de la prueba.

### 🔹 Tasa de conversión acumulada
- Inicialmente, el **grupo A** presentó mayor tasa de conversión.  
- A partir del día 5, **grupo B igualó y luego superó** al grupo A en conversión acumulada.

### 🔹 Comportamiento de pedidos por usuario
- El **95% de los visitantes realizaron 2 o menos pedidos** en ambos grupos.  
- El **95% de los pedidos** estuvieron por debajo de:  
  - Grupo A → $280.8  
  - Grupo B → $285.82  

### 🔹 Análisis estadístico
- Diferencia significativa en **tasa de conversión** entre grupo A y B.  
- No hay diferencia significativa en **tamaño promedio de pedido** entre los grupos.  
- Los resultados se mantienen tanto con datos completos como filtrados para anomalías.

---

## 🧩 Conclusiones Finales
- Las hipótesis **0, 7, 8 y 2** mostraron los mejores resultados según ICE y RICE.  
- Aunque la hipótesis 7 tuvo mayor RICE por su alcance total, puede no ser positiva para la conversión; se recomienda enfocarse en las hipótesis 0, 2 y 8.  
- El **grupo B** generó mayor ingreso acumulado y presentó una tasa de conversión superior al grupo A, aunque el tamaño y número de pedidos por usuario fueron similares.  
- La diferencia de ingresos se debe a la **mayor retención** y conversión del grupo B.  
- **Recomendación:** adoptar la **estrategia del grupo B**, ya que fue claramente más efectiva.

---

## 🛠️ Tecnologías y Librerías
- **Python**  
- **Pandas**, **NumPy**  
- **Matplotlib**, **Seaborn**  
- **SciPy (stats)**

---

## 👤 Autor
**Alexis Gerardo Martínez Rangel**  
📍 *TripleTen Data Analyst Program*  
📅 *Proyecto: Priorización de Hipótesis y Test A/B (2025)*
