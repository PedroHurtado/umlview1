Las relaciones `include` y `extend` en un diagrama de casos de uso de UML son fundamentales para modelar la funcionalidad y los comportamientos de un sistema. A continuación se detallan las diferencias clave entre ambas:

### 1. **Include (Inclusión)**
- **Definición**: La relación `include` se utiliza para mostrar que un caso de uso incluye o llama a otro caso de uso como parte de su proceso. Es una relación obligatoria, lo que significa que el caso de uso que incluye siempre invoca al caso de uso incluido.
- **Uso**:
  - Se aplica cuando hay funcionalidad común que se utiliza en varios casos de uso.
  - Ayuda a evitar la duplicación de código y a centralizar el comportamiento común.
- **Ejemplo**: 
  - Imagina un caso de uso "Procesar Pedido". Este caso de uso podría incluir "Calcular Envío", ya que calcular el envío es una parte necesaria del proceso de procesamiento del pedido.

### 2. **Extend (Extensión)**
- **Definición**: La relación `extend` se utiliza para mostrar que un caso de uso puede extender la funcionalidad de otro caso de uso en ciertas condiciones. Es una relación opcional, lo que significa que el caso de uso extendido no siempre se invoca.
- **Uso**:
  - Se aplica cuando hay comportamientos adicionales que solo se ejecutan bajo ciertas condiciones o circunstancias.
  - Permite agregar características opcionales a un caso de uso base sin modificar su definición.
- **Ejemplo**:
  - Considera el caso de uso "Realizar Pago". Este caso de uso puede extenderse a "Validar Tarjeta" que se activa solo si el usuario selecciona el pago con tarjeta. Si el usuario elige el pago en efectivo, no se invoca la validación.

### Resumen de Diferencias

| Característica   | Include                                | Extend                                   |
|------------------|----------------------------------------|-----------------------------------------|
| **Tipo de Relación** | Obligatoria                            | Opcional                                 |
| **Ejemplo**      | "Procesar Pedido" incluye "Calcular Envío" | "Realizar Pago" extiende "Validar Tarjeta" |
| **Propósito**    | Para reutilizar funcionalidad común      | Para agregar funcionalidad adicional     |
| **Llamadas**     | Siempre se invoca                      | Solo se invoca bajo ciertas condiciones   |

Estas diferencias son cruciales para modelar adecuadamente los casos de uso y comprender cómo interactúan los diferentes componentes dentro de un sistema.