
 El coste representa lo alejado que se está del resultado deseado, por lo que querremos minimizar su valor.  El método gradiente descendiente permite minimizar una función. Para ello, 
 partiendo de unos valores para los parámetros elegidos aleatoriamente, avanza en pasos sucesivos hacia un mínimo.

- **Hipótesis**: El valor a reducir decrece rápidamente si, en cada paso, se aplica un corrector negativo. 
		$\rightarrow$ El corrector se obtiene de la derivada parcial en el peso a establecer computado.
		$\rightarrow$ La aplicación de cada gradiente sobre cada peso aumenta la posibilidad de caer en óptimos locales. En su lugar, aplicamos un factor de aprendizaje (ratio) que en cada iteración,
		el valor de un peso se actualiza: $$wi_{t+1} = wi_t * (1 – ratio) – (ratio * gradient)$$
Tomando una función cualquiera F($\theta_0$, $\theta_1$) $\rightarrow$ Queremos minimizar F $\rightarrow$  Partimos de unos valores $\theta_0$ y $\theta_1$ elegidos aleatoriamente $\rightarrow$ Actualizamos   $\theta_0$ y $\theta_1$ mientras se reduzca F

![[Descenso por gradiente img.png]]

# Algoritmo

*Inicializar aleatoriamente $\theta_0$ y $\theta_1$*

*Repetir hasta convergencia {*$$\theta _{j}:=\theta _{j}-\alpha \dfrac{\partial }{\partial \theta _{j}}F\left( \theta _{0},\theta _{1}\right)(Para\quad j=0\quad y\quad j = 1,\quad \alpha > 0)$$
*}*

## Anotaciones

- El signo de la derivada marcará si $\theta_1$ crece o decrece y, cuando la derivada de la tangente sea 0, se estanca en un valor.
			· La derivada parcial de la función representa la recta tangente.

- Cuando el valor de los parámetros se aproxima a un mínimo, el algoritmo da pasos más pequeños, ya que dF($\theta_1$) es menor. Entonces, no se necesario decrementar $\alpha$ 
	a lo largo de las iteraciones, pero sí debemos fijar un valor aceptable.

## Valor de $\alpha$

Se denomina razón/coeficiente de aprendizaje. Casos:

- Si $\alpha$ es demasiado pequeña, la convergencia puede ser demasiado lenta.
- Si $\alpha$ es demasiado grande, el algoritmo puede no converger, o incluso divergir.

## Convergencia

El método del gradiente descendiente siempre convergerá a un óptimo local que, en algunos casos, coincidirá con el global.

![[Optimos img.png]]

El punto hacia el que converge el algoritmo depende de los valores iniciales de los parámetros. Ejemplo de dos puntos de partidas diferentes en el mínimo de convergencia:

![[Convergencia img.png]]
