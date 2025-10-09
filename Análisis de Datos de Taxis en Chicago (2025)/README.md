# 🚖 **Análisis de Datos de Taxis en Chicago**

## 📘 **Introducción**
Este proyecto analiza datos históricos de viajes en taxi en la ciudad de **Chicago (EE. UU.)**, con el objetivo de identificar patrones de transporte urbano, las compañías más activas y los barrios con mayor número de llegadas.  

Además, se realiza una **prueba estadística** para determinar si las condiciones climáticas —específicamente los sábados lluviosos— influyen en la duración promedio de los viajes desde el **Loop** hasta el **Aeropuerto Internacional O'Hare**.

---

## 🎯 **Objetivos del Proyecto**

1. Analizar la actividad de las principales compañías de taxis.  
2. Identificar los barrios con mayor número de viajes finalizados.  
3. Visualizar los resultados mediante gráficos.  
4. Probar la hipótesis sobre el efecto de la lluvia en la duración de los viajes al aeropuerto.  
5. Desarrollar conclusiones basadas en los resultados estadísticos.

---

## 📂 **Datasets Utilizados**

### 🗃️ `project_sql_result_01.csv`
Contiene información sobre las empresas de taxis y la cantidad de viajes realizados:

- **company_name** → Nombre de la empresa de taxis  
- **trips_amount** → Número de viajes realizados los días *15 y 16 de noviembre de 2017*

---

### 🗃️ `project_sql_result_04.csv`
Contiene información sobre las zonas donde finalizan los viajes:

- **dropoff_location_name** → Barrio donde finalizó el viaje  
- **average_trips** → Promedio de viajes que terminaron en ese barrio durante *noviembre de 2017*

---

### 🗃️ `project_sql_result_07.csv`
Contiene información sobre viajes desde el **Loop** hacia el **Aeropuerto O’Hare**:

- **start_ts** → Fecha y hora del inicio del viaje  
- **weather_conditions** → Condiciones climáticas en el momento del viaje  
- **duration_seconds** → Duración del viaje en segundos

---

## 🧠 **Análisis Exploratorio de Datos (EDA)**

### 🔹 **Importación y Limpieza**
- Se cargaron los datasets en **Python** usando `pandas`.  
- Se revisaron tipos de datos, valores nulos y duplicados.  
- Se ajustaron formatos para garantizar la coherencia en el análisis.

---

### 🔹 **Resultados del Análisis**

#### 🚕 **Empresas de Taxis**
Las compañías con mayor número de viajes fueron:

1. **Flash Cab**  
2. **Taxi Affiliation Service**  
3. **Medallion Leasing**

> Estas diferencias pueden deberse al tamaño de las flotas, tarifas o calificaciones del público. Se requeriría información adicional para confirmar estas causas.

---

#### 🗺️ **Barrios con Mayor Número de Viajes Finalizados**
Los barrios con más llegadas fueron:

1. **Loop**  
2. **River North**  
3. **Streeterville**  
4. **West Loop**

> Esto puede estar influido por el tamaño, densidad poblacional o nivel socioeconómico de cada barrio.

---

### 📊 **Visualizaciones Realizadas**
- Gráfico de barras: **Empresas vs. número de viajes**  
- Gráfico de barras: **Top 10 barrios por promedio de finalización de viajes**

---

## 🧪 **Prueba de Hipótesis**

### 📍 **Hipótesis Planteadas**

- **H₀ (nula):** La duración promedio de los viajes desde el Loop hasta el aeropuerto **no cambia** los sábados lluviosos.  
- **H₁ (alternativa):** La duración promedio de los viajes **sí cambia** los sábados lluviosos.

---

### ⚙️ **Nivel de Significancia**
Se utilizó un nivel de **α = 0.05**.

---

### 🧮 **Método Estadístico**
Se aplicó una **prueba t de Student para muestras independientes**, ya que se comparan los tiempos promedio de dos grupos:  
- *Viajes en sábados lluviosos*  
- *Viajes en otros días*

---

### 📈 **Resultados**
- **Duración promedio sábados lluviosos:** ≈ *2427 segundos*  
- **Duración promedio otros días:** ≈ *1999.6 segundos*  
- **Conclusión:** Se **rechazó la hipótesis nula**.

> Esto indica que los sábados lluviosos presentan un aumento significativo en la duración del viaje, probablemente por tráfico o condiciones climáticas adversas.

---

## 🧩 **Conclusiones**

- **Flash Cab** fue la empresa con mayor volumen de viajes.  
- Los barrios **Loop** y **River North** concentraron la mayoría de las llegadas.  
- Se confirmó que los **sábados lluviosos** aumentan el tiempo promedio de los viajes desde el Loop hasta O’Hare.  
- Se recomienda ampliar el estudio con:
  - Datos de otras fechas o estaciones del año.  
  - Información sobre tarifas, calificaciones o tamaño de flota.  
  - Comparaciones entre distintos climas y zonas.

---

## 🛠️ **Tecnologías y Librerías Utilizadas**

- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib**  
- **Seaborn**  
- **SciPy (stats)**

---

## 👤 **Autor**

**Alexis Gerardo Martínez Rangel**  
📍 *TripleTen Data Analyst Program*  
📅 *Proyecto: Análisis de Datos de Taxis en Chicago (2025)*  
