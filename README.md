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

e) STDIN, STDOUT y STDERR son flujos predefinidos utilizados para la entrada, salida y el flujo de errores de un programa. Se puede utilizar el caracter < para 
redirigir la entrada de un flujo mientras que con el caracter > se puede redirigir la salida de un flujo. El caracter | sirve para poner juntos 2 flujos utilizando la salida de uno como la entrada de otro.


<h1> Paso 1 - SERCOM - Errores de generación y normas de programación: </h1>

a)![](/taller-tp0/punto1-error-estilo.png)


b)![](/taller-tp0/punto1-error-gen.png)

c)![](/taller-tp0/punto1-warning.png)

<h1> Paso 2 - SERCOM - Errores de generación 2: </h1>

![](/taller-tp0/punto2-diff-main.png)
![](/taller-tp0/punto2-diff-wordsc.png)
![](/taller-tp0/punto2-diff-wordsh.png)
![](/taller-tp0/punto2-error-gen.png)
![](/taller-tp0/punto2-error-estilo.png)

<h1> Paso 3 - SERCOM - Errores de generación 3: </h1>

![](/taller-tp0/punto3-diff.png)
![](/taller-tp0/punto3-error-gen.png)
![](/taller-tp0/punto3-error-estilo.png)

<h1> Paso 4 - SERCOM - Memory Leaks y Buffer Overflows: </h1>
![](/taller-tp0/punto4-diff.png)
![](/taller-tp0/punto4-res-sin-valgrind.png)
![](/taller-tp0/punto4-res-valgrind2.png)
![](/taller-tp0/punto4-res-valgrind1.png)
![](/taller-tp0/punto4-longname-valgrind.png)
![](/taller-tp0/punto4-tda-valgrind.png)

<h1> Paso 5 - SERCOM - Código de retorno y salida estándar: </h1>
![](/taller-tp0/punto5-diff.png)
![](/taller-tp0/punto5-res-valgrind.png)
![](/taller-tp0/punto5-hexdump.png)
![](/taller-tp0/punto5-make.png)
![](/taller-tp0/punto5-gdb-tp.png)
![](/taller-tp0/punto5-gdb-info-functions.png)
![](/taller-tp0/punto5-gdb-wordscounter-next.png)
![](/taller-tp0/punto5-gdb-break.png)

<h1> Paso 6 - SERCOM - Entrega exitosa: </h1>
![](/taller-tp0/punto6-diff-main.png)
![](/taller-tp0/punto6-diff-wordsc.png)
![](/taller-tp0/punto6-diff-wordsh.png)
![](/taller-tp0/punto6-res-valgrind.png)
![](/taller-tp0/punto6-listado-res.png)
![](/taller-tp0/punto6-single-word.png)
![](/taller-tp0/punto6-single-word-textfile.png)
![](/taller-tp0/punto6-res-valgrind1.png)
![](/taller-tp0/punto6-res-valgrind2.png)
![](/taller-tp0/punto6-res-valgrind3.png)

<h1> Paso 7 - SERCOM - Revisión de la entrega: </h1>






















