Esta estrategia consiste en crear una columna binaria (que solo puede contener los valores 0 o 1) para cada valor único que exista en la variable categórica que estamos 
codificando, y marcar con un 1 la columna correspondiente al valor presente en cada registro, dejando las demás columnas con un valor de 0.

De esta manera, cada registro queda representado por un vector binario que indica la presencia o ausencia de cada valor categórico, y se evita la posibilidad de que 
los algoritmos malinterpreten los valores numéricos.