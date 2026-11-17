# PapeleriaPos
Nombre del proyecto: PapeleriaPOS.

Negocio: Papelería.

Objetivo: Conformar el equipo de trabajo, definir el negocio y realizar el diseño inicial del sistema de punto de venta (POS).
1. Definición del negocio
Nombre del negocio: Papelería POS.

Descripción:

Es un negocio dedicado a la venta de útiles escolares y artículos de papelería. Su objetivo es ofrecer productos a estudiantes, profesores y personas que necesiten materiales escolares y de oficina.

¿Qué vende?
- Cuadernos.
- Lápices y lapiceros.
- Borradores y sacapuntas.
- Carpetas y hojas.
- Colores y marcadores.
- Artículos de oficina.
Tipos de productos y precios:
- Productos escolares: tienen un precio individual dependiendo del producto.
- Productos de papelería al por mayor: tienen precios especiales cuando se compran en grandes cantidades.
Medios de pago aceptados:
- Efectivo.
- Transferencia bancaria.
2. Integrantes del equipo
- Alejandro Acevedo.
- Juan Pablo Díaz.
- Nombre del tercer integrante.
3. Identificación de las clases
Para desarrollar el sistema POS se identificaron las siguientes clases:

Cliente: representa a los compradores. Sus atributos son nombre, documento y teléfono. Sus métodos son registrarCliente() y consultarDatos().

Producto: representa los productos de la papelería. Sus atributos son código, nombre, precio y stock. Sus métodos son consultarPrecio() y actualizarStock().

ProductoEscolar: representa los productos escolares y permite calcular su precio.

ProductoPapeleriaMayor: representa los productos vendidos al por mayor y maneja descuentos o precios especiales por cantidad.

Venta: registra las ventas realizadas. Sus atributos son número, fecha, cliente y total. Sus métodos son calcularTotal() y registrarVenta().

ItemVenta: relaciona los productos con una venta. Sus atributos son producto, cantidad y subtotal. Su método es calcularSubtotal().

MetodoPago: representa los medios de pago y contiene el método procesarPago().

PagoEfectivo: representa los pagos en efectivo. Su atributo es valorRecibido y su método es calcularCambio().

PagoTransferencia: representa los pagos por transferencia. Su atributo es referencia y su método es validarTransferencia().

SistemaPOS: administra el funcionamiento del sistema. Sus métodos son registrarProducto(), buscarProducto() y realizarVenta().
4. Relaciones entre las clases
1. ProductoEscolar hereda de Producto.
2. ProductoPapeleriaMayor hereda de Producto.
3. Venta se relaciona con Cliente porque cada venta puede tener un comprador.
4. Venta contiene uno o varios ItemVenta.
5. ItemVenta se relaciona con Producto porque indica qué producto se vendió y en qué cantidad.
6. PagoEfectivo y PagoTransferencia heredan de MetodoPago.
7. SistemaPOS administra los productos, clientes y ventas.
5. Diagrama de clases U
