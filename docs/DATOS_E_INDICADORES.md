# Datos, indicadores y lectura

## Origen y corte

La cuenta ficticia Tienda Horizonte se creó para demostrar el sistema sin utilizar ventas de una empresa ni datos de clientes. La población automática genera 6 categorías, 24 productos, 49 lotes y 294 ventas entre el 31/08 y el 22/11/2026. Después se ejecutó desde la interfaz el alta de la granola, una entrada de 30 unidades y una venta con dos productos: el corte final tiene **25 productos, 50 lotes y 295 ventas**. Son ventas registradas de demostración, no 295 clientes ni ventas comerciales reales.

Las fechas de la población se calculan respecto al día de ejecución. En una reproducción posterior, el historial cambia de fechas y los filtros deben ajustarse. Las capturas conservan el corte del 22/11/2026.

## Interpretar cada indicador

| Indicador | Definición y alcance | Resultado en la evidencia |
|---|---|---|
| Ventas del día | Suma de ventas del 22/11, cuenta de evidencias | $52.15 en 6 operaciones |
| Ventas del mes | Ventas únicas del 01/11 al 22/11 | $816.20 en 80 operaciones |
| Ventas por período | Intervalo inclusivo 23/10–22/11 | $1,153.60 en 111 operaciones |
| Ticket promedio del período | Importe del período / ventas únicas | $10.39 |
| Período previo | 22/09–22/10, también 31 días | $1,142.85; variación redondeada +0.9% |
| Stock por producto | Suma de cantidad disponible de sus lotes | 660 unidades en toda la cuenta |
| Productos críticos | Stock mayor que cero y menor o igual que tres | 3 productos |
| Productos agotados | Stock total igual a cero | 1 producto |
| Alerta del panel por lote | Lotes con cantidad disponible menor o igual que tres, incluidos lotes agotados | 25 lotes; no 25 productos críticos |
| Valor de inventario | Existencias × precio de venta | $892.90; no costo de adquisición |
| Sin movimiento | Productos con stock sin ventas en 30 días | 3 productos, 61 unidades, $85.55 a precio de venta |
| Top 10 | Diez productos ordenados por unidades vendidas en noviembre | 336 unidades y $430.45 del subconjunto |
| Margen bruto | Ingreso menos costo de mercadería registrado en detalles | $322.15 = $816.20 − $494.05; 39.47% |
| Entradas del mes | Lotes creados dentro del período | 2 entradas, 38 unidades, costo $40.00 |

En las filas por categoría, una venta con artículos de varias categorías aparece una vez en cada categoría correspondiente. La suma de esas participaciones no representa ventas únicas. El KPI general usa 80 ventas únicas. En los filtros de inventario y ventas, los KPI superiores pueden mantener el resumen global mientras la tabla muestra el subconjunto seleccionado.

El margen bruto no es utilidad neta: no incluye salarios, alquiler, impuestos, mermas u otros gastos. Esta simulación mantiene el costo de un producto constante entre lotes. El código descuenta lotes por FIFO y toma el último costo al registrar una venta; queda pendiente resolver y probar la valoración cuando los costos de lotes sean distintos.

## Ejemplos de lectura

En [categorías](img/35-grafico-categorias.jpg), Abarrotes aporta $231.75, un 28.4% de los $816.20 del período mensual. Ese aporte no basta para concluir que sea la categoría más rentable: también hay que comparar costos y gastos.

En [sin movimiento](img/21-sin-movimiento.jpg), cepillo dental, queso fresco y crema acumulan 61 unidades sin ventas en 30 días. En un negocio real revisaría demanda, ubicación, vencimientos y cantidades antes de proponer promociones o reposiciones. Los $85.55 son valor potencial de venta; no una pérdida realizada.

La [tendencia semanal](img/18-ventas-por-semana.jpg) resume los mismos 31 días que la diaria. Las semanas de los extremos son parciales; no deben compararse como si tuvieran igual duración. La agrupación mensual también contiene dos meses parciales. Las oscilaciones son propias del generador de datos, no evidencia de estacionalidad del mercado.

## Archivos y verificación

[resumen-demostracion.json](../datos/resumen-demostracion.json) se obtuvo con consultas de lectura. Se contrastó que las entradas menos las cantidades vendidas coincidan con las existencias y que cada venta coincida con la suma de sus detalles: no se encontraron desbalances en este corte.

[ventas-simuladas-noviembre.csv](../datos/ventas-simuladas-noviembre.csv) procede de una descarga real de la interfaz. Contiene 80 ID de venta distintos y sus líneas suman $816.20. El encabezado heredado «Total Venta» corresponde al subtotal de cada línea; para obtener una venta completa hay que agrupar sus filas por ID. No se debe repetir el total de la venta por cada producto ni contar cada fila como una transacción distinta.

La comprobación automatizada final cubre 28 pruebas y 408 verificaciones. Es evidencia de los recorridos y del balance de esta población; no equivale a comprobar todas las combinaciones, concurrencia o aptitud para producción.
