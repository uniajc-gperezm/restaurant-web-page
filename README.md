# Restaurant Webpage

## Explicacion Propiedades CSS

### 1. **Propiedades de Flexbox**
Flexbox es un modelo de diseño que permite la disposición de elementos en un espacio unidimensional. Es particularmente útil para crear diseños responsivos.

- **`display: flex;`**: Esta propiedad habilita el diseño flexbox en el contenedor. Permite que los elementos secundarios (elementos flexibles) se dispongan en una fila o columna.

- **`flex-direction: column;`**: Esta propiedad define la dirección en la que se colocan los elementos flexibles en el contenedor. Configurarlo como `column` apila los elementos verticalmente.

- **`justify-content: space-between;`**: Esta propiedad alinea los elementos flexibles a lo largo del eje principal (horizontal por defecto). `space-between` distribuye los elementos uniformemente, con el primer elemento al inicio y el último al final del contenedor.

- **`align-items: center;`**: Esta propiedad alinea los elementos flexibles a lo largo del eje cruzado (vertical por defecto). `center` centra verticalmente los elementos dentro del contenedor flexible.

### 2. **Propiedades de Fondo**
Las propiedades de fondo se utilizan para establecer el fondo de un elemento.

- **`background: linear-gradient(...)`**: Esta propiedad crea un fondo de degradado. La función `linear-gradient` toma paradas de color como parámetros, permitiendo transiciones suaves entre colores.

- **`background-size: cover;`**: Esta propiedad especifica que la imagen de fondo debe cubrir toda el área del elemento, potencialmente recortando la imagen para mantener su relación de aspecto.

- **`background-repeat: no-repeat;`**: Esta propiedad evita que la imagen de fondo se repita, asegurando que solo aparezca una vez.

### 3. **Propiedades de Transformación y Transición**
Estas propiedades se utilizan para animaciones y transformaciones de elementos.

- **`transform: translate(-50%, -50%);`**: Esta propiedad mueve un elemento desde su posición actual. Los valores `-50%` para ambos ejes X e Y centran el elemento desplazándolo hacia la izquierda y hacia arriba en la mitad de su propio ancho y altura.

- **`transition: all 0.3s ease-in-out;`**: Esta propiedad permite transiciones suaves entre cambios de propiedades. La palabra clave `all` indica que todas las propiedades se transicionarán, `0.3s` especifica la duración y `ease-in-out` define la función de temporización, haciendo que la transición comience y termine lentamente.

### 4. **Pseudo-elementos y Pseudo-clases**
Estos son selectores especiales que permiten el estilo de partes específicas de los elementos.

- **`::after`**: Este pseudo-elemento se utiliza para insertar contenido después de un elemento. En el código proporcionado, se utiliza para crear una superposición semitransparente sobre las imágenes.

- **`:hover`**: Esta pseudo-clase aplica estilos cuando el usuario pasa el cursor sobre un elemento. Se utiliza comúnmente para elementos interactivos como botones y enlaces.

### 5. **Consultas de Medios**
Las consultas de medios se utilizan para el diseño responsivo, permitiendo que los estilos cambien según el tamaño de la ventana gráfica.

- **`@media (max-width: 780px)`**: Esta consulta de medios aplica estilos solo cuando el ancho de la ventana gráfica es de 780 píxeles o menos. Se utiliza para ajustar diseños para pantallas más pequeñas, como dispositivos móviles.

- **`flex-wrap: wrap;`**: Esta propiedad permite que los elementos flexibles se envuelvan en múltiples líneas si exceden el ancho del contenedor. Es particularmente útil en diseños responsivos.

### 6. **Opacidad y Z-index**
Estas propiedades controlan la visibilidad y el orden de apilamiento de los elementos.

- **`opacity: 0;`**: Esta propiedad establece el nivel de transparencia de un elemento. Un valor de `0` hace que el elemento sea completamente transparente (invisible).

- **`z-index: 2;`**: Esta propiedad controla el orden de apilamiento de los elementos posicionados. Un valor de `z-index` más alto significa que el elemento estará encima de los elementos con valores más bajos.

### 7. **Object-fit y Object-position**
Estas propiedades se utilizan para controlar cómo se muestran las imágenes dentro de sus contenedores.

- **`object-fit: cover;`**: Esta propiedad especifica cómo debe redimensionarse una imagen para ajustarse a su contenedor. `cover` asegura que la imagen cubra todo el contenedor mientras mantiene su relación de aspecto.

- **`object-position: center;`**: Esta propiedad define la alineación de la imagen dentro de su contenedor. `center` asegura que la imagen esté centrada tanto horizontal como verticalmente.

### 8. **Clip-path**
La propiedad `clip-path` se utiliza para crear formas recortadas en elementos. Permite definir una región visible de un elemento, ocultando el resto. Esto se puede hacer utilizando formas básicas (como círculos o elipses) o rutas SVG complejas.

- **`clip-path: circle(50%);`**: Esta propiedad recorta el elemento en forma de círculo, donde el valor `50%` define el radio del círculo en relación con el tamaño del elemento.

- **`clip-path: polygon(...);`**: Esta propiedad permite definir un polígono mediante coordenadas, creando formas personalizadas para recortar el elemento.

<!-- ## CSS Properties Explained

### 1. **Flexbox Properties**
Flexbox is a layout model that allows for the arrangement of elements in a one-dimensional space. It is particularly useful for creating responsive layouts.

- **`display: flex;`**: This property enables the flexbox layout on the container. It allows child elements (flex items) to be arranged in a row or column.

- **`flex-direction: column;`**: This property defines the direction in which the flex items are placed in the flex container. Setting it to `column` stacks the items vertically.

- **`justify-content: space-between;`**: This property aligns flex items along the main axis (horizontal by default). `space-between` distributes the items evenly, with the first item at the start and the last item at the end of the container.

- **`align-items: center;`**: This property aligns flex items along the cross axis (vertical by default). `center` vertically centers the items within the flex container.

### 2. **Background Properties**
Background properties are used to set the background of an element.

- **`background: linear-gradient(...)`**: This property creates a gradient background. The `linear-gradient` function takes color stops as parameters, allowing for smooth transitions between colors.

- **`background-size: cover;`**: This property specifies that the background image should cover the entire area of the element, potentially cropping the image to maintain its aspect ratio.

- **`background-repeat: no-repeat;`**: This property prevents the background image from repeating, ensuring it only appears once.

### 3. **Transform and Transition Properties**
These properties are used for animations and transformations of elements.

- **`transform: translate(-50%, -50%);`**: This property moves an element from its current position. The values `-50%` for both X and Y axes center the element by shifting it left and up by half of its own width and height.

- **`transition: all 0.3s ease-in-out;`**: This property allows for smooth transitions between property changes. The `all` keyword indicates that all properties will transition, `0.3s` specifies the duration, and `ease-in-out` defines the timing function, making the transition start and end slowly.

### 4. **Pseudo-elements and Pseudo-classes**
These are special selectors that allow for styling of specific parts of elements.

- **`::after`**: This pseudo-element is used to insert content after an element. In the provided code, it is used to create a semi-transparent overlay on images.

- **`:hover`**: This pseudo-class applies styles when the user hovers over an element. It is commonly used for interactive elements like buttons and links.

### 5. **Media Queries**
Media queries are used for responsive design, allowing styles to change based on the viewport size.

- **`@media (max-width: 780px)`**: This media query applies styles only when the viewport width is 780 pixels or less. It is used to adjust layouts for smaller screens, such as mobile devices.

- **`flex-wrap: wrap;`**: This property allows flex items to wrap onto multiple lines if they exceed the width of the container. It is particularly useful in responsive designs.

### 6. **Opacity and Z-index**
These properties control the visibility and stacking order of elements.

- **`opacity: 0;`**: This property sets the transparency level of an element. A value of `0` makes the element fully transparent (invisible).

- **`z-index: 2;`**: This property controls the stacking order of positioned elements. A higher `z-index` value means the element will be on top of elements with lower values.

### 7. **Object-fit and Object-position**
These properties are used for controlling how images are displayed within their containers.

- **`object-fit: cover;`**: This property specifies how an image should be resized to fit its container. `cover` ensures the image covers the entire container while maintaining its aspect ratio.

- **`object-position: center;`**: This property defines the alignment of the image within its container. `center` ensures the image is centered both horizontally and vertically. -->
