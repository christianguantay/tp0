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

a)

![](/taller-tp0/punto1-error-estilo.png)

Analizando los problemas de estilo podemos ver que:

## paso1_wordscounter.c

En la linea 27 se observa que falta un espacio entre el while y el parentesis.

En la linea 41 no coinciden los espacios dentro de los argumentos del if() (deberian haber 0 espacios).

En la linea 47 el else deberia aparecer en la misma linea donde se cierra la llave } del if anterior.

En la linea 48 falta un espacio entre el if() y el parentesis que contiene los argumentos.

En la linea 53 hay un espacio entre la instruccion y el punto y coma ;.

## main.c

En la linea 12 es mejor usar sprintf que strcpy

En la linea 15 el else deberia aparecer en la misma linea donde se cierra la llave } del if anterior.

## paso1_wordscounter.h

La linea 5 deberia tener menos de 80 caracteres de largo.

b)

![](/taller-tp0/punto1-error-gen.png)

En la linea 22 de main.c se declara un tipo de dato desconocido words_counter_t

En las lineas 23, 24, 25 y 27 de main.c se hace una declaracion implicita de funciones que no se definieron antes debido a que no se incluyo el .h

Todos estos errores reportados se tratan de errores del compilador.

c)

![](/taller-tp0/punto1-warning.png)

El sistema reporta un error ya que no se pudo compilar el programa.

<h1> Paso 2 - SERCOM - Errores de generación 2: </h1>

a)

![](/taller-tp0/punto2-diff-main.png)
![](/taller-tp0/punto2-diff-wordsc.png)
![](/taller-tp0/punto2-diff-wordsh.png)

En el archivo paso2_main.c se puede observar que se incluyo el header paso2_wordscounter.h y se reemplazo strcpy por memcpy. Ademas de esto
se corrigio el error de estilo respecto a los brackets } en el else.

En el archivo paso2_wordscounter.c se puede observar que se incluyo el header de paso2_wordscounter.h y se corrigieron los errores de estilo referentes
a los brackets } y a los espacios dentro de los, while, if y else detallados en el paso 1.

En el archivo paso2_wordscounter.h se cambio el comentario sobre para que se utiliza wordscounter_t.


b)

![](/taller-tp0/punto2-error-estilo.png)

Se puede observar que con las correcciones anteriores no se presentan errores de estilo.


c)

![](/taller-tp0/punto2-error-gen.png)

En las lineas 7 y 20 de paso2_wordscounter.h no se reconoce el tipo de dato size_t debido a que no se incluyo el header stdio.h.

En la linea 25 de paso2_wordscounter.h tampoco se reconoce el tipo de dato FILE debido a que no se incluyo el header stdio.h.

En la linea 17 de paso2_wordscounter.c hay un conflico en la declaracion de wordscounter_get_words debido a que no se reconoce el tipo de dato size_t.

En la linea 30 de paso2_wordscounter.c no se reconoce la funcion malloc() debido que a no se incluyo el header stdlib.h

Estos errores se tratan de errores del compilador.

<h1> Paso 3 - SERCOM - Errores de generación 3: </h1>

a)

![](/taller-tp0/punto3-diff.png)

En este paso se puede ver que se agregaron las librerias faltantes stdlib.h, string.h y stdio.h para que funcione el programa.

b)

![](/taller-tp0/punto3-error-gen.png)

En este paso el error se debe a que hay una referencia no definida a wordscounter_destroy realizada en el momente de linkear el programa.

<h1> Paso 4 - SERCOM - Memory Leaks y Buffer Overflows: </h1>

a)

![](/taller-tp0/punto4-diff.png)

En este paso se puede ver que se definio la funcion wordscounter_destroy para que se pueda compilar el programa.

![](/taller-tp0/punto4-res-sin-valgrind.png)


![](/taller-tp0/punto4-res-valgrind1.png)
![](/taller-tp0/punto4-res-valgrind2.png)



b)

![](/taller-tp0/punto4-longname-valgrind.png)

c)

![](/taller-tp0/punto4-tda-valgrind.png)

d)

e)

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






















