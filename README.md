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