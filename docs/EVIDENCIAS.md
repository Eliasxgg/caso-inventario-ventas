# Evidencias del funcionamiento de QUANTY

## Qué se puede contrastar en este caso

El propósito de la evidencia es que el lector pueda relacionar la propuesta, los módulos descritos y sus pantallas. Una imagen muestra una vista concreta; un recorrido conecta varias vistas y permite explicar una operación completa.

| Capacidad del proyecto | Evidencia que la acompaña | Qué muestra |
|---|---|---|
| Registrar y utilizar una cuenta | Registro, inicio de sesión y perfil ficticio | Acceso y relación del usuario con su espacio de trabajo |
| Organizar catálogo | Categorías, alta y detalle de producto | Clasificación e identidad del artículo |
| Recibir mercadería | Formulario de entrada e historial de lotes | Incorporación de cantidades y precios |
| Registrar una venta | Preparación, confirmación y detalle | Una operación con varios artículos y sus subtotales |
| Actualizar existencias | Detalle del producto antes y después | Relación entre entrada, salida y saldo |
| Mostrar alertas | Panel, inventario crítico y producto agotado | Situaciones que requieren revisión del propietario |
| Consultar reportes | Períodos, productos, categorías, movimientos y margen | Distintas lecturas de los registros de una cuenta |
| Obtener un archivo | Pantalla de exportación y CSV ficticio | Descarga de líneas de venta para otra revisión |

## El recorrido principal

La demostración crea un producto, recibe un lote de 30 unidades y registra una venta que consume dos. El producto queda con 28 unidades y la venta conserva sus líneas. Esta secuencia muestra una relación funcional; no pretende medir el impacto comercial del proyecto.

El historial ficticio adicional permite que los reportes muestren distintos períodos, categorías, existencias y productos sin movimiento. No se presenta como operaciones realizadas por una empresa ni como un análisis de éxito de QUANTY.

## Complemento de comprobación de la implementación

La implementación privada cuenta con 28 pruebas y 408 verificaciones automatizadas. Se comprobaron registro, acceso, perfiles, operaciones de inventario/ventas y consultas de reportes, además del balance de la población de demostración. También se verificó la construcción del laboratorio desde un entorno limpio.

Las pruebas complementan el recorrido; no reemplazan la explicación del proyecto ni certifican todos los escenarios de negocio o de autorización. La finalidad del repositorio público es mostrar cómo funciona la solución y qué aprendizaje puedo respaldar con ella.

## Cómo se organiza el material

- [Galería seleccionada y enlaces al resto de pantallas](RECORRIDO_VISUAL.md).
- [Diagramas de las tareas del propietario](RECORRIDOS_DE_USO.md).
- [Arquitectura y modelo relacional](ARQUITECTURA.md).
- [Resultados funcionales y aprendizajes](RESULTADOS_Y_APRENDIZAJES.md).
- [Manifiesto de los 36 archivos de imagen](MANIFIESTO_EVIDENCIAS.json), con fecha, pantalla de origen y huella de archivo para identificar las capturas originales.

El manifiesto es un índice técnico de archivos. No es un informe de resultados del negocio. Las claves de acceso, respaldos y documentos académicos completos se conservan por separado.
