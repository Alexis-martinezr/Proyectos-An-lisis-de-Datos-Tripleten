# 🍔 Análisis del Comportamiento de Usuarios en la App de Productos Alimenticios

## 📘 Introducción
Este proyecto analiza el comportamiento de los usuarios en una **empresa emergente de productos alimenticios**, con el objetivo de estudiar cómo los usuarios navegan por la aplicación y cuáles son los pasos más críticos en el **embudo de conversión**.

Se analiza además un **experimento A/A/B** realizado para evaluar si el cambio de fuentes en la app afecta la conducta de los usuarios y sus decisiones de compra.

---

## 🎯 Objetivos del Proyecto
1. Estudiar el embudo de eventos de la aplicación y detectar posibles puntos de fuga.  
2. Calcular la proporción de usuarios que alcanzan la etapa de compra y las etapas donde más usuarios se pierden.  
3. Analizar los resultados del test A/A/B sobre el cambio de fuentes.  
4. Comprobar si hay diferencias estadísticamente significativas entre los grupos de control y el grupo de prueba.  
5. Extraer conclusiones sobre la experiencia de usuario y posibles mejoras.

---

## 📂 Dataset Utilizado
### `logs_exp_us.csv`
Cada fila representa un evento generado por un usuario:  
- **EventName**: nombre del evento realizado.  
- **DeviceIDHash**: identificador único del usuario.  
- **EventTimestamp**: fecha y hora del evento.  
- **ExpId**: número de experimento (246 y 247 = grupos de control, 248 = grupo de prueba).

---

## 🧹 Limpieza y Preparación de Datos
- Se estandarizaron los nombres de columnas y se verificaron tipos de datos.  
- Se agregaron columnas separadas para la **fecha** y la **hora** del evento.  
- Se identificaron los usuarios pertenecientes a los tres grupos experimentales.  
- Se excluyeron eventos anteriores al **01-08-2019** para garantizar consistencia en los datos.  
- Después del filtrado, se conservaron los siguientes registros por grupo:  
  - Grupo 246: 67,844 movimientos de usuario  
  - Grupo 247: 64,811 movimientos de usuario  
  - Grupo 248: 72,412 movimientos de usuario

---

## 🧠 Análisis Exploratorio de Datos

### 🔹 Embudo de Eventos
Se propuso el siguiente orden de eventos en la aplicación:  
1. **Tutorial**  
2. **Main Screen Appear** (Pantalla principal)  
3. **Offers Screen Appear** (Pantalla de ofertas)  
4. **Cart Screen Appear** (Pantalla del carrito)  
5. **Payment Screen Successful** (Pantalla de pago exitosa)

- Solo el **0.79% de los usuarios completó el tutorial**, por lo que la mayoría probablemente lo omitió.  
- La mayor parte de los usuarios se perdió en la **pantalla de ofertas**.  
- Aproximadamente el **29.5% de los usuarios completó todos los pasos hasta la compra**.  
- El filtrado de datos no alteró la distribución general de los eventos.

### 🔹 Observaciones Generales
- La mayoría de los usuarios omite el tutorial, lo cual podría estar influenciado por usuarios recurrentes que ya lo completaron anteriormente.  
- No se observó una diferencia significativa en la proporción de usuarios que completó cada evento entre los tres grupos.  
- El grupo B (248) tuvo más usuarios y, por lo tanto, más ventas concluidas, pero no se pudo determinar una ventaja estadística significativa del cambio de fuentes.

---

## 🧪 Análisis del Experimento A/A/B
- Se compararon los dos grupos de control (246 y 247) para validar la consistencia de la prueba.  
- Se comprobó que **no existen diferencias significativas** entre ambos grupos de control, asegurando que la asignación de usuarios es correcta.  
- Se comparó el grupo de prueba (248) con los grupos de control para cada evento:  
  - No se detectaron diferencias significativas en el comportamiento de los usuarios.  
  - Aunque el grupo de prueba tuvo más usuarios activos y más compras, se requieren más datos para sacar conclusiones firmes.

---

## 🧩 Conclusiones
- El embudo de conversión muestra **puntos críticos de fuga**: principalmente en la pantalla de ofertas.  
- Aproximadamente **1 de cada 3 usuarios completa todo el embudo hasta la compra**.  
- Los resultados del experimento A/A/B sugieren que **el cambio de fuentes no afecta significativamente la conducta de los usuarios**.  
- Para decisiones futuras, se recomienda:  
  - Realizar pruebas con **muestras más grandes y períodos de observación más extensos**.  
  - Analizar el impacto de otros cambios en la interfaz sobre el embudo de conversión.  
  - Considerar **experimentos adicionales** para optimizar la retención y finalización de compra.

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
📅 *Proyecto: Análisis de Comportamiento de Usuarios (2025)*
