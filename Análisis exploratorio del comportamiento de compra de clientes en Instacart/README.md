🛒 **Análisis de Datos de Pedidos de Instacart**

Este proyecto consiste en un análisis exploratorio de datos (EDA) sobre un conjunto de datos de la plataforma de entregas de comestibles Instacart, con el objetivo de identificar patrones de compra, preferencias de los usuarios y comportamiento de reordenamiento de productos.

El dataset proporcionado es una versión modificada del original, con reducción de tamaño, valores ausentes y duplicados, pero manteniendo las distribuciones originales para un análisis representativo.

📘 **Objetivos del Proyecto**

1. Leer y explorar los datos: cargar los CSV proporcionados y verificar su contenido, tipos de datos y valores faltantes.

2. Analizar el comportamiento de los usuarios: evaluar patrones de reordenamiento, frecuencia de pedidos, horarios y días de mayor actividad.

3. Identificar preferencias de productos: determinar los productos y categorías más populares, así como tendencias de compra por departamento y pasillo.

🗂️ **Diccionario de Datos**

El conjunto de datos contiene cinco tablas principales:

1. **instacart_orders.csv**
Cada fila corresponde a un pedido.

- order_id: ID único de pedido

- user_id: ID único de cliente

- order_number: número de pedido del cliente

- order_dow: día de la semana (0 = domingo)

- order_hour_of_day: hora del pedido

- days_since_prior_order: días desde el pedido anterior

2. **products.csv**
Cada fila corresponde a un producto.

- product_id: ID único de producto

- product_name: nombre del producto

- aisle_id: ID de la categoría de pasillo

- department_id: ID del departamento

3. **order_products.csv**
Cada fila corresponde a un artículo en un pedido.

- order_id: ID del pedido

- product_id: ID del producto

- add_to_cart_order: orden en que se añadió al carrito

- reordered: 0 = primer pedido del producto, 1 = reorden

4. **aisles.csv**

- aisle_id: ID único del pasillo

- aisle: nombre del pasillo

5. **departments.csv**

- department_id: ID único del departamento

- department: nombre del departamento

📊 **Conclusiones Generales**

- Los usuarios presentan una clara preferencia por artículos orgánicos, evidenciado por la alta tasa de reordenamiento.

- Se observa un ligero incremento en pedidos los sábados y lunes, con los horarios más activos entre 10:00 am y 3:00 pm.

- La mayoría de los usuarios compran entre 1 y 10 artículos por pedido, con un pico entre 3 y 5 artículos.

- Un gran número de usuarios realiza nuevos pedidos 30 días después del anterior, pero también hay picos en 0 días o 7 días, probablemente debido a compras semanales regulares.

🛠️ **Tecnologías Utilizadas**

- Python (pandas, numpy, matplotlib, seaborn)

- Jupyter Notebook
