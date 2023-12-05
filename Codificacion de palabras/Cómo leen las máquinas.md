
En primer lugar, tenemos una representación del texto de manera natural, es decir, tenemos unas reglas ortográficas y un contenido semántico $\rightarrow$ Existen unas reglas que diferencian el proceso de comunicación.

El primer problema que encontramos es codificar todas estas reglas $\rightarrow$ Aplicar técnicas de ML/DL. Podemos tener un corpus de entrada y pasarlo a las [[Redes Neuronales]], pero solo leen datos de numéricos, de forma
que necesitamos codificar (pasar a formato numérico) ese input $\rightarrow$ Encoding

Tipos de división:
- División por palabras
- División por subpalabras
- División por caracteres

Este proceso se denomina [[Tokenización]].