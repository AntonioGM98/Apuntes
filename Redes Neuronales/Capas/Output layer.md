Es la última capa de nodos, cuya función es generar las predicciones en base al procesamiento de la información que ha tenido lugar en las capas anteriores. 

La configuración de la capa de salida depende de la naturaleza del problema u objetivo de la red:

- **Clasificación**: Estará compuesta por un único nodo por cada clase posible y función de activación softmax, para los problemas multiclase. En caso de clasificación binaria, tendremos un nodo aplicando 
  la función de activación sigmoidal y, obteniendo 0 ó 1, en función del más próximo a la salida. La salida se interpreta como la probabilidad de pertenencia a cada clase y, la que tenga mayor valor, 
  se considera como predicción final.

- **Regresión**: Al buscar predecir valores numéricos continuos, aplicaremos un único nodo de salida y puede tener, o no, función de salida.

- **Generación de secuencias**: Al necesitar que la red genere una secuencia de datos, como en el [[Natural Language Processing (NLP)]], la capa de salida puede tener tantos nodos como símbolos o categorías 
  podamos encontrar en la secuencia de salida.