# Nombre: Christian Guantay
# Padron: 98538
# Repositorio de Github: 

<h1> Paso 0 - Entorno de trabajo: </h1>

a)

![0.Paso 0 - Ej](/taller-tp0/punto0.png)
![0.Paso 0 - Valgrind](/taller-tp0/punto0-valgrind.png)

b) Valgrind es una herramienta utilizada para analizar el manejo de memoria en un programa en ejecucion.
La opciones mas comunes son memcheck y leak-check, la primera chequea todos los accessos de memoria y los valores computados que realiza nuestro programa mientras
que la segunda chequea fugas de memoria.

c) **sizeof()** es un operador del lenguaje C que representa el tamaño en bytes de un tipo de dato. Si tenemos un tipo de dato **char**, de acuerdo a la arquitectura utilizada por la computadora donde se ejecuto el presente trabajo practico, el valor de salida sera de 1 byte. Para el tipo de dato **int** sera de 4 bytes.

d) No es siempre el caso. Supongamos que tengo un **struct** compuesto por los tipos de dato que analizamos anteriormente, un **char** y un  **int**. 
La suma de estos datos por separado nos da 5 bytes pero el **sizeof()** del **struct** propuesto resultara de 8 bytes. Esto se debe al padeo o **padding**
que realiza la arquitectura de nuestro programa con el tipo de dato **char** debido a la presencia del dato **int**.

e)
!(/taller-tp0/punto1-error-gen.png)


