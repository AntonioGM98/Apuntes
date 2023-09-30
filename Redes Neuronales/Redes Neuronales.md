Surgen como modo de simular el comportamiento de las redes neuronales biológicas.
## Perceptrón

Precursor de las redes neuronales. de mayores capas. compuesto por una única [[Neurona]].
Los parámetros que tendrá que establecer por el usuario de la red serán:
	- Topología: Tipo, nº de capas ocultas y las conexiones entre ellas.
	- Función de activación
	- Ratio de aprendizaje, o
	- Capa de salida (en función del problema), como el uso de la función Softmax.

## Perceptrón Multicapa (RNA)

Caso que vamos a encontrar que se conforma por una red de [[Neurona]]s, también llamado topología neuronal.
En ella distinguimos tres capas: [[Input layer]], [[Hidden layer]] y [[Output layer]].

A tener en cuenta en la preparación de los datos para las redes neuronales:
- Los datos deben de ser numéricos, es decir, deberemos aplicar One Hot Encoding o una codificación de etiquetas.
- Deben estar normalizados, para mejorar la ponderación evitando tratar con valores muy altos.

Este modelo toma N-entradas (x$_1$, . . . , x$_n$) y genera una salida a partir de una función que utiliza una serie de pesos (w$_1$, . . ., w$_n$), y un sesgo (b).

### Características

- El número de capas ocultas aumenta la complejidad de la red:
	- Afecta al proceso de clasificación, pero sobre todo aumenta la complejidad del aprendizaje.
- El proceso de aprendizaje se puede ver como la búsqueda de reducir un valor, el **coste** $\rightarrow$ Representa lo lejos que está la red de producir un resultado perfecto.

### Topologías

- [[Feed Forward]]
- [[Recurrent NN]]

## Aprendizaje de la red
### Propagación hacia delante

Proceso mediante el cual una red neuronal realiza cálculos para procesar datos de entrada y generar una predicción o salida. Este proceso ocurre en tres etapas principales: entrada, 
cálculo en capas ocultas y cálculo en la capa de salida. También se utiliza después de haber entrenado la red para hacer predicciones sobre nuevos datos.

En ambos casos, la salida de la red se comparará con la salida esperada y se calcula el error.

### Propagación hacia atrás

Tras haber realizado esta propagación, el error se propaga de vuelta a través de la red. 
Por cada capa, se actualizan los pesos de cada nodo de acuerdo a su contribución al error resultante. Este proceso se repetirá para todos los ejemplos que tengamos.


Una técnica fundamental en el entrenamiento de redes neuronales, y para minimizar la función de pérdida es el [[Descenso por gradiente]].
