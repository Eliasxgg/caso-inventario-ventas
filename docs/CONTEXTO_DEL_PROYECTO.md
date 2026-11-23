# De la necesidad de negocio a QUANTY

## Origen académico

QUANTY se desarrolló en grupo en la asignatura Emprendedurismo de la Universidad Evangélica de El Salvador, durante el ciclo 8 de 2025. El trabajo giró alrededor de la digitalización de la gestión operativa de microempresas salvadoreñas: inventario, ventas y la información necesaria para comprender el negocio.

La situación que orientó la propuesta fue el uso de cuadernos, hojas sueltas o registros desconectados. Un propietario puede anotar cuánto vendió y, aun así, no relacionarlo con las unidades que quedan, las entradas anteriores o los productos que llevan tiempo detenidos. La necesidad planteada fue reunir esos registros en una herramienta sencilla.

El público propuesto incluía tiendas de abarrotes, minisúper, negocios familiares y pequeños emprendimientos. No se definió la aplicación para una sola tienda específica: la intención era que diferentes propietarios pudieran utilizar el mismo servicio con su propia cuenta.

## Cómo se fue construyendo la propuesta

| Trabajo académico | Qué aportó al proyecto |
|---|---|
| Investigación sobre digitalización operativa | Delimitar la necesidad de pasar del registro manual a información organizada |
| Propuesta de valor | Priorizar facilidad de uso, inventario, ventas y reportes comprensibles |
| Modelo Canvas | Relacionar usuarios, recursos, actividades, canales y sostenibilidad del servicio |
| Comparación de competidores | Pensar diferencias de alcance y simplicidad frente a soluciones más amplias |
| Estructura de costos | Considerar recursos técnicos, operación, soporte y un posible modelo de suscripción |
| Prototipo web | Convertir esas ideas en cuentas, formularios, registros y reportes |

Estos documentos muestran la evolución de la idea. Los costos, precios y escenarios pertenecen a una propuesta académica; no son facturación, usuarios contratados ni gastos de una empresa en funcionamiento. Los estudios completos se conservan de forma privada y aquí se explica únicamente lo necesario para entender el proyecto.

## Finalidad de la aplicación

QUANTY busca acompañar la operación diaria de un pequeño negocio:

1. Registrar qué productos maneja y cómo los clasifica.
2. Incorporar mercadería mediante entradas con cantidad, costo, precio y vencimiento cuando corresponda.
3. Registrar qué se vende y mantener la relación entre la venta y sus productos.
4. Actualizar las existencias disponibles por lote.
5. Consultar información organizada sobre ventas, inventario y productos sin movimiento.

La propuesta no se limita a digitalizar una lista. Su valor está en conectar **catálogo, entradas, ventas y reportes** para que el propietario encuentre información que pueda utilizar al revisar su negocio.

## De una referencia técnica al prototipo Laravel

Al comenzar revisamos un ERP en PHP encontrado en YouTube. El grupo decidió reconstruir la propuesta con Laravel tomando esa referencia como punto de partida. Trabajamos con asistencia importante de IA en la base, conexiones, código e interfaz, haciendo preguntas y ajustes paso a paso.

Por ello distingo dos cosas: el problema y el comportamiento que buscábamos resolver como grupo, y la ayuda utilizada para implementarlos. El prototipo no se presenta como una plantilla intacta ni como programación manual individual. La referencia exacta del video sigue pendiente de identificar.

## Modelo para distintos negocios

Una cuenta representa al propietario y su negocio dentro del prototipo. Los registros se asocian al usuario: cada cuenta mantiene su catálogo, entradas y ventas, y las consultas principales utilizan esa asociación al mostrar los datos.

La aplicación y MySQL son compartidos. No se configura una base independiente por tienda. Este es el modelo de uso planteado para que la herramienta sea general; las capturas utilizan una sola cuenta ficticia para explicar los mismos recorridos que seguiría otro propietario con sus propios registros.

El prototipo no define todavía una estructura de empleados, sucursales o permisos por puesto dentro de una misma empresa. Eso corresponde a una ampliación del modelo, no a una función que se atribuya a la versión mostrada.

## Qué presenta este caso público

El caso explica el origen, los módulos, la arquitectura y mi aprendizaje. Las capturas permiten ver cómo se materializa la propuesta. Los datos ficticios se utilizan para que las pantallas no estén vacías y para ilustrar los reportes, no para presentar resultados de investigación o de una tienda real.

[Recorridos de uso](RECORRIDOS_DE_USO.md) · [Arquitectura](ARQUITECTURA.md) · [Participación](PARTICIPACION.md).
