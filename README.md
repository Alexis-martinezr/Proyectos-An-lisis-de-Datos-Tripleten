# 📊 Portafolio de Proyectos de Análisis de Datos – TripleTen

Este repositorio reúne los **proyectos de análisis de datos** que he realizado como parte del programa **TripleTen Data Analyst**, incluyendo **análisis exploratorios, pruebas A/B, priorización de hipótesis y estudios de comportamiento de usuarios** en aplicaciones, plataformas de música y tiendas online.

Cada proyecto muestra el **flujo completo de trabajo**: descripción de los datos, preprocesamiento, análisis, visualización y conclusiones.

---

## 📂 Proyectos Incluidos

### 1️⃣ Déjame Escuchar la Música
**Carpeta:** `music_streaming_analysis`  
**Descripción:** Análisis de hábitos de consumo musical en Springfield y Shelbyville.  
**Técnicas:** Agrupamiento de datos, conteo de reproducciones, filtrado por ciudad y día.  
**Resultados y Observaciones:** Springfield más activo lunes y viernes; Shelbyville más activo miércoles; patrones similares lunes y viernes.  
**Conclusiones:** Diferencias y coincidencias entre ciudades; se recomienda análisis estadístico más profundo para confirmar tendencias.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn

---

### 2️⃣ Análisis de Embudo de Ventas y Test A/A/B – Productos Alimenticios
**Carpeta:** `sales_funnel_aa_b_test`  
**Descripción:** Estudio del comportamiento de usuarios en una app de productos alimenticios, embudo de ventas y test A/A/B sobre diseño de fuentes.  
**Técnicas:** Preprocesamiento de logs, filtrado, análisis de embudo, test estadístico entre grupos.  
**Resultados y Observaciones:** La mayoría de los usuarios se pierden en la pantalla de ofertas; solo 29.5% completó todos los pasos hasta la compra. No se observaron diferencias significativas entre grupos de control y prueba.  
**Conclusiones:** Diseño de fuentes no afectó el comportamiento; se necesita más data para conclusiones robustas.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn

---

### 3️⃣ Priorización de Hipótesis y Test A/B – Tienda Online
**Carpeta:** `hypotheses_ab_test`  
**Descripción:** Priorización de hipótesis para aumentar ingresos y análisis de test A/B.  
**Técnicas:** Frameworks ICE y RICE, métricas acumuladas, tasa de conversión, outliers, pruebas estadísticas.  
**Resultados y Observaciones:**  
- Hipótesis 0, 7, 8 y 2 mostraron mejores scores ICE y RICE.  
- Grupo B tuvo mayor ingreso acumulado y tasa de conversión; tamaño promedio de pedido similar.  
**Conclusiones:** Adoptar estrategia B basada en retención y conversión; priorizar hipótesis de alto impacto y bajo esfuerzo.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy

---

### 4️⃣ Análisis de Datos de Taxis en Chicago
**Carpeta:** `chicago_taxi_analysis`  
**Descripción:** Análisis histórico de viajes en taxi para identificar patrones, compañías activas y barrios con más llegadas.  
**Técnicas:** Limpieza de datos, visualización, prueba t de Student.  
**Resultados y Observaciones:** Flash Cab más activa; barrios Loop y River North con mayor tráfico; la lluvia los sábados aumenta duración de viajes hacia O’Hare.  
**Conclusiones:** Mejorar planificación según clima y horarios pico.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy

---

### 5️⃣ Análisis de Comportamiento Musical – Extendido
**Carpeta:** `music_behavior_extended`  
**Descripción:** Profundización en hábitos musicales por ciudad y día.  
**Técnicas:** Agrupamiento múltiple, tendencias y visualización de frecuencias.  
**Resultados y Observaciones:** Springfield lunes/viernes, Shelbyville miércoles; patrones similares lunes/viernes.  
**Conclusiones:** Útil para recomendaciones y marketing personalizado.  
**Tecnologías:** Python, Pandas, Matplotlib, Seaborn

---

### 6️⃣ Análisis de Embudos de Eventos y Conversión – Apps de Consumo
**Carpeta:** `event_funnel_analysis`  
**Descripción:** Estudio del flujo de usuarios en etapas de interacción con la app.  
**Técnicas:** Conteo de eventos, proporciones de usuarios entre etapas, identificación de pérdidas críticas.  
**Resultados y Observaciones:** Mayor pérdida en pantalla de ofertas; tutorial completado solo por 0.79 de usuarios.  
**Conclusiones:** Optimizar pantallas críticas para reducir abandono.  
**Tecnologías:** Python, Pandas, Matplotlib, Seaborn

---

### 7️⃣ Test A/A/B Detallado – Validación de Experimentos
**Carpeta:** `aa_b_test_validation`  
**Descripción:** Validación de diseño experimental con dos grupos de control y un grupo de prueba.  
**Técnicas:** Comparación de proporciones de eventos, significancia estadística entre grupos, análisis de retención.  
**Resultados y Observaciones:** No hay diferencias significativas entre grupos de control; grupo B con mayores ventas por mayor número de usuarios.  
**Conclusiones:** Experimento confiable; diseño de fuentes no afecta conducta de usuario.  
**Tecnologías:** Python, Pandas, NumPy, SciPy

---

### 8️⃣ Priorización RICE vs ICE – Hipótesis de Tienda Online
**Carpeta:** `rice_vs_ice_prioritization`  
**Descripción:** Comparación de frameworks ICE y RICE para priorizar hipótesis sobre incremento de ingresos.  
**Técnicas:** Cálculo de puntuaciones ICE y RICE, análisis de impacto vs esfuerzo vs alcance.  
**Resultados y Observaciones:** Hipótesis 7 tuvo mayor RICE debido al alcance, aunque su impacto podría ser percibido como negativo por usuarios.  
**Conclusiones:** Priorizar hipótesis con alto ICE y RICE, considerando riesgos y experiencia de usuario.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib

---

### 9️⃣ Análisis de Conversión y Retención de Usuarios
**Carpeta:** `conversion_retention_analysis`  
**Descripción:** Estudio de tasas de conversión y retención por grupo de prueba.  
**Técnicas:** Visualización acumulativa de ingresos y conversión, outliers, percentiles, pruebas estadísticas.  
**Resultados y Observaciones:** Grupo B mayor ingreso y retención; tamaño de pedidos similar entre grupos.  
**Conclusiones:** Adoptar estrategia B; optimizar retención.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy

---

### 1️⃣0️⃣ Test A/B – Visualización y Métricas
**Carpeta:** `ab_test_metrics`  
**Descripción:** Evaluación de ingresos, tamaño de pedido y conversión en test A/B.  
**Técnicas:** Gráficos acumulativos, dispersión, percentiles, filtrado de datos anómalos, significancia estadística.  
**Resultados y Observaciones:** Ingreso y conversión mayores en grupo B; no hay diferencia en tamaño de pedido.  
**Conclusiones:** Confirmación de la estrategia B como ganadora.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy

---

### 1️⃣1️⃣ Análisis Global de Proyectos TripleTen
**Carpeta:** `tripleten_global_analysis`  
**Descripción:** Resumen de los 10 proyectos anteriores, integrando conclusiones, patrones y resultados de experimentos.  
**Técnicas:** Integración de resultados, comparación de métricas y aprendizaje general de los experimentos.  
**Conclusiones:** Los proyectos muestran la importancia de la retención, priorización de hipótesis y análisis estadístico robusto en la toma de decisiones basadas en datos.  
**Tecnologías:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy

---

## 🛠️ Tecnologías utilizadas en todos los proyectos

- **Python**  
- **Pandas, NumPy**  
- **Matplotlib, Seaborn**  
- **SciPy**  
- **Jupyter Notebook**  
- **Git / GitHub**

---

## 🚀 Próximos pasos

- Validar hipótesis y experimentos con datasets adicionales.  
- Explorar técnicas de machine learning avanzadas para predicción de comportamiento de usuarios.  
- Mejorar visualizaciones y documentación en cada proyecto.  
- Integrar métricas de negocio para medir impacto real de cada estrategia.
