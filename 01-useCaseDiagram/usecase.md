Un diagrama de casos de uso en UML representa las interacciones de los usuarios (actores) con un sistema para lograr un objetivo específico. Los principales elementos de un diagrama de casos de uso son:


### 1. **Actores**
   - Representan roles o entidades externas que interactúan con el sistema, como usuarios humanos o sistemas externos.
   - Se dibujan como figuras de palo o simplemente un nombre entre corchetes (`[Actor]`).
   - Ejemplos de actores pueden ser "Cliente", "Administrador" o "Sistema de Pago".

### 2. **Casos de Uso**
   - Representan acciones o procesos que el sistema realiza en respuesta a una interacción de un actor. Un caso de uso es un objetivo o función específica, como "Realizar Pedido" o "Actualizar Perfil".
   - Se representan como óvalos, con el nombre del caso de uso dentro.
   - Los casos de uso son siempre verbos en infinitivo, pues describen la acción (por ejemplo, "Ver Producto").

### 3. **Sistema o Limite del Sistema**
   - Se usa un rectángulo para indicar el límite del sistema, dentro del cual se encuentran los casos de uso.
   - Representa el alcance del sistema que se está modelando y ayuda a diferenciar lo que ocurre dentro del sistema de lo que ocurre fuera.

### 4. **Relaciones entre Casos de Uso**
   - **Inclusión (`<<include>>`)**: Indica que un caso de uso siempre incluye el comportamiento de otro. Se utiliza cuando una acción se repite en varios casos de uso.
      - Ejemplo: En "Procesar Pedido", el caso de uso "Calcular Envío" puede incluirse, ya que siempre es parte del proceso.
   - **Extensión (`<<extend>>`)**: Muestra comportamiento opcional o condicional. Se utiliza cuando un caso de uso principal se amplía en ciertas condiciones.
      - Ejemplo: "Realizar Pago" puede tener un caso extendido "Validar Tarjeta", que solo se realiza si es necesario.
   - **Generalización**: Similar a la herencia entre clases, permite que un caso de uso hijo herede comportamientos del caso de uso padre.
      - Ejemplo: "Realizar Pago" puede generalizarse en "Pago con Tarjeta" y "Pago en Efectivo".

### 5. **Relaciones entre Actores y Casos de Uso**
   - Las líneas simples conectan actores con casos de uso para indicar las interacciones.
   - Una flecha simple puede señalar la dirección en la que se inicia la acción, aunque suele omitirse si el flujo es claro.

