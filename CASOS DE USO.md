**Casos de Uso:  **   	

**Visualizar detalles del producto**

**Actores:**

●     Cliente (usuario registrado)  
●     Administrador del sistema

**Precondiciones:**

●     El cliente debe estar registrado en el sistema.

●     El sistema debe estar en funcionamiento y accesible para los usuarios.

●     El catálogo de productos debe estar actualizado y disponible.

●     El sistema debe permitir pagos mediante transferencia bancaria.

 

**Flujo Básico:**

1. El cliente accede al sistema e ingresa su nombre de usuario y contraseña.  
2. El sistema valida las credenciales y permite el acceso del usuario.  
3. El cliente navega por el catálogo de productos, organizado en secciones como "Mujeres" y "Niños".  
4. El cliente selecciona un producto para ver sus detalles.  
5. El sistema muestra las opciones de talles y colores disponibles.  
6. Si el producto no está en stock, el sistema lo indica, pero sigue mostrando la información del producto.  
7. El cliente selecciona el talle y color deseado y añade el producto al carrito de compras.  
8. El cliente puede seguir navegando y añadiendo productos o proceder a la compra.  
9. El cliente revisa los productos en el carrito y, si es necesario, realiza modificaciones.  
10. El cliente confirma los productos y procede a realizar el pago.  
11. El cliente selecciona la opción de pago mediante transferencia bancaria.  
12. El sistema proporciona las instrucciones para la transferencia bancaria.  
13. El cliente confirma en el sistema que ha realizado la transferencia.  
14. El sistema registra el pedido y genera una confirmación.  
15. El cliente recibe una notificación de confirmación del pedido.

**Flujos Alternativos:**

●     **1.A. Si el cliente no está registrado:**

1\.    El cliente accede a la opción de registro.

2\.    Proporciona los datos necesarios y crea una cuenta.

3\.    El sistema valida la información y envía una confirmación por correo electrónico.

●     **2.A. Si el producto seleccionado no está en stock:**

1\.    El cliente puede optar por recibir una notificación cuando el producto vuelva a estar disponible.

2\.    Proporciona su correo electrónico para recibir la notificación.

**Postcondiciones:**

●     El pedido del cliente es registrado en el sistema.

●     El cliente recibe una confirmación del pedido.

●     El administrador del sistema tiene acceso a la información del pedido.

---

**Concretar ventas online**

**Actores:**

●     Cliente  
●     Sistema de pago

**Precondiciones:**

●     El cliente ha seleccionado productos en el carrito.

**Flujo Principal:**

1. El cliente accede al carrito.  
2. Al hacer clic en "Finalizar compra".  
3. El sistema muestra las instrucciones de pago por transferencia bancaria.  
4. El cliente realiza la transferencia y envía el comprobante junto con la dirección de envío al WhatsApp indicado.  
5. El administrador revisa el comprobante y valida la información.  
6. Si todo es correcto, confirma la venta.  
7. Se genera la orden y se envía la confirmación al cliente.

**Flujos Alternativos:**

●     **5.A. Comprobante inválido o incorrecto:** Se solicita enviar o corregir el pago.

●     **5.B. Cliente no envía comprobante:** Se envía un recordatorio.

●     **5.C. Error en la información de envío:** Se solicita corrección antes de confirmar la orden.

**Postcondiciones:**

●     Pedido confirmado y registrado en el sistema.

---

**Notificación de Stock**

**Actores:**

●     Cliente (usuario registrado)  
●     Administrador del sistema

**Precondiciones:**

●     El cliente debe estar registrado en el sistema.

●     El sistema debe estar en funcionamiento y accesible.

●     El catálogo de productos debe estar actualizado.

**Flujo Básico:**

1. El cliente accede al sistema e inicia sesión.  
2. Navega por el catálogo de productos.  
3. Selecciona un producto para ver sus detalles.  
4. El sistema verifica la disponibilidad de stock.  
5. Si el producto no está disponible, se muestra una notificación de "Producto sin stock".  
6. El cliente puede solicitar una notificación cuando el producto vuelva a estar disponible.  
7. Ingresa su correo electrónico y confirma la solicitud.  
8. El sistema registra la solicitud y envía una confirmación.  
9. Cuando el producto está en stock, el sistema envía una notificación.

**Postcondiciones:**

●     El cliente ha sido informado sobre la falta de stock.  
●     Si solicita la notificación, recibirá un aviso cuando el producto esté disponible.

---

**Carrito de Compras**

**Actores:**

●     Cliente  
●     Sistema

**Flujo Principal:**

1. El cliente agrega productos al carrito.  
2. El sistema muestra el contenido del carrito con productos, cantidades y precios.  
3. El cliente puede modificar las cantidades o eliminar productos.  
4. Procede a la compra seleccionando el método de pago.  
5. El sistema calcula el total de la compra.  
6. El cliente confirma el pedido.

**Postcondiciones:**

●     Pedido registrado en el sistema.

---

**Gestión de Categorías de Productos**

**Actores:**

●     Administrador del sistema

**Precondiciones:**

●     El sistema debe estar en funcionamiento y accesible.  
●     El administrador debe haber iniciado sesión.

**Flujo Básico:**

1. El administrador accede al sistema.  
2. Navega a la sección de gestión de categorías.  
3. Selecciona la opción de agregar una nueva prenda a una categoría.  
4. Si la categoría ya existe, la prenda se añade a la misma.

**Flujo Alternativo:**

1. Si la categoría no existe, el administrador tiene la opción de crearla.  
2. El sistema guarda la nueva categoría y asigna la prenda.  
3. Se actualiza el catálogo de productos.

**Postcondiciones:**

●     La prenda ha sido agregada a la categoría correspondiente.

●     Si no existía la categoría, se ha creado y añadido la prenda.

●     El catálogo de productos se ha actualizado correctamente.

---

**Tipos de Usuarios**

**Actores:**

●     Cliente (usuario registrado)  
●     Administrador del sistema

**Precondiciones:**

●     El sistema debe estar en funcionamiento y accesible.  
●     El usuario debe estar registrado e iniciar sesión para acceder a sus funcionalidades.

**Flujo Básico:**

1. El usuario accede al sistema e inicia sesión.  
2. El sistema verifica el tipo de usuario y le asigna los permisos correspondientes:

   ○     Si es un administrador, accede a funciones de gestión del catálogo, gestión de pedidos y administración de clientes.

   ○     Si es un cliente, puede visualizar el catálogo, agregar productos al carrito y realizar compras.

3. El usuario interactúa con el sistema según los permisos asignados.

**Flujos Alternativos:**

●     **1.A. Si un usuario intenta acceder a funciones restringidas para su rol:**  
○     El sistema muestra un mensaje de error y redirige al usuario a su área de funciones permitidas.

**Postcondiciones:**

●     El usuario ha accedido correctamente a las funcionalidades asignadas según su rol.  
●     El sistema garantiza que los permisos de usuario se respeten.

 

