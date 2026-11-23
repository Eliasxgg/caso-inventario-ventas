# Recorrido visual de QUANTY

Capturas reales del laboratorio local del **22/11/2026**, con una tienda y datos completamente ficticios. Documentan una secuencia: las primeras vistas tienen 24 productos; después del alta manual hay 25. Las capturas extensas de reportes muestran encabezados, gráficos y primeras filas; no necesariamente toda la tabla. No se alteraron cifras ni se dibujaron gráficos sobre las imágenes.

## Acceso y cuenta

<details>
<summary>Portada del proyecto</summary>

Presentación académica de la propuesta y acceso a la aplicación.

![Portada del proyecto](img/01-portada.jpg)

</details>

<details>
<summary>Inicio de sesión</summary>

Formulario de acceso, sin contraseña ni correo introducidos.

![Inicio de sesión](img/02-login.jpg)

</details>

<details>
<summary>Registro de una cuenta</summary>

Formulario disponible para crear una cuenta. Esta imagen documenta el formulario; el registro se verifica también en pruebas automatizadas.

![Registro de una cuenta](img/31-registro.jpg)

</details>

<details>
<summary>Perfil de demostración</summary>

Datos de una cuenta ficticia y opciones de gestión del perfil; los campos de contraseña están vacíos.

![Perfil de demostración](img/32-perfil-demo.jpg)

</details>

## Operación diaria e inventario

<details>
<summary>Panel de indicadores y alertas</summary>

Estado final de la demostración: $52.15 en seis ventas del día, $816.20 en el mes, 25 productos y un producto agotado. La alerta de stock bajo cuenta lotes, incluidos lotes ya agotados; no equivale al número de productos críticos.

![Panel de indicadores y alertas](img/03-dashboard.jpg)

</details>

<details>
<summary>Categorías del catálogo</summary>

Seis grupos para organizar el inventario: bebidas, abarrotes, snacks, limpieza, cuidado personal y lácteos.

![Categorías del catálogo](img/14-categorias.jpg)

</details>

<details>
<summary>Alta de categoría</summary>

Formulario de nombre e icono. En esta captura no se envió una categoría adicional.

![Alta de categoría](img/15-formulario-categoria.jpg)

</details>

<details>
<summary>Catálogo inicial</summary>

24 productos de la población histórica, antes de crear la granola desde la interfaz. Muestra categoría, existencias, precio y estado.

![Catálogo inicial](img/04-productos.jpg)

</details>

<details>
<summary>Preparar un nuevo producto</summary>

Se completa Granola artesanal 300 g en Snacks. El precio y las existencias se asignan mediante una entrada posterior.

![Preparar un nuevo producto](img/05-nuevo-producto.jpg)

</details>

<details>
<summary>Producto creado, antes de recibir stock</summary>

El producto existe, todavía con cero existencias y sin precio: es el paso previo del recorrido, no un fallo.

![Producto creado, antes de recibir stock](img/06-producto-creado.jpg)

</details>

<details>
<summary>Formulario de edición</summary>

Se recuperan nombre, categoría, estado y detalles del producto. Captura del formulario, sin una modificación adicional.

![Formulario de edición](img/28-editar-producto.jpg)

</details>

<details>
<summary>Historial inicial de lotes</summary>

Entradas históricas con cantidad original y disponible, compra, venta y vencimiento.

![Historial inicial de lotes](img/07-entradas.jpg)

</details>

<details>
<summary>Registrar una entrada</summary>

Granola: 30 unidades, costo $1.20 y precio $2.00, con fecha de vencimiento. Formulario completado antes de guardar.

![Registrar una entrada](img/08-nueva-entrada.jpg)

</details>

<details>
<summary>Entrada confirmada</summary>

La aplicación confirma el ingreso y muestra el lote nuevo con 30 unidades.

![Entrada confirmada](img/09-entrada-registrada.jpg)

</details>

<details>
<summary>Detalle editable del lote</summary>

Después de vender, el mismo lote mantiene 30 unidades iniciales y 28 disponibles. Se ve el vencimiento y ambos precios.

![Detalle editable del lote](img/29-editar-lote.jpg)

</details>

## Venta completa y actualización de stock

<details>
<summary>Seleccionar producto y cantidad</summary>

El formulario obtiene desde la base el precio $2.00 y las 30 unidades disponibles de granola.

![Seleccionar producto y cantidad](img/10-seleccionar-producto-venta.jpg)

</details>

<details>
<summary>Preparar una venta con dos productos</summary>

Dos granolas a $2.00 más tres aguas a $0.60: total $5.80. La cesta está preparada antes de registrar.

![Preparar una venta con dos productos](img/11-venta-lista.jpg)

</details>

<details>
<summary>Venta confirmada</summary>

Mensaje de confirmación y nueva operación en el listado. El historial de esta cuenta pasa de 294 a 295 ventas.

![Venta confirmada](img/12-venta-registrada.jpg)

</details>

<details>
<summary>Comprobante interno de la venta</summary>

Detalle por producto, cantidades y subtotales de $4.00 y $1.80. Es un registro interno académico, no un documento tributario.

![Comprobante interno de la venta](img/13-detalle-venta.jpg)

</details>

<details>
<summary>Existencias después de vender</summary>

La granola queda con 28 unidades: 30 ingresadas menos dos vendidas. El historial del producto conserva la entrada.

![Existencias después de vender](img/27-producto-despues-venta.jpg)

</details>

<details>
<summary>Buscar una venta específica</summary>

Filtro por el ID de la operación registrada en este recorrido. Los KPI superiores describen el historial completo; la tabla muestra el filtro.

![Buscar una venta específica](img/30-filtros-ventas.jpg)

</details>

<details>
<summary>Producto agotado</summary>

Seleccionar aceite sin existencias muestra la alerta y deshabilita Agregar producto en la interfaz. No es por sí sola una prueba de todas las validaciones del servidor.

![Producto agotado](img/34-alerta-sin-stock.jpg)

</details>

## Reportes, gráficos e indicadores

<details>
<summary>Centro de reportes</summary>

Acceso a ventas, productos, inventario, artículos sin movimiento y análisis avanzado.

![Centro de reportes](img/16-centro-reportes.jpg)

</details>

<details>
<summary>Ventas e indicadores diarios</summary>

Del 23/10 al 22/11/2026: $1,153.60, 111 ventas y ticket promedio $10.39. El gráfico usa un eje monetario y otro para transacciones.

![Ventas e indicadores diarios](img/17-ventas-por-dia.jpg)

</details>

<details>
<summary>Agrupación semanal</summary>

Los mismos filtros y totales, agrupados por semana. Los extremos pueden contener semanas parciales.

![Agrupación semanal](img/18-ventas-por-semana.jpg)

</details>

<details>
<summary>Agrupación mensual</summary>

Los mismos datos agrupados por mes. Octubre y noviembre son parciales dentro del intervalo; no representan dos meses completos.

![Agrupación mensual](img/33-ventas-por-mes.jpg)

</details>

<details>
<summary>Top de productos por unidades</summary>

Ranking de diez productos del 01/11 al 22/11/2026. Los $430.45 y 336 unidades corresponden al Top seleccionado, no a todas las ventas del negocio.

![Top de productos por unidades](img/19-top-productos.jpg)

</details>

<details>
<summary>Estado y distribución del inventario</summary>

660 unidades disponibles y $892.90 a precio de venta. Incluye productos normales, críticos y agotados. La imagen muestra la parte superior y primeras filas del reporte.

![Estado y distribución del inventario](img/20-inventario-completo.jpg)

</details>

<details>
<summary>Filtrar productos críticos</summary>

Se muestran tres productos con una, dos y tres unidades. Los KPI superiores permanecen globales; la tabla y su total responden al filtro.

![Filtrar productos críticos](img/26-filtro-stock-critico.jpg)

</details>

<details>
<summary>Productos sin ventas recientes</summary>

Tres productos sin ventas en los últimos 30 días: 61 unidades y $85.55 a precio de venta. Ese importe no es costo de adquisición ni una pérdida realizada.

![Productos sin ventas recientes](img/21-sin-movimiento.jpg)

</details>

<details>
<summary>Resumen por categorías</summary>

Seis categorías y $816.20 en 80 ventas únicas del 01/11 al 22/11. Una venta puede participar en varias filas de categoría.

![Resumen por categorías](img/22-ventas-categorias.jpg)

</details>

<details>
<summary>Gráfico por categoría</summary>

Detalle del gráfico de barras. Abarrotes representa $231.75; se muestra junto con parte de la tabla para contrastar los valores.

![Gráfico por categoría](img/35-grafico-categorias.jpg)

</details>

<details>
<summary>Tabla por categoría</summary>

Detalle de ingresos, cantidades y proporciones por categoría. Las transacciones de las filas no se suman para obtener ventas únicas.

![Tabla por categoría](img/36-tabla-categorias.jpg)

</details>

<details>
<summary>Movimientos del período</summary>

Dos entradas en noviembre: ocho cepillos y 30 granolas, 38 unidades en total y $40.00 de compra. Las entradas históricas de agosto quedan fuera del filtro.

![Movimientos del período](img/23-movimientos-stock.jpg)

</details>

<details>
<summary>Margen bruto por producto</summary>

Ingresos $816.20 menos costo de mercadería $494.05: margen bruto $322.15 (39.5% redondeado). No incluye gastos operativos, impuestos o pérdidas. Se usó costo constante por producto entre lotes.

![Margen bruto por producto](img/24-ganancias.jpg)

</details>

<details>
<summary>Exportar resultados</summary>

La descarga CSV se ejecutó y se contrastó con el resumen mensual. PDF aparece como Próximamente, no como función terminada.

![Exportar resultados](img/25-exportar-csv.jpg)

</details>
