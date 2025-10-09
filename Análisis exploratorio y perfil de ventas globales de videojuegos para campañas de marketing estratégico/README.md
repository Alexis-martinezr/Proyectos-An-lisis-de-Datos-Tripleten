**<h1>**🎮 **Análisis de Ventas de Videojuegos – Predicción de Éxito y Tendencias del Mercado****</h1>**

Este proyecto analiza datos históricos de ventas de videojuegos para identificar patrones que permitan predecir el éxito comercial de un título y planificar campañas publicitarias más efectivas.

📘 **Descripción del Proyecto**

**Objetivo principal:**
1. Detectar plataformas y géneros con mayor potencial de ventas.

2. Analizar el impacto de las reseñas de usuarios y críticos, así como la clasificación ESRB.

3. Identificar tendencias de mercado y ciclos de vida de las consolas.

4. Comparar patrones de consumo entre distintas regiones.

**Información analizada:**

- Ventas por región (Norteamérica, Europa, Japón y resto del mundo).

- Plataforma y género del juego.

- Año de lanzamiento.

- Calificaciones de usuarios y críticos.

- Clasificación ESRB.

El estudio se desarrolla con datos hasta 2016, simulando la planificación de campañas de marketing para el año 2017.

🧩 **Metodología**

1. Preparación y limpieza de datos para garantizar consistencia en formatos, tipos y valores.

2. Análisis exploratorio (EDA) para identificar tendencias históricas y ciclos de vida de las consolas.

3. Selección de periodo relevante (2014–2016) como base para pronósticos de ventas.

4. Segmentación por región para detectar preferencias locales.

5. Pruebas de hipótesis para comparar diferencias significativas entre géneros y plataformas.

6. Visualización de datos mediante gráficos de distribución, correlaciones y diagramas de caja.

📊 **Resultados Principales**

**Tendencia general:**
Desde 1980 se observó un incremento constante en el número de juegos lanzados, con un estancamiento entre 2009–2010 y una caída posterior.
Este descenso no se relaciona con una menor cantidad de consolas, ya que el número de plataformas activas se mantuvo alto entre 2007 y 2016.

**Ventas por consola:**
A pesar del descenso global en ventas, la PS4 se mantuvo como la consola más exitosa, seguida de Xbox One.

**Correlación entre calificaciones y ventas:**

- critic_score y user_score mostraron una correlación media entre sí.

- La correlación con las ventas fue baja, especialmente en user_score (≈ 0.005), lo que indica que las reseñas no son un predictor confiable del éxito comercial.

- La critic_score tuvo una correlación ligeramente mayor (≈ 0.32).

**Distribución por género:**

1. El género Acción fue el más lanzado entre 2014–2016, seguido de Rol, Aventura, Deportes y Shooter.

2. Sin embargo, al analizar la relación ventas/juegos lanzados, los Shooters y Deportes resultaron más rentables.

3. Por región:

- Japón: predomina el género Rol, seguido de Acción.

- Europa: destacan Acción, Shooter y Deportes.

- EE.UU.: los Shooters lideran, seguidos de Acción y Deportes.

- Resto del mundo: preferencia por Acción y Shooter.

🧠 **Conclusiones**

1. Se seleccionaron los años 2014–2016 como periodo base por reflejar un cambio en las tendencias de ventas y lanzamientos.

2. El género Acción domina en número de lanzamientos y ventas totales, aunque enfrenta alta competencia.

3. Los Shooters muestran la mejor relación ventas/juegos lanzados, lo que los convierte en un segmento atractivo y rentable.

4. Las calificaciones de usuarios y críticos no son un indicador fuerte de ventas, por lo que las estrategias de marketing deben centrarse más en género, plataforma y región.

🛠️ **Tecnologías Utilizadas**

- Python:

  pandas, numpy – Limpieza y manipulación de datos

  matplotlib, seaborn – Visualización de tendencias

  scipy.stats – Pruebas de hipótesis

- Jupyter Notebook
