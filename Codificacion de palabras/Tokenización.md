Proceso de división de las palabras, es decir, cómo se van a dividir las palabras, donde, cada elemento, se llamará Token.
![[Tokenizacion img.png]]

A lo largo del proceso vamos a buscar la asignación de una etiqueta numérica a cada Token, contando con que cada palabra debe tener siempre el mismo y 
único valor numérico.

Un problema que se plantea con estas asignaciones, es que los modelos de ML se basan en distancias numéricas, de forma que al dar identificadores a palabras 
da lugar a una idea incorrecta, ya que no estarán bien representadas o asignará distancias no reales. Por ejemplo:

![[Problema tokenizacion img.png]]

Una solución presente a este problema es el [[One Hot Encoding]], por lo que cada palabra estará conformada por un vector, cuyo tamaño es el del número de elementos del 
vocabulario. Y con esta solución, si tomamos el ejemplo anterior, evitamos el inconveniente de la distancia, ya que será constante entre todas las palabras.

Por otra parte, el problema de esta solución, es que crece exponencialmente, creando vectores muy densos y dispersos, ya que, para representar una palabra, todos los 
elementos serán 0 menos el de la palabra.
También, debemos tener en cuenta que la distancia entre Python y R tendrá que ser menor que con sofá, ya que sabemos que son lenguajes de programación y están más
relacionados entre sí.

Entonces, necesitamos introducir la relación entre las palabras, este proceso consistirá en pasar de OHE a [[Embedding]].