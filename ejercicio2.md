# Ejercicio 2  
Determinar si un numero es positivo o negativo

## Pseudocodigo

Algoritmo Libro_Digital_ejercicio2
	
	//Determinar si un numero es positivo o negativo
	
	// Variables
	
	definir digito Como Real
	
	// Entrada
	
	Escribir "Ingrese un digito diferente de 0"
	Leer digito
	
	// Salida
	Si digito > 0 Entonces
		Escribir "El numero es positivo"
	FinSi
	
	Si digito < 0 Entonces
		Escribir "El numero es negativo"
	FinSi
	
FinAlgoritmo

## Diagrama de flujo
<img width="842" height="813" alt="ejercicio2diagrama" src="https://github.com/user-attachments/assets/082be87f-7e60-46ac-af15-14b77f525e4a" />

## Codigo en C

#include <stdio.h>
#include <math.h>

int main(){

    // Determinar si un numero es positivo o negativo

    // Variable
    float digito;

    // Entrada

    printf("Coloque el digito deseado, que sea diferente de 0: ");
    scanf("%f", &digito);

    // Proceso y salida

    if (digito > 0){
        printf ("El digito ingresado es positivo");
    }

    if (digito < 0){
        printf ("El digito ingresado es negativo");
    }

    return 0;
}

[Pagina anterior](ejercicios.md)

