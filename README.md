# ED-Unidad07: Actividades de Modelado UML

Este repositorio contiene la resolución de las actividades prácticas de la Unidad 07, centradas en el diseño de diagramas de Casos de Uso, Actividades y Estados para diversos sistemas digitales.

---

## 📂 Estructura del Repositorio

El repositorio está organizado siguiendo la estructura jerárquica solicitada para la entrega:

* **/Actividad 1**: Gestión de un Centro Deportivo.
* **/Actividad 2**: Máquina Expendedora de Metro.
* **/Actividad 3**: Sistema de Alarma Inteligente.
* **README.md**: Documentación general del proyecto.

---

## 📝 Explicación de los Diagramas

### Actividad 1: Sistema de Gestión de un Centro Deportivo
* **Casos de Uso**: Representa las interacciones de los Socios y el Administrador. Se ha aplicado una relación `include` para la verificación de pagos y una relación `extend` para la contratación opcional del seguro de lesiones.
* **Actividades**: Describe el flujo de reserva de una pista, desde la elección de fecha hasta la confirmación final o denegación por motivos económicos.

### Actividad 2: Máquina Expendedora de Billetes de Metro
* **Actividades**: Modela la lógica de pago. Se diferencia el proceso entre el uso de tarjeta (validación de PIN) y efectivo (gestión de cambio por parte de la máquina).
* **Estados**: Detalla el ciclo de vida de un billete, transitando por estados como "Emitido", "Validado" (al entrar en el torno) y "Agotado" o "Caducado".

### Actividad 3: Sistema de Control de una Alarma Inteligente
* **Estados**: Refleja el comportamiento dinámico del sistema. Destaca el estado "En Espera" (retardo de entrada de 30 segundos) y el acceso global al estado de "Mantenimiento" mediante llave técnica.
* **Casos de Uso**: Define las funciones principales del Propietario, integrando sensores de movimiento y la comunicación con la Central de Policía.

---

## 🔍 Justificación del Diseño

* **Actores**: Se han identificado tanto actores humanos (Socio, Propietario) como sistemas o dispositivos externos (Sensores, Banco, Policía) para dar una visión completa del entorno.
* **Relaciones**: El uso de `include` asegura que las reglas de negocio críticas (como estar al corriente de pago) se cumplan siempre, mientras que `extend` permite modelar opciones voluntarias.
* **Transiciones de Estado**: Se han definido eventos claros (introducir código, detectar movimiento, picar billete) para que los cambios de estado sean lógicos y sigan los requerimientos técnicos.

---

## 🛠️ Especificaciones de Formato
* **Diagramas**: Entregados en formato `.png` para garantizar su correcta visualización.
* **Legibilidad**: Se ha cuidado el etiquetado y la limpieza visual para facilitar su comprensión técnica.