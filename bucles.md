# Bucles o Ciclos

Un bucle en programación es una estructura de control que permite ejecutar repetidamente un bloque de código mientras se cumple una condición específica o durante un número determinado de iteraciones. Son fundamentales para automatizar tareas repetitivas, realizar cálculos iterativos y procesar grandes conjuntos de datos. En el lenguaje C, existen tres tipos principales de bucles: **for**, **while**, y **do-while**. El bucle **for** se utiliza cuando se conoce de antemano la cantidad de iteraciones, especificando un inicio, una condición y un incremento o decremento. El bucle **while** ejecuta el bloque de código mientras la condición sea verdadera, siendo útil cuando no se conoce el número exacto de iteraciones. Finalmente, el bucle **do-while** es similar al **while**, pero garantiza que el bloque de código se ejecute al menos una vez, ya que evalúa la condición al final de cada iteración. Estas estructuras son herramientas esenciales para la resolución eficiente de problemas en C.

# Ejercicios de Bucles en Clase:
## Ejercicio 1.
 Se requiere un algoritmo para determinar, de N cantidades, cuantas son cero, cuantas son menores a cero y cuantas son mayores a cero. Realice el diagrama de flujo y el pseudocodigo, representarlo, utilizando el ciclo apropiado

|Input | Cantidad|Control|
|---------|-----|---------|
|N, cant| ceros, mayores, menores (contador)| N|

```
Inicio
Leer N
ceros = 0
mayores = 0
menores = 0
Mientras N > 0:
    Leer cant
    Si cant > 0:
        mayores = mayores+1
    Si no
        Si cant = 0:
        ceros = ceros + 1
    Si no
        menores = menores + 1
    Fin si
Fin si
N = N - 1
Fin Mientras
Mostrar ceros, mayores, menores
Fin
```
![ImagenEjer1](./Images/Buclesej1.png)

## Ejercicio 2.
 Calcular el Factorial de un numero entero ingresado por el usuario.
 ![ImagenEjer1](./Images/Buclesej3.png)

# TAREA:
