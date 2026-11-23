# Resultados del proyecto y lo que aprendí

## Qué se materializó en QUANTY

El resultado del proyecto es un prototipo que conecta la operación de un pequeño negocio: cuentas, clasificación de productos, entradas por lote, registro de ventas, existencias y reportes. Su valor como caso académico está en explicar esa relación y mostrarla en funcionamiento.

| Resultado del sistema | Qué permite demostrar |
|---|---|
| Registro y acceso | Un propietario crea una cuenta y utiliza la aplicación |
| Catálogo organizado | Los productos se clasifican y se mantienen disponibles para entradas y ventas |
| Entradas por lote | Se registran unidades, precios y vencimientos asociados a un producto |
| Venta con detalles | Una operación conserva varios artículos, cantidades y subtotales |
| Descuento FIFO | La venta se relaciona con la salida de unidades de los lotes más antiguos |
| Reportes de la cuenta | Los registros se consultan por período, producto, categoría o estado |
| Exportación CSV | El propietario puede obtener líneas de venta para otra revisión |

Esto no equivale a afirmar mejoras de productividad o rentabilidad de una empresa. Los datos de demostración permiten observar las funciones; no constituyen mediciones de impacto del proyecto.

## Tablas y relaciones de un mini ERP en MySQL

Trabajé y comprendí a nivel básico cómo relacionar las tablas que necesita una operación de inventario y ventas. El producto no contiene todo lo que ocurre en el negocio: sus entradas y sus ventas necesitan registros relacionados.

Por ejemplo, un producto puede recibir varios lotes, y una venta puede incluir varios productos mediante sus detalles. Relacionar esas entidades permite conservar el historial y consultar el estado de la operación.

Lo que destaco como aprendizaje es **la lógica del modelo relacional aplicado al negocio**. El código y la construcción de los scripts se trabajaron con asistencia; no atribuyo su implementación completa a programación manual propia.

## Registro e inicio de sesión

Comprendí el recorrido de registrar una cuenta e iniciar sesión para utilizar el sistema. La identidad de la cuenta es relevante porque la aplicación asocia con ella los registros del propietario.

En el caso de QUANTY, esto permite entender la propuesta de una misma web para distintos negocios: todos utilizan los mismos módulos, pero trabajan con registros asociados a su cuenta. No es necesario que cada tienda tenga una aplicación distinta.

## Entradas, ventas y FIFO

Trabajé la diferencia entre una ficha de producto, una entrada y una venta. Crear el producto define el artículo; registrar una entrada incorpora unidades; vender produce una salida que debe reflejarse en las existencias.

También comprendí el método FIFO: consumir primero los lotes más antiguos. Si hay 5 unidades en un lote antiguo y 8 en uno posterior, una salida de 7 utiliza las 5 primeras y 2 del segundo. Esa lógica ayuda a explicar por qué se conservan cantidades por lote y no solamente un número general en el producto.

El recorrido fotografiado permite observar una entrada, una venta y el saldo que queda. Es una forma de mostrar que entiendo la relación de esas operaciones, sin convertir los datos ficticios en un análisis de resultados comerciales.

## Definir la información de reportes y gráficos

En los reportes participé definiendo **de dónde queríamos obtener la información y qué debía mostrarse**. Fuimos indicando a la IA la lógica esperada, qué registros utilizar y qué lectura necesitábamos en las pantallas.

No escribí directamente las consultas de los reportes. El aprendizaje que destaco es formular el requisito: pasar de «queremos entender las ventas o el inventario» a precisar qué datos, filtros, tablas o gráficos ayudarían a verlo.

Este aporte se relaciona con análisis de necesidades y comprensión de la operación del negocio. La programación de la consulta y de la visualización fue asistida.

## Tecnología del proyecto y conocimientos personales

| Área | Cómo la presento profesionalmente |
|---|---|
| MySQL | Conocimientos básicos de tablas y relaciones de un mini ERP |
| Cuentas y acceso | Comprensión del registro e inicio de sesión y su relación con los registros |
| Inventario | Comprensión de entradas, ventas, existencias y lógica FIFO |
| Reportes | Participación en requisitos y lógica de la información, con código asistido |
| PHP y Laravel | Tecnologías utilizadas en la implementación grupal; mi siguiente paso es profundizar en su organización técnica |
| Docker del laboratorio | Forma de ejecutar y conservar la aplicación; se explica como entorno de demostración |

Mis siguientes pasos son repasar la estructura de Laravel y practicar consultas sencillas que permitan reproducir por mi cuenta una parte de los reportes. En el CV destaco lo que puedo vincular a mi participación confirmada, no todas las tecnologías como si tuviera el mismo nivel de autonomía en ellas.

## Cómo revisar esta evidencia

El [modelo de datos](ARQUITECTURA.md#modelo-relacional) ayuda a ubicar las relaciones; los [recorridos](RECORRIDOS_DE_USO.md) muestran cómo se usan; y la [galería](RECORRIDO_VISUAL.md) permite contrastarlos con la interfaz. La [participación](PARTICIPACION.md) explica el trabajo grupal y la asistencia de IA.

La evidencia funcional incluye pruebas de registro, acceso, perfiles, operaciones de inventario, ventas y reportes en la implementación privada. El caso público muestra el proyecto y sus aprendizajes, conservando separados el código, los accesos y los documentos académicos completos.
