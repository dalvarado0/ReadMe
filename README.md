─────────────────────────────────────────────────────────────
─██████████████─██████████████─██████─────────██████████████─
─██░░░░░░░░░░██─██░░░░░░░░░░██─██░░██─────────██░░░░░░░░░░██─
─██████░░██████─██░░██████████─██░░██─────────██░░██████░░██─
─────██░░██─────██░░██─────────██░░██─────────██░░██──██░░██─
─────██░░██─────██░░██████████─██░░██─────────██░░██──██░░██─
─────██░░██─────██░░░░░░░░░░██─██░░██─────────██░░██──██░░██─
─────██░░██─────██░░██████████─██░░██─────────██░░██──██░░██─
─────██░░██─────██░░██─────────██░░██─────────██░░██──██░░██─
─────██░░██─────██░░██████████─██░░██████████─██░░██████░░██─
─────██░░██─────██░░░░░░░░░░██─██░░░░░░░░░░██─██░░░░░░░░░░██─
─────██████─────██████████████─██████████████─██████████████─
─────────────────────────────────────────────────────────────

# Instalación

# Diagrama Conceptual

![alt text](https://pi7e-davidalvaradov414989.codeanyapp.com/DavidPI/diagramaConceptual.jpg "Logo Title Text 1")

# Historias de usuario

No. | Quien | Que | Para que
--- |--- | --- | ---
1 | Vendedor | Agregar clientes a mi agenda de manera rápida. | Para poder no perder algún cliente por cuestiones de tiempo
2 | Vendedor | Agregar productos a mis catálogos | Para cubrir necesidades de mis clientes.
3 | Vendedor | Que pueda cargar una foto al agregar mis productos. | Para que mis clientes puedan dar una vista previa a lo que pueden comprar.
4 | Vendedor | Al buscar un cliente, ver su estado de cuenta. | Para saber el estado actual del cliente.
5 | Vendedor | Filtrar a  los clientes por su estatus (debe o no debe) de cuenta. | Hacer un listado dependiendo de su estatus, debe o no debe.
6 | Vendedor | Poder realizar ventas por abonos semanales o mensuales. | En caso que un cliente no pueda pagar en un solo pago, darle la oportunidad de pagar en plazos.
7 | Vendedor | Poder realizar ventas al contado | Vender al cliente un producto que quiera al momento.
8 | Vendedor | Modificar datos de un cliente. | Para mantener los datos actualizados de los clientes.
9 | Vendedor | Modificar datos de un producto. | Para modificar los datos actualizados de los productos.
10 | Vendedor | Ver qué clientes tienen algún pago de abonos pendiente | Filtrar para mandar un aviso de que tiene uno o varios abonos pendientes.
11 | Vendedor | Generar reportes de pagos pendientes de los clientes, por día, semana o mes, junto con los datos de los clientes como domicilio y el monto a pagar. | Llevar un control de los pagos pendientes.
12 | Vendedor | Poder agregar productos pero no agregarlos al catálogo. | Agregar productos y dejarlos pendientes en caso de que falte información, ya se cantidad total, precio descripción del producto.
13 | Vendedor | Tener varias formas de ingresar entrar en la aplicación, ya sea por contraseña, patrón o PIN de seguridad. |Poder elegir al menos dos maneras de entrar a la aplicación.
14 | Vendedor | En caso de pérdida, robo o extravío del smartphone poder recuperar todo el catálogo junto con los clientes. | No tener complicaciones con continuar las ventas ni los cobros.
15 | Vendedor | Poder vender más de un producto a la vez. | En una solo venta poder vender todo lo que el inventario permita.
16 | Vendedor | Poder apartar un producto a un cliente por un periodo de tiempo acordado. | Dar la facilidad al cliente de en caso de no poder pagar en un solo pago  y no elegir el pago a plazos, poder apartar el producto.
17 | Vendedor | Quiero poder contactar con el soporte técnico en caso de que tenga algún inconveniente. | En caso de alguna duda, problema o sugerencia poder comunicar con el soporte técnico de la aplicación por algún medio de comunicación disponible.
18 | Vendedor | Quiero generar gráficas sobre todo lo relacionado al catálogo, los clientes y ventas. | Generar estadística sobre todo lo relacionado con las ventas, clientes y ventas para la toma de decisiones.
19 | Vendedor | Cada vez que se reciba dinero por un pago a abono generar un acuse de recibo y mandarselo automáticamente al cliente por correo. | Mantener informado al cliente sobre cualquier pago que se haga y tener evidencia sobre los pagos que se van realizando.

# Casos de uso

![alt text](https://pi7e-davidalvaradov414989.codeanyapp.com/DavidPI/cu_gestionClientes.jpg "Logo Title Text 1")
![alt text](https://pi7e-davidalvaradov414989.codeanyapp.com/DavidPI/cu_gestionProductos.jpg "Logo Title Text 1")
![alt text](https://pi7e-davidalvaradov414989.codeanyapp.com/DavidPI/cu_reportes.jpg "Logo Title Text 1")

# Diagrama entidad - relación

![alt text](https://pi7e-davidalvaradov414989.codeanyapp.com/DavidPI/diagramaER.png "Logo Title Text 1")

# Diccionario de datos

## Tabla Clientes
### Descripción
Tabla donde se van a almacenar todos los clientes de los vendedores.

No. | Campo | Tamaño | Tipo de dato | Descripción
--- |--- | --- | --- | --- 
1 | IdCliente | 11 | int | Identidicador del cliente 
2 | Nombre | 35 | varchar | Nombre completo del cliente
3 | Direccion | 50 | varchar | Domicilio del cliente
4 | Telefono | 10 | varchar | Telefono del cliente
5 | Email | 35 | varchar | Correo electronico del cliente
6 | Foto | -- | text | Nombre de la imagen
7 | IdVendedor | 11 | int | Id del vendedor para relacionarlo con sus clientes

*Relaciones* | 
---|
Vendedores | 

_Campos Clave_ |
---|
IdCliente |

## Tabla Vendedores
### Descripción
Tabla donde se van a almacenar todos los vendedores

No. | Campo | Tamaño | Tipo de dato | Descripción
--- |--- | --- | --- | --- 
1 | IdVendedor | 11 | int | Identidicador del vendedor 
2 | Nombre | 35 | varchar | Nombre completo del vendedor
3 | Direccion | 50 | varchar | Domicilio del vendedor
4 | Telefono | 10 | varchar | Telefono del vendedor
5 | Email | 35 | varchar | Correo electronico del vendedor
6 | Contrasena | 35 | varchar | Contraseña del vendedor

*Relaciones* | 
---|
Clientes | 

_Campos Clave_ |
---|
IdVendedor |

## Tabla Abonos
### Descripción
Tabla donde se van a almacenar todos los abonos que registren los vendedores

No. | Campo | Tamaño | Tipo de dato | Descripción
--- |--- | --- | --- | --- 
1 | idabono | 11 | int | Identidicador del abono
2 | fechaabono | 35 | varchar | Fecha que se hizo el abono
3 | cantidadabono | 50 | varchar | Cantidad que fue abonada
4 | idventa | 10 | varchar | Id de la venta a la que se abona

*Relaciones* | 
---|
Ventas | 

_Campos Clave_ |
---|
idabono |

## Tabla Abonos
### Descripción
Tabla donde se van a almacenar todos los abonos que registren los vendedores

No. | Campo | Tamaño | Tipo de dato | Descripción
--- |--- | --- | --- | --- 
1 | IdVenta | 11 | int | Identidicador de la venta
2 | Fecha | 35 | varchar | Fecha de venta
3 | Cantidad | -- | double | Cantidad de productos que se compro
4 | TotalAPagar | 11 | varchar | Total a pagar
5 | PagoEnAbonos | -- | double | --
6 | IdCliente | -- | text | Fecha que se hizo el abono
7 | IdProducto | -- | text | Cantidad que fue abonada
8 | IdVendedor | 11 | int | Id de la venta a la que se abona

*Relaciones* | 
---|
Clientes |
Productos |
Vendedores |

_Campos Clave_ |
---|
 IdVenta |

# Interfaces de usuario
