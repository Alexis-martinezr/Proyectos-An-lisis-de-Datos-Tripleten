# 📡 **Análisis de Ingresos y Comportamiento de Clientes de Megaline**

## 🧩 **Descripción del Proyecto**
Trabajas como analista para el operador de telecomunicaciones **Megaline**.  
La empresa ofrece dos tarifas de prepago —**Surf** y **Ultimate**— y busca determinar **cuál de las dos genera más ingresos** para optimizar su presupuesto de publicidad.

Para ello, se analizaron los datos de **500 clientes**, incluyendo:
- Información demográfica (edad, ciudad, fecha de suscripción).  
- Uso de llamadas, mensajes SMS y tráfico de datos durante 2018.  
- Plan contratado y consumo mensual.

El objetivo es **comprender el comportamiento de los usuarios**, calcular **ingresos promedio y totales** por plan y **probar estadísticamente** si existen diferencias significativas en los ingresos entre planes y regiones.

---

## 💰 **Descripción de las Tarifas**

### 🌊 **Plan Surf**
- Pago mensual: **$20**  
- Incluye: **500 minutos**, **50 SMS**, **15 GB de datos**  
- Costos adicionales:  
  - $0.03 por minuto extra  
  - $0.03 por SMS extra  
  - $10 por GB extra  

### 🚀 **Plan Ultimate**
- Pago mensual: **$70**  
- Incluye: **3000 minutos**, **1000 SMS**, **30 GB de datos**  
- Costos adicionales:  
  - $0.01 por minuto extra  
  - $0.01 por SMS extra  
  - $7 por GB extra  

> 🧮 **Nota:**  
> Megaline redondea los segundos a minutos y los megabytes a gigabytes:
> - Cada llamada se redondea al minuto superior.  
> - El consumo total mensual de datos se redondea al gigabyte superior.

---

## 🗂️ **Diccionario de Datos**

### 👤 **users**
| Campo | Descripción |
|--------|--------------|
| user_id | Identificador único del usuario |
| first_name / last_name | Nombre y apellido |
| age | Edad del usuario |
| reg_date / churn_date | Fecha de alta y baja del servicio |
| city | Ciudad del usuario |
| plan | Plan contratado |

### 📞 **calls**
| Campo | Descripción |
|--------|--------------|
| id | Identificador de la llamada |
| call_date | Fecha de la llamada |
| duration | Duración (en minutos) |
| user_id | Usuario que realizó la llamada |

### 💬 **messages**
| Campo | Descripción |
|--------|--------------|
| id | Identificador del SMS |
| message_date | Fecha del SMS |
| user_id | Usuario que envió el SMS |

### 🌐 **internet**
| Campo | Descripción |
|--------|--------------|
| id | Identificador de la sesión |
| mb_used | Datos consumidos (en MB) |
| session_date | Fecha de la sesión |
| user_id | Usuario que realizó la conexión |

### 📋 **plans**
| Campo | Descripción |
|--------|--------------|
| plan_name | Nombre del plan |
| usd_monthly_fee | Pago mensual |
| minutes_included | Minutos incluidos |
| messages_included | SMS incluidos |
| mb_per_month_included | Datos incluidos |
| usd_per_minute | Costo por minuto extra |
| usd_per_message | Costo por SMS extra |
| usd_per_gb | Costo por GB extra |

---

## 🧠 **Metodología del Proyecto**

### 📍 **Paso 1. Carga y Exploración Inicial**
Se cargaron los datasets con `pandas` y se revisaron:
- Tipos de datos  
- Valores nulos y duplicados  
- Estructura general de cada tabla  

### ⚙️ **Paso 2. Preparación de los Datos**
- Conversión de tipos de datos (fechas, enteros, floats).  
- Corrección de errores detectados.  
- Cálculo de métricas mensuales por usuario:  
  - Total de **llamadas**, **minutos**, **mensajes** y **datos consumidos**.  
  - **Ingresos mensuales**, considerando los cargos extra según cada plan.

### 📊 **Paso 3. Análisis Exploratorio**
Se analizaron los siguientes aspectos:
- Consumo promedio mensual de minutos, SMS y datos.  
- Distribuciones por plan y medidas estadísticas (**media, varianza, desviación estándar**).  
- Gráficos de distribución e histogramas para comparar comportamientos.

### 🧪 **Paso 4. Pruebas de Hipótesis**
Se evaluaron dos hipótesis principales:

1. **El ingreso promedio de los usuarios de Surf y Ultimate es diferente.**  
2. **El ingreso promedio de los usuarios en el área NY-NJ difiere del resto de las regiones.**

- Se usó un **nivel de significancia α = 0.05**.  
- Se aplicó una **prueba t de Student** para comparar medias entre grupos.  

---

## 📈 **Resultados Principales**

- El **ingreso promedio mensual** fue mayor para el **plan Ultimate**, sin embargo:  
  - El **plan Surf** generó **el doble de ingresos totales**, debido a que **tiene más del doble de usuarios**.  
- El **plan Surf** mostró una **tendencia ascendente de ingresos** a lo largo del año, alcanzando su punto máximo en **diciembre**.  
- El **mayor consumo de minutos, SMS y datos** en el plan Surf generó suficientes **cargos adicionales** para hacerlo casi tan rentable como Ultimate.

---

## 🧩 **Conclusiones**

- Los usuarios de **ambos planes tienen comportamientos de uso similares**, pero los cargos extra en **Surf** aumentan significativamente los ingresos totales.  
- Aunque **Ultimate** presenta un mayor ingreso promedio, la **cantidad de usuarios y cargos adicionales en Surf** lo convierten en el plan más rentable en términos globales.  
- La **prueba de hipótesis** confirmó que los ingresos promedio difieren significativamente entre los planes.  
- También se detectó una diferencia significativa en los ingresos promedio entre los usuarios del área **NY-NJ ($60.9)** y los del resto del país (**$65**).  

> 💡 **Recomendación:**  
> Promocionar el **plan Surf**, ya que su costo más bajo lo hace más atractivo para nuevos clientes, y sus cargos adicionales lo vuelven altamente rentable para la empresa.

---

## 🛠️ **Tecnologías Utilizadas**

- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib / Seaborn**  
- **SciPy (stats)**  
- **Jupyter Notebook**

---

## 👤 **Autor**
**Alexis Gerardo Martínez Rangel**  
📍 *TripleTen Data Analyst Program*  
📅 *Proyecto: Análisis de Tarifas Megaline (2025)*
