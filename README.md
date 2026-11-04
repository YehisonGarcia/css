# Hallazgos: El Modelo de Caja
(1) La diferencia práctica entre Margin y Padding
La diferencia es que Margin es el espacio externo de un elemento, es decir, la distancia que existe entre una caja y los demás elementos y el Padding es el espacio interno que hay entre el contenido y el borde de la caja.

(2) Por qué es obligatorio usar box-sizing: border-box
Porque permite que el tamaño de una caja se mantenga dentro de las medidas que establecemos, Esto facilita organizar los elementos y evita que las cajas sean mas grande de lo esperado.

(3) Cómo se ven afectados los elementos hermanos cuando le aplicas un margen grande a uno de ellos.
Puede generar una mayor separación con los elementos que están a su alrededor.