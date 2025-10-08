🧪 **Prueba A/B – Sistema de Recomendaciones**

Este proyecto analiza los resultados de una prueba A/B realizada en una tienda en línea internacional, con el objetivo de evaluar la eficacia de un nuevo sistema de recomendaciones en la conversión de los usuarios.

Se busca comparar el comportamiento de los usuarios en dos grupos: A (control) y B (nuevo embudo de pago), midiendo su interacción en diferentes etapas del embudo de compra: vistas de productos, adición al carrito y compras.

📘 **Descripción del Proyecto**

- Nombre de la prueba: recommender_system_test

- Grupos: A (control), B (nuevo embudo de pago)

- Fecha de inicio: 07-12-2020

- Fecha de fin: 01-01-2021

- Audiencia: 15% de nuevos usuarios en la región UE

*Objetivo:* Evaluar si el nuevo sistema de recomendaciones incrementa al menos un 10% los eventos product_page → product_card → purchase en 14 días posteriores a la inscripción.

**Número previsto de participantes: 6,000**

**Datasets utilizados:**

- ab_project_marketing_events_us.csv – Calendario de eventos de marketing.

- final_ab_new_users_upd_us.csv – Datos de usuarios nuevos registrados entre 7 y 21 de diciembre de 2020.

- final_ab_events_upd_us.csv – Eventos de los usuarios en el período de prueba.

- final_ab_participants_upd_us.csv – Información sobre el grupo de prueba asignado a cada usuario.

🔍 **Análisis Exploratorio de Datos (EDA)**

Hallazgos principales:

- Se identificaron usuarios presentes en ambos grupos, lo que puede generar sesgos.

- El grupo A es ~1/3 más grande que el grupo B, con casi 1,900 usuarios adicionales.

- Picos en el número de eventos se observaron los días 12 y 21 de diciembre, seguido de una caída hasta el día 29.

- Se detectaron anomalías en los eventos: en el grupo A hay más compras que adiciones al carrito, algo imposible según la lógica del embudo.

- La fecha de la prueba coincide con días festivos, lo que podría afectar la interpretación de los resultados.

📊 **Evaluación de la Prueba A/B**

Tras realizar pruebas estadísticas (z-test) por proporciones, a primera vista, el grupo A mostró mejor retención, especialmente en usuarios con iPhone.

Sin embargo, errores en la implementación, como usuarios duplicados, tamaños de grupo desbalanceados y fechas inapropiadas, impiden considerar los resultados confiables.

Posibles causas de anomalías: usuarios que iniciaron eventos en un grupo y los completaron en otro, o realizaron acciones en distintos dispositivos.

🎯 **Conclusiones Finales**

1. Aunque el grupo A parece mostrar mejores métricas, estas no pueden atribuirse al sistema de recomendaciones, debido a los errores de segmentación y ejecución de la prueba.

2. La prueba no puede considerarse confiable para tomar decisiones comerciales.

3. Recomendaciones: realizar una nueva prueba con segmentación correcta, grupos equilibrados, y evitando periodos festivos o factores externos que puedan sesgar los resultados.

🛠️ **Tecnologías Utilizadas**

- Python (pandas, numpy, matplotlib, seaborn, scipy)

- Jupyter Notebook
