## Ejercicio 1: Encontrar numero menor

```plaintext
Inicio
    Escribir "Ingrese el primer número:"
    Leer num1
    Escribir "Ingrese el segundo número:"
    Leer num2
    Escribir "Ingrese el tercer número:"
    Leer num3

    Si num1 < num2 y num1 < num3 Entonces
        Escribir "El menor número es:", num1
    Sino Si num2 < num1 y num2 < num3 Entonces
        Escribir "El menor número es:", num2
    Sino
        Escribir "El menor número es:", num3
    FinSi
Fin
```


## Ejercicio 2: Determinar si un Año es Bisiesto

```plaintext
Inicio
    Escribir "Ingrese el año:"
    Leer año

    Si (año mod 4 = 0 y año mod 100 != 0) o (año mod 400 = 0) Entonces
        Escribir "El año", año, "es bisiesto."
    Sino
        Escribir "El año", año, "no es bisiesto."
    FinSi
Fin

```


## Ejercicio 3: Clasificación por Edades
Este programa debe clasificar a una persona según su edad en diferentes categorías y, adicionalmente, verificar si es su cumpleaños para dar un mensaje especial. Las categorías son: infante (0-5 años), niño (6-12 años), adolescente (13-17 años), adulto (18-64 años), y senior (65 años o más).


```plaintext
Inicio
    Escribir "Ingrese su edad:"
    Leer edad
    Escribir "¿Es hoy su cumpleaños? (sí/no):"
    Leer cumpleaños

    Si edad < 0 o edad > 120 Entonces
        Escribir "Edad no válida."
    Sino
        Si edad >= 0 y edad <= 5 Entonces
            categoria = "Infante"
        Sino Si edad >= 6 y edad <= 12 Entonces
            categoria = "Niño"
        Sino Si edad >= 13 y edad <= 17 Entonces
            categoria = "Adolescente"
        Sino Si edad >= 18 y edad <= 64 Entonces
            categoria = "Adulto"
        Sino
            categoria = "Senior"
        FinSi

        Escribir "Usted está clasificado como:", categoria

        Si cumpleaños = "sí" Entonces
            Escribir "¡Feliz cumpleaños! Que tenga un día maravilloso."
        FinSi
    FinSi
Fin

```
