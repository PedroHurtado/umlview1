Un diagrama de actividades (activity diagram) en UML es una representación visual de los flujos de trabajo y procesos dentro de un sistema. Se utiliza para mostrar el flujo de control o de datos de una actividad a otra y es particularmente útil para modelar procesos complejos. Aquí tienes los elementos clave de un diagrama de actividades:

```yuml
// {type:usecase}
// {generate:true}
// Actores
[Usuario]-(Ver lista de pizzas)
[Usuario]-(Ver detalles de pizza)
[Usuario]-(Calcular precio de pizza)
 
[Administrador]-(Crear pizza)
(Crear pizza)<(Añadir ingrediente a pizza)
[Administrador]-(Actualizar pizza)
[Administrador]-(Eliminar pizza)
[Administrador]-(Añadir ingrediente a pizza)
[Administrador]-(Eliminar ingrediente de pizza)
[Administrador]-(Crear ingrediente)
[Administrador]-(Actualizar ingrediente)
```

### 1. **Actividades**
   - **Descripción**: Representan las tareas o acciones que se realizan dentro del proceso.
   - **Símbolo**: Se dibujan como rectángulos con bordes redondeados.
   - **Ejemplo**: "Enviar Correo", "Procesar Pago".

### 2. **Flujos de Control**
   - **Descripción**: Indican la dirección del flujo entre actividades.
   - **Símbolo**: Se representan con flechas que conectan actividades, decisiones, y otros elementos.
   - **Ejemplo**: Una flecha desde "Iniciar Proceso" a "Enviar Correo".

### 3. **Decisiones**
   - **Descripción**: Representan puntos en los que se toma una decisión que afectará el flujo de control.
   - **Símbolo**: Se dibujan como rombos.
   - **Ejemplo**: "¿Pago Aprobado?" que dirige a diferentes actividades basadas en la respuesta.

### 4. **Uniones**
   - **Descripción**: Usadas para combinar múltiples flujos en uno solo.
   - **Símbolo**: Se representa como un rombo (similar a una decisión) donde convergen múltiples flechas.
   - **Ejemplo**: Combina flujos que provienen de múltiples decisiones.

### 5. **Inicio (Start)**
   - **Descripción**: Indica el inicio del flujo de actividades.
   - **Símbolo**: Se representa como un círculo sólido.
   - **Ejemplo**: Un círculo que señala el comienzo del proceso.

### 6. **Fin (End)**
   - **Descripción**: Representa el final del flujo de actividades.
   - **Símbolo**: Se representa como un círculo con un borde grueso alrededor de un círculo sólido.
   - **Ejemplo**: Un círculo con un borde exterior que indica que se ha completado el proceso.

### 7. **Subactividades (Sub-activities)**
   - **Descripción**: Actividades que pueden ser desglosadas en más actividades o flujos. Ayudan a mantener el diagrama limpio y organizado.
   - **Símbolo**: Se representan como un rectángulo con bordes redondeados que incluye el nombre de la subactividad.
   - **Ejemplo**: Una actividad "Gestión de Pedido" que se divide en "Recibir Pedido", "Procesar Pedido", "Enviar Confirmación".

### 8. **Nodos de Control (Control Nodes)**
   - **Descripción**: Puntos donde se puede controlar el flujo de actividades.
   - **Tipos**:
     - **Fork**: Separa el flujo en múltiples flujos paralelos (representado como una línea horizontal o vertical).
     - **Join**: Combina múltiples flujos en uno solo.
   - **Ejemplo**: Un fork podría separar el flujo de "Enviar Correo" y "Generar Reporte" en dos actividades simultáneas.

### 9. **Notas (Notes)**
   - **Descripción**: Proporcionan información adicional sobre ciertas actividades o decisiones.
   - **Símbolo**: Se representan como un rectángulo con un borde en forma de línea punteada.
   - **Ejemplo**: Una nota que explica el objetivo de una actividad.

### 10. **Particiones (Swimlanes)**
   - **Descripción**: Usadas para organizar actividades y mostrar qué actor o entidad es responsable de cada actividad.
   - **Símbolo**: Se dibujan como rectángulos que dividen el diagrama en secciones.
   - **Ejemplo**: Particiones para "Cliente", "Sistema", "Administrador".

### Ejemplo de Diagrama de Actividades
Un diagrama de actividades típico podría mostrar el flujo de un proceso de compra en línea, comenzando desde "Iniciar Compra", pasando por decisiones como "¿Artículos en Carrito?", realizando actividades como "Procesar Pago", y terminando en "Confirmar Pedido".

### Resumen
Los diagramas de actividades son herramientas poderosas para visualizar procesos, ayudando a identificar áreas de mejora, optimizar flujos de trabajo, y comunicar procesos a interesados. Al comprender estos elementos, puedes crear diagramas que representen de manera clara y efectiva la dinámica de cualquier proceso o sistema.