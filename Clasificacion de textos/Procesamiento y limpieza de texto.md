- Eliminar símbolos HTML
- Tokenizar el texto
- Convertir todas las palabras a minúsculas
- Eliminar todo lo que no sean letras, es decir, número, signos de puntuación, etc
- Eliminar las **stop words** (Palabras que no aportan información al documento)
- Obtención de la raíz, mediante:
	- [[Lematizacion]]
	- [[Stemming]]



Según el problema que esté enfrentando, debemos tener en cuenta situaciones como las siguientes:

- :( $\rightarrow$ Puede ser una puntuación o un sentimiento
- Las mayúsculas con exclamaciones pueden ser indicativas de spam

También tenemos a nuestra disposición librerías que abstraen esa complejidad del texto mediante expresiones regulares como **NLTK**.

Ejemplo:

![[Ejemplo NLTK img.png]]