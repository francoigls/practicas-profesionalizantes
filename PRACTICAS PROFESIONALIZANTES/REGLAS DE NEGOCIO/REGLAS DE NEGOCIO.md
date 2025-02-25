# Reglas de Negocio:

#### **Hechos:**

* **Disponibilidad de Productos:** Un producto puede estar en stock o agotado.  
* **Tallas y Colores:** Cada producto tiene asociadas tallas y colores disponibles.  
* **Categorías de Productos:** Los productos se dividen en categorías específicas (por ejemplo, ropa de mujer, ropa de niños).

  #### **Restricciones:**

* **Registro Único:** El nombre de usuario debe ser único para cada cuenta de cliente.  
* **Validación de Datos:** Todos los campos obligatorios del registro deben ser completados correctamente para que se pueda crear la cuenta.  
* **Pagos:** Solo se aceptan pagos mediante transferencia bancaria.  
* **Interfaz:** La interfaz del sistema debe ser completamente responsive, es decir, adaptable al 100% para dispositivos móviles.

  #### **Acciones Disparadoras:**

* **Agregar al Carrito:** Al seleccionar una talla y un color, el cliente puede agregar el producto al carrito de compras.  
* **Compra Finalizada:** Una vez confirmada la transferencia bancaria, el pedido se procesa y se envía al cliente.  
* **Actualización de Inventario:** El stock de un producto se actualiza automáticamente al completar una compra.

  #### **Cálculos:**

* **Total del Pedido:** El total del pedido se calcula sumando los precios de todos los productos en el carrito.  
* **Subtotal del Detalle:** El subtotal de cada artículo en el pedido se calcula multiplicando la cantidad de productos por su precio unitario.  
* **Descuentos y Promociones:** Si se aplican descuentos o promociones, el total del pedido se recalcula automáticamente.

  #### **Inferencias:**

* **Disponibilidad para Compra:** Si el stock de un producto es mayor que cero, el producto está disponible para su compra.  
* **Notificación de Stock:** Si el producto está agotado, se muestra una notificación de "Sin stock", pero el producto sigue visible en el catálogo para consultas.  
* **Validación de Usuario:** Un usuario es válido para iniciar sesión si su nombre de usuario y contraseña coinciden con los datos registrados en el sistema.