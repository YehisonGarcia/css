# Hallazgos: El Modelo de Caja
(1) La diferencia práctica entre Margin y Padding
La diferencia es que Margin es el espacio externo de un elemento, es decir, la distancia que existe entre una caja y los demás elementos y el Padding es el espacio interno que hay entre el contenido y el borde de la caja.

(2) Por qué es obligatorio usar box-sizing: border-box
Porque permite que el tamaño de una caja se mantenga dentro de las medidas que establecemos, Esto facilita organizar los elementos y evita que las cajas sean mas grande de lo esperado.

(3) Cómo se ven afectados los elementos hermanos cuando le aplicas un margen grande a uno de ellos.
Puede generar una mayor separación con los elementos que están a su alrededor.

# Hallazgos: Centralización de Identidad Visual y Espaciado
(1) La lista completa de variables declaradas (colores y espaciados)

--color-primario: #1f47c0

--color-secundario: #6a88e0

--color-background: #011142

--color-texto: #fff

--fuente-principal: "PT Sans", sans-serif

--espaciado-medio: 16px

--espaciado-grande: 24px

(2) La ventaja de reutilizar medidas de margen y relleno en lugar de inventar valores en cada selector
Asegura un ritmo visual coherente, evita valores arbitrarios y simplifica la actualización global del diseño modificando un único punto de referencia.

(3) De qué manera la centralización en :root previene colisiones visuales a medida que la hoja de estilos crece.
Establece un estándar único que frena la fragmentación de estilos, aísla la lógica visual y mantiene la armonía gráfica a medida que el proyecto escala.

# Hallazgos: Pseudoclases y Pseudoelementos

Durante el desarrollo e implementación de interactividad y mejoras de experiencia de usuario (UX) en la interfaz, se identificaron los siguientes conceptos clave:

# 1 Diferencia funcional entre pseudoclase y pseudoelemento:

Pseudoclase (:hover, :active, :focus): Su función principal es reaccionar al estado dinámico o a las acciones del usuario sobre un elemento existente (por ejemplo, cuando se pasa el cursor por encima, se hace clic o se selecciona con el teclado). Cambian el comportamiento o estilo del elemento según la interacción.

Pseudoelemento (::before, ::after): Su función es inyectar contenido visual o elementos decorativos que no existen originalmente en el marcado HTML. Permiten estructurar partes gráficas (como insignias o líneas) directamente desde la capa de estilos.

# 2 Importancia técnica de la pseudoclase :focus en accesibilidad web:
La utilización de :focus (acompañado de un outline visible y personalizado) es una buena práctica indispensable de accesibilidad (a11y). Permite que los usuarios que navegan mediante el uso de la tecla Tab o tecnologías de asistencia identifiquen claramente en qué elemento interactivo se encuentran posicionados, evitando la pérdida de contexto visual al eliminar los contornos por defecto sin un reemplazo adecuado.

# 3 Ventajas de inyectar elementos decorativos desde CSS (::before/::after):
Inyectar contenido o insignias visuales (como etiquetas de "¡Nuevo!" o iconos) mediante pseudoelementos mantiene el archivo HTML limpio, semántico y enfocado únicamente en la estructura de la información. Evita saturar el marcado con etiquetas o contenedores vacíos cuya única función sea estética, delegando toda la responsabilidad visual y decorativa a la hoja de estilos.