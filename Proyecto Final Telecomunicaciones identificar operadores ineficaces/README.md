📞 **Proyecto: Identificación de Operadores Ineficaces — CallMeMaybe**
📘 **Descripción General**

El servicio de telefonía virtual CallMeMaybe busca mejorar su eficiencia operativa al identificar a los operadores con menor rendimiento.
Un operador se considera ineficaz cuando presenta:

- Una alta cantidad de llamadas entrantes perdidas (internas o externas).

- Tiempos de espera prolongados para atender llamadas entrantes.

- Baja cantidad de llamadas salientes, en los casos en que éstas formen parte de sus funciones.

El análisis combina técnicas de exploración de datos, estadística inferencial y clustering para segmentar a los operadores según su desempeño.

🎯 **Objetivos del Proyecto**

1. Analizar el comportamiento de los operadores telefónicos y sus métricas de desempeño.

2. Detectar patrones de ineficiencia en la atención de llamadas.

3. Establecer umbrales de rendimiento basados en datos (en lugar de valores arbitrarios).

4. Probar hipótesis estadísticas que respalden las diferencias observadas.

5. Aplicar técnicas de clustering para clasificar operadores por desempeño.

🧠 **Hipótesis Principal**

Los operadores con una mayor duración promedio de llamadas también presentan tiempos de espera más prolongados.

🧩 **Plan de Trabajo**

1. Preprocesamiento de datos: limpieza, verificación de tipos y eliminación de valores atípicos.

2. Análisis exploratorio (EDA): distribución de llamadas, tiempos de espera y proporción de llamadas perdidas.

3. Cálculo de métricas clave:

4. Duración promedio de llamadas.

5. Tasa de llamadas perdidas.

6. Tiempo promedio de espera.

7. Comparación entre grupos: operadores con alto vs. bajo desempeño.

8. Correlación entre variables: tiempo de espera vs. llamadas perdidas.

9. Clasificación mediante clustering (K-means o jerárquico).

10. Identificación del 10 % de operadores menos eficientes.

11. Conclusiones y recomendaciones.

📊 **Descripción de los Datos**
1. Dataset principal — telecom_dataset_us.csv
- Columna	Descripción
- user_id	ID de la cuenta de cliente
- date	Fecha de registro de estadísticas
- direction	Dirección de llamada (in / out)
- internal	Indica si la llamada fue interna
- operator_id	Identificador del operador
- is_missed_call	Indicador de llamada perdida
- calls_count	Número de llamadas
- call_duration	Duración efectiva de llamada (sin espera)
- total_call_duration	Duración total de llamada (con espera)
- Dataset complementario — telecom_clients_us.csv
- Columna	Descripción
- user_id	ID de cliente
- tariff_plan	Plan tarifario
- date_start	Fecha de registro
📈 **Resultados Principales**
🔹 **Estadísticas generales**

- Promedio de duración efectiva de llamada: 866.7 s

- Promedio de duración total (incluido tiempo de espera): 1157.1 s

- Valores atípicos: llamadas con más de 140 000 s de duración efectiva.

🔹 **Observaciones clave**

1. Los operadores con mayor tiempo de espera también muestran mayor proporción de llamadas perdidas.

2. Se detectaron operadores con 0 días de antigüedad, por lo que se filtraron casos con menos de 15 días de experiencia.

El análisis se normalizó para evitar sesgos derivados del tiempo laborado.

🔹 **Resultados del clustering**

- No se obtuvo el patrón esperado (operadores con altas tasas de pérdida y largos tiempos de espera).

- Se identificó un grupo con baja actividad y bajos tiempos de espera, posiblemente operadores con funciones administrativas o de supervisión.

Se requiere información adicional sobre roles para confirmar esta hipótesis.

🔹 **Identificación de operadores ineficaces**

- Top 10 % con mayor tiempo de espera: 47 operadores

- Top 10 % con mayor tasa de pérdida de llamadas: 47 operadores

- Coincidencia en ambas métricas: 29 operadores

Los operadores en el top 10 % mostraron:

- Tasa media de pérdida de llamadas: 0.514

- Tiempo medio de espera: 703 s
En comparación, el resto presentó:

- Tasa media de pérdida: 0.30

- Tiempo medio de espera: 258.5 s

🧾 **Conclusiones**

1. Se logró identificar el 10 % de operadores con peor desempeño.

2. El clustering sugiere la existencia de roles mixtos dentro del dataset (operativos vs. administrativos).

3. Los operadores con mayor tiempo de espera también presentan mayor proporción de llamadas perdidas, validando parcialmente la hipótesis.

4. Se recomienda implementar métricas internas de rendimiento y mantener una clasificación por tipo de puesto para futuras evaluaciones.


💻 **Tecnologías Utilizadas**

- Python 3.11:

  Pandas, NumPy

  Matplotlib, Seaborn

  Scikit-learn  
