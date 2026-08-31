Markdown
# Sistema de Entregas SpeedFast - Semana 3

Proyecto desarrollado en Java utilizando IntelliJ IDEA Ultimate, enfocado en la aplicación de los pilares de la Programación Orientada a Objetos (POO), incluyendo clases abstractas, polimorfismo, sobrecarga e interfaces.

## Descripción del Proyecto
SpeedFast es un sistema de gestión de entregas que modela diferentes tipos de pedidos (comida, encomienda y express) a partir de una clase abstracta base y la implementación de contratos mediante interfaces para garantizar la rastreabilidad, cancelación y despacho de los envíos.

## Estructura de Clases
* **`Pedido` (Clase Abstracta):** Define los atributos base comunes a cualquier envío (ID, dirección de destino, costo base) y métodos abstractos o concretos para la gestión de repartidores y resúmenes.
* **`PedidoComida`:** Extiende de `Pedido` e implementa comportamientos específicos para el área gastronómica.
* **`PedidoEncomienda`:** Extiende de `Pedido` incorporando lógica de peso y dimensiones para paquetes estándar.
* **`PedidoExpress`:** Extiende de `Pedido` para envíos prioritarios o de alta velocidad.
* **Interfaces Implementadas:**
  * `Despachable`: Controla las operaciones de salida y despacho.
  * `Cancelable`: Gestiona la anulación de envíos bajo ciertas condiciones.
  * `Rastreable`: Permite el seguimiento del estado del paquete.
* **`Main`:** Clase principal encargada de la ejecución, instanciación de objetos y demostración de polimorfismo y asignación de repartidores (tanto automática como manual mediante sobrecarga de métodos).

## Tecnologías Utilizadas
* **Lenguaje:** Java
* **IDE:** IntelliJ IDEA
* **Control de Versiones:** Git y GitHub
