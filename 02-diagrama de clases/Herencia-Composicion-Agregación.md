Las diferencias entre asociación, composición y herencia son fundamentales en la programación orientada a objetos. Aquí te explico cada uno de estos conceptos:

### 1. Herencia
- **Definición**: La herencia es un mecanismo que permite que una clase (subclase o clase derivada) herede atributos y métodos de otra clase (superclase o clase base).
- **Ejemplo**: Si tienes una clase `Animal`, puedes tener una subclase `Perro` que herede las propiedades de `Animal`, como `especie`, `edad`, etc.
- **Relación**: "Es un" (un perro es un animal).
- **Características**:
  - Promueve la reutilización de código.
  - Permite la creación de jerarquías de clases.
  - Puede dar lugar a problemas como el "problema de la herencia múltiple" en algunos lenguajes.

### 2. Composición
- **Definición**: La composición es una relación entre objetos en la que un objeto (el contenedor) está compuesto por uno o más objetos (componentes). Si se elimina el contenedor, los componentes también se destruyen.
- **Ejemplo**: Una clase `Coche` puede tener una clase `Motor` como parte de su composición. Si el `Coche` se elimina, el `Motor` también deja de tener sentido.
- **Relación**: "Tiene un" (un coche tiene un motor).
- **Características**:
  - Promueve la reutilización y flexibilidad.
  - Permite cambiar componentes sin afectar a otros.
  - Es más robusta frente a cambios en la implementación.

### 3. Asociación
- **Definición**: La asociación es una relación más general entre dos o más objetos, donde cada objeto puede existir independientemente del otro. Puede ser unidireccional o bidireccional.
- **Ejemplo**: Una clase `Profesor` puede asociarse con una clase `Estudiante`, donde un `Profesor` puede enseñar a varios `Estudiantes` y un `Estudiante` puede ser enseñado por varios `Profesores`.
- **Relación**: "Conoce a" (un profesor conoce a un estudiante).
- **Características**:
  - Más flexible y menos restrictiva que la herencia o la composición.
  - Permite establecer relaciones más complejas y dinámicas.
  - No implica una relación de propiedad; los objetos pueden existir por separado.

### Resumen de las diferencias
- **Herencia**: Relación de tipo "es un", implica jerarquía y reutilización de código.
- **Composición**: Relación de tipo "tiene un", los objetos están fuertemente acoplados; si uno se destruye, el otro también.
- **Asociación**: Relación de tipo "conoce a", más flexible y permite que los objetos existan de forma independiente.

Estos conceptos son cruciales para diseñar sistemas de software robustos y mantenibles.