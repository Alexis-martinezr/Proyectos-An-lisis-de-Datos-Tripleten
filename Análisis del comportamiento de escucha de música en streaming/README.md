# 🎵 Déjame escuchar la música

## 📘 Introducción
Este proyecto tiene como propósito analizar las **preferencias musicales** de usuarios en las ciudades de **Springfield** y **Shelbyville**, con el objetivo de comprender si la actividad de los oyentes difiere según el **día de la semana** y la **ubicación geográfica**.  

El análisis incluye la **preparación y limpieza de datos**, el **procesamiento de información** y la **prueba de hipótesis** basada en datos reales de reproducción musical en línea.

---

## 🎯 Objetivos del Proyecto

1. Analizar el comportamiento de los usuarios de música en dos ciudades distintas.  
2. Evaluar las diferencias de actividad musical según el día de la semana.  
3. Limpiar y preparar los datos para garantizar su calidad.  
4. Comprobar una hipótesis sobre las diferencias de comportamiento entre ciudades.  
5. Elaborar conclusiones basadas en los resultados obtenidos.

---

## 📂 Dataset Utilizado

### `music_project_en.csv`
Contiene información sobre los hábitos de escucha de música en línea, con las siguientes columnas:

- **userID**: Identificador del usuario o la usuaria.  
- **Track**: Título de la canción.  
- **artist**: Nombre del artista.  
- **genre**: Género musical.  
- **City**: Ciudad del usuario o la usuaria.  
- **time**: Hora exacta en que se reprodujo la canción.  
- **Day**: Día de la semana.

---

## 🧹 Limpieza y Preparación de Datos

Durante esta fase se realizaron las siguientes acciones:

- **Revisión y corrección de encabezados**: se detectaron inconsistencias en mayúsculas/minúsculas, espacios innecesarios y errores de formato como `userID` (ajustado a `user_id`).  
- **Tratamiento de valores ausentes y duplicados** para asegurar la calidad del conjunto de datos.  
- **Estandarización de tipos de datos** y normalización de textos.  

---

## 🧠 Análisis Exploratorio de Datos (EDA)

Se evaluó el número de canciones reproducidas por ciudad y día de la semana.

### 🔹 Hipótesis planteada

- **H₀ (nula):** La actividad de los usuarios no difiere según el día de la semana o la ciudad.  
- **H₁ (alternativa):** La actividad de los usuarios **sí difiere** según el día de la semana o la ciudad.

Para comprobarlo, se analizaron los datos agrupados por **ciudad** y **día de la semana**, contando el número de canciones reproducidas 
---

## 📊 Resultados y Conclusiones

Los usuarios de Springfield escuchan más música los lunes y viernes, mientras que los de Shelbyville prefieren los miércoles.
Se identificaron patrones de consumo similares entre ambas ciudades los lunes y viernes.
Estas tendencias reflejan diferencias locales en los hábitos musicales, posiblemente influenciadas por factores demográficos o culturales.

La hipótesis se considera parcialmente correcta: existen diferencias entre ciudades, pero también coincidencias en ciertos días de la semana.
Los resultados muestran que Shelbyville tiene picos de consumo los miércoles, mientras que Springfield concentra su actividad los lunes y viernes.
Aunque los datos reflejan comportamientos distintos, sería necesario profundizar con un análisis estadístico formal y una muestra más amplia para confirmar la validez de estas observaciones.

Este estudio demuestra cómo el análisis exploratorio de datos puede ofrecer una primera aproximación útil para comprender las diferencias de comportamiento entre grupos.

### 🛠️ Tecnologías y Librerías

- Python

- Pandas, NumPy

- Matplotlib, Seaborn

### 👤 Autor

Alexis Gerardo Martínez Rangel
📍 TripleTen Data Analyst Program
📅 Proyecto: Déjame escuchar la música (2025)
