# Mi participación en QUANTY

## Trabajo grupal y enfoque de mi aporte

QUANTY fue un trabajo universitario grupal de Emprendedurismo. Participé en la construcción de una propuesta para digitalizar inventario y ventas de pequeños negocios y en el trabajo paso a paso para convertirla en una aplicación.

Partimos de una referencia ERP en PHP de YouTube y decidimos reconstruir la propuesta con Laravel. Fuimos trabajando con asistencia de IA, preguntando qué hacía el código, solicitando cambios y ajustando la base, las conexiones y la interfaz. No fue simplemente descargar el sistema y conservarlo sin cambios.

## Datos y lógica de operación

Uno de los conocimientos que trabajé fue **cómo relacionar las tablas de un mini ERP en MySQL**. El negocio no se representa en una sola tabla: un producto pertenece a una clasificación, puede recibir varias entradas y aparece en detalles de distintas ventas.

Comprendí la diferencia entre definir el producto y registrar una entrada de mercadería. También la relación entre una venta, su detalle y el inventario que queda disponible. En ese proceso trabajé la lógica **FIFO**, que consume primero las existencias de los lotes más antiguos.

El registro e inicio de sesión también forman parte de lo que recuerdo comprender: el propietario crea una cuenta, accede a la aplicación y trabaja con la información asociada a ella.

## Mi participación en los reportes

En los reportes mi aporte estuvo en **definir qué información queríamos mostrar, de dónde debía obtenerse y cómo presentarla**. Indicábamos a la IA qué registros nos interesaban, qué relaciones debían considerarse y qué debía comunicar un reporte, una tabla o un gráfico.

Esto es diferente de escribir las consultas directamente. La implementación del código fue asistida; mi participación se concentró en la lógica del resultado solicitado. Por ejemplo, que el propietario pudiera revisar ventas de un período, identificar productos sin movimiento o relacionar una venta con las existencias.

## Lo que aprendí y el nivel con el que lo presento

| Área | Aprendizaje que puedo vincular a QUANTY |
|---|---|
| MySQL y modelo relacional | Tablas y relaciones de un mini ERP: cuentas, categorías, productos, entradas, ventas y detalles |
| Registro e inicio de sesión | Recorrido de creación y uso de una cuenta para acceder a la información del negocio |
| Entradas y ventas | Diferenciar datos del catálogo, recepción de unidades y salida por venta |
| FIFO | Comprender que las salidas consumen primero las existencias de los lotes más antiguos |
| Reportes y gráficos | Traducir necesidades del negocio a información que debía obtenerse y mostrarse, con implementación asistida |

Presento estos puntos como formación académica y práctica inicial. Mi siguiente paso en Laravel es profundizar en sus rutas, controladores, modelos y vistas. Por ahora distingo la arquitectura descrita del proyecto de los conocimientos personales que ya puedo vincular a mi participación.

## Uso de IA

La IA tuvo un papel importante en código, interfaz y datos. Trabajábamos paso a paso, pidiendo explicaciones y cambios y copiando y ajustando fragmentos. En los reportes también ayudó a transformar lo que solicitábamos en consultas, cálculos y gráficos.

Mi aporte consistió en participar en los requisitos, orientar el comportamiento esperado y revisar lo que necesitábamos mostrar, dentro de un trabajo grupal. Mantengo esa distinción para que el caso respalde mi formación sin atribuirme programación autónoma ni una experiencia laboral que no corresponde al proyecto.

## Equipo académico

Elias Alexander Garcia Garcia, Cristian Leandro Rodriguez Vasquez, Ever Alexis Corleto Guardado y Samuel Enrique Alvarado Romero.

La lista conserva los créditos del trabajo grupal. La referencia exacta de YouTube y los permisos de los materiales deben identificarse antes de redistribuir públicamente toda la implementación; este repositorio presenta el caso y sus evidencias.

[Resultados y aprendizajes concretos](RESULTADOS_Y_APRENDIZAJES.md) · [Contexto del proyecto](CONTEXTO_DEL_PROYECTO.md).
