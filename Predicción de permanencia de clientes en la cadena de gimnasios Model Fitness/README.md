🏋️ **Predicción de Permanencia de Clientes – Model Fitness**

Este proyecto analiza la retención de clientes de la cadena de gimnasios Model Fitness, utilizando datos de perfiles y comportamiento de los usuarios para predecir abandonos y generar estrategias de retención.

El objetivo principal es identificar patrones que indiquen la probabilidad de que un cliente abandone el gimnasio y proponer estrategias para reducir la pérdida de usuarios.

📘 **Descripción del Proyecto**

La pérdida de clientes es un problema común en gimnasios y servicios de suscripción.

Se define que un cliente ha abandonado si no asiste al gimnasio durante un mes.

El análisis se basa en datos digitalizados de perfiles de clientes, visitas, contratos y participación en actividades grupales.

🔍 **Análisis Exploratorio de Datos (EDA)**

- Conclusiones Parte 1:

1. Los clientes que permanecen más tiempo suelen vivir o trabajar cerca del gimnasio, estar asociados a empresas con descuentos o haber ingresado con promociones de amigos.

2. Pagaban contratos más largos, participaban en sesiones grupales con mayor frecuencia y tenían mayor antigüedad en el gimnasio.

3. Los clientes que abandonan tienden a visitar menos, tener contratos más cortos y menor participación en actividades grupales.

🛠️ **Construcción del Modelo**

Predicción de usuarios que abandonarán el próximo mes:

Se construyeron modelos para predecir clientes con alta probabilidad de abandono.

- Conclusión Parte 2: Aproximadamente 41 usuarios se espera que abandonen si las características se mantienen constantes.

📊 **Segmentación de Clientes (Clustering)**

- Conclusión Parte 3:

Se dividieron los usuarios en 5 clusters según su comportamiento:

1. Clusters 4 y 0: mayor riesgo de abandono; menor frecuencia de visitas, menor antigüedad y contratos más cortos.

2. Clusters 2 y 3: menor riesgo de abandono; visitas frecuentes, mayor antigüedad y contratos más largos.

Estas segmentaciones permiten orientar estrategias de retención personalizadas.

🎯 **Conclusiones Finales**

1. Promociones para nuevos usuarios (ingreso con amigos o contratos más largos) podrían aumentar la retención.

2. Mantener a los usuarios activos más de 4–5 meses ayuda a formar hábitos de entrenamiento y mejorar motivación, reduciendo la probabilidad de abandono.

3. Se recomienda descuentos por pronto pago para miembros con membresías próximas a vencer.

🛠️ **Tecnologías Utilizadas**

- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)

- Jupyter Notebook
