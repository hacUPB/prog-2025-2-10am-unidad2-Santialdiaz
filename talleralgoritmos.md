# **Introducción**

En el ámbito de la ingeniería, la resolución de problemas requiere no solo un análisis preciso de la situación, sino también la capacidad de transformar ese análisis en una solución práctica y eficiente. En este taller, los estudiantes deberán demostrar sus competencias para:

- Analizar problemas relacionados con la ingeniería.
- Diseñar un algoritmo que solucione el problema planteado.
- Representar la solución utilizando pseudocódigo y diagramas de flujo.

Cada problema deberá resolverse empleando estructuras de control como condicionales y bucles, asegurando la correcta interpretación de requisitos y el diseño lógico del flujo de ejecución.

## **1. Ejercicios con condicionales**

1. **Verificación de peso de despegue**
    
    En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.

# Pseudocódigo:
```
Inicio
    Leer peso_vacio
    Leer peso_combustible
    Leer peso_carga
    Leer peso_max_despegue

    peso_total = peso_vacio + peso_combustible + peso_carga

    Si peso_total <= peso_max_despegue Entonces
        Escribir "Aeronave lista para despegar"
    SiNo
        Escribir "Reducir carga o combustible"
    FinSi
Fin
```

### **2. Ejercicios con bucles**

1. **Registro de altitudes de vuelo**
    
    Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.

```
INICIO
NICIO
i=0
  Mientras i<6
     Leer altitud
     Mediciones[i]=altitud
     i=i+1
  Fin Mientras
i=0
  Mientras i<6
    Mostrar altitud
     i=i+1
  Fin Mientras

Fin
```
### **2. Ejercicios con bucle y condicionales**
6. **Control de temperatura en cabina**

Un sistema mide cada 5 minutos la temperatura en cabina durante una hora. Si en algún momento se detecta una temperatura mayor a 27°C o menor a 18°C, debe indicar que se active el sistema de climatización
```
Inicio
    contador = 1

    Mientras contador <= 12 Hacer
        Leer temp
        Si temp > 27 O temp < 18 Entonces
            Escribir "Activar climatización"
            Salir
        FinSi
        contador = contador + 1
    FinMientras
Fin
```