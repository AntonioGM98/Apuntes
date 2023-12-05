La clasificación de los textos en NLP implica la asignación de una etiqueta/categoría a un documento en función de su contenido. Esto tiene gran variedad de 
aplicaciones como filtrado de spam, categorización de noticias, detección de sentimientos en redes sociales, etc.

Pero, el primer paso que debemos tomar será el [[Procesamiento y limpieza de texto]].

## Bolsa de palabras

Se utiliza comúnmente en la clasificación de documentos para los vectores de características. 

Es la frecuencia de aparición de cada palabra en esos documentos y se utiliza como característica para entrenar un clasificador.

### Carencias

- Vectores de documentos grandes (si tenemos un vocabulario muy grande) y muy escasos (muchos 0's)
- Se pierde la gramática y el orden de las palabras y, por tanto, el contexto
- Semánticamente débil por la pérdida de contexto

### Mejoras

-  Vectores TF-IDF: Penaliza las palabras que se repiten en muchos documentos partiendo de que implicaría menor valor en cuanto información.
$$TF\left(t\right)\:=\:\frac{Nº\:de\:veces\:que\:aparece\:el\:término\:t\:en\:un\:documento}{Nº\:total\:de\:términos\:que\:hay\:en\:el\:documento}$$
$$IDF\left(t\right)\:=\:\log _e\left(\frac{Nº\:total\:de\:docs}{Nº\:de\:docs\:con\:el\:término\:t\:en\:él}\right)$$
- Bolsa de n-agramas: Construye bigramas, trigramas ó n-agramas en dos palabras como, por ejemplo: *This is not a good movie* $\rightarrow$ *This not, not good, good movie* **(Bigramas)**


En resumen, puede funcionar bien, pero se puede perder el contexto e ignora la semántica, por lo que sirve como base pero habría que considerar otras opciones.