# One-vs-Rest classifier (a.k.a. One-vs-All)

#¿Qué es?
OVA (one-versus-all) es un modelo de clasificación binaria, donde se aprende a distinguir una clase específica del resto de las clases. El i-ésimo clasificador binario genera una respuesta  ri ≡ para el vector de entrada x. Cada respuesta corresponde a un elemento del vector, definido como r = [r1, . . . , rc], el cual es la entrada de una estrategia de agregación.

#Ventajas
-Este enfoque es relativamente razonable cuando la cantidad total de clases es pequeña.
-Usado comúnmente para algoritmos que predicen naturalmente la probabilidad o puntaje de membresía de clase numérica
