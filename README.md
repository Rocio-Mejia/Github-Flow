# One-vs-Rest classifier (a.k.a. One-vs-All)

##**¿Qué es?**

OVA (one-versus-all) es un modelo de clasificación binaria, donde se aprende a distinguir una clase específica del resto de las clases. El i-ésimo clasificador binario genera una respuesta  ri ≡ para el vector de entrada x. Cada respuesta corresponde a un elemento del vector, definido como r = [r1, . . . , rc], el cual es la entrada de una estrategia de agregación.

##**Ventajas**

-Este enfoque es relativamente razonable cuando la cantidad total de clases es pequeña.
-Usado comúnmente para algoritmos que predicen naturalmente la probabilidad o puntaje de membresía de clase numérica

##**Desventajas**

-Se vuelve cada vez más ineficiente a medida que aumenta la cantidad de clases.
-Requiere la creación de un modelo para cada clase.
-Con grandes conjuntos de datos, el modelo se vuelve lento(por ejemplo, redes neuronales) o con un gran número de clases (por ejemplo, cientos de clases).

##**Funcionamiento**

-Si el caso tiene n clases, One-Vs-All convierte su conjunto de datos de entrenamiento en n problemas de clasificación binaria.
-Para cada clase i, se asignan entradas de cualquier otra clase al conjunto de datos negativo y asigna entradas con clase i al conjunto de datos positivo. El conjunto de datos ahora es un conjunto de datos binario.
entrena un modelo, como la regresión logística para que se ajuste al conjunto de datos binarios. Este modelo determina la probabilidad de que una entrada dada pertenezca a la clase i (h (i) (x) = P (y = i), donde h (i) es el clasificador para la clase i).
-Después de tener un modelo para cada clase/etiqueta, es hora de determinar a qué clase (si tiene un problema multiclase) o a qué clases (si tiene un problema multilabel) cada entrada pertenece a:
Multiclase: elija la clase i,  si h(i)(x) devuelve la mayor probabilidad de cada clasificador.
Multilabel: para cada clase i, si h(i)(x) devuelve positivo, adjunte la clase i a esa entrada.


##**Colaboradores**
[LOPEZ VALENCIA LUIS DANIEL](https://github.com/Drani04)
[MARTINEZ IRIBE DAVID ERNESTO](https://github.com/DavidMtz1)
[MEJIA MANRIQUEZ ROCIO]
[MONTAÑO PELAYO RAUL ANTONIO]

