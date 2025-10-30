## Ejercicio 1   
[Pagina anterior](ejercicios.md)  

🔥Un estudiante de la carrera de Computación necesita sacar el promedio de sus notas de la Unidad 1 en la asignatura Teoria de la Programación
para ello debe basarse en la siguiente rubrica
ACD: 20%
APE: 25%
AA: 20%
EVALUACIÓN: 35% ¿Cual seria el promedio sobre 10?

## 📝 Pseudocódigo: 
Se representara este algoritmo por medio de Pseudocódigo usando los conocimientos adquiridos en clase  
Herramienta usada: Pseint

	// ACD: 20 MOD
	// APE: 25 MOD
	// AA: 20 MOD
	// EVALUACIÓN: 35 MOD   
	¿Cual seria el promedio sobre 10?  
	
	// Variables y Constantes
	Definir ACD, APE, AA, EVALUACION, promedio, ponderadoAcd, ponderadoApe, ponderadoAa, ponderadoEvaluacion, notaAcd, notaApe, notaAa, notaEvaluacion Como Real  
	
	ACD <- 0.2
	APE <- 0.25
	AA <- 0.2
	EVALUACION <- 0.35  
	
	// Entrada
	Escribir 'Escriba la nota del ACD'
	Leer notaAcd
	ponderadoAcd <- notaAcd*ACD  
	
	Escribir 'Escriba la nota del APE'
	Leer notaApe
	ponderadoApe <- notaApe*APE  
	
	Escribir 'Escriba la nota del AA'
	Leer notaAa
	ponderadoAa <- notaAa*AA  
	
	Escribir 'Escriba la nota de la evaluacion'
	Leer notaEvaluacion
	ponderadoEvaluacion <- notaEvaluacion*EVALUACION  
	
	// Salida
	promedio <- ponderadoAcd+ponderadoApe+ponderadoAa+ponderadoEvaluacion
	Escribir 'El promedio de la Unidad 1 es: ', promedio  
	
	

FinAlgoritmo  


## 📊 Diagrama de flujo:  
Usando la herramienta Pseint se representa el pseudocódigo a manera de diagrama de flujo, dandonos un contenido mucho más visual y estético  

**Imagen 2** 
<img width="3260" height="1535" alt="ejercicio1diagrama" src="https://github.com/user-attachments/assets/3a5e3abf-064a-4879-8b9a-dd4791369e93" />

## 💻 Código en C:  
El algoritmo presentado a inicios de esta página sera trasladado a un lenguaje de programación C, adaptandolo a la sintaxis y lógica del mismo


#include <stdio.h>  

#include <math.h>

int main(){

	// ACD: 20 MOD
	// APE: 25 MOD
	// AA: 20 MOD
	// EVALUACIÓN: 35 MOD    ¿Cual seria el promedio sobre 10?

	// Variables y Constantes

    float promedio, ponderadoAcd, ponderadoApe;
    float ponderadoAa, ponderadoEvaluacion, notaAcd, notaApe, notaAa, notaEvaluacion;

    // Entrada

    printf("Ingrese la nota del ACD: \n");
    scanf("%f", &notaAcd);

    printf("Ingrese la nota del APE: \n");
    scanf("%f", &notaApe);

    printf("Ingrese la nota del AA: \n");
    scanf("%f", &notaAa);

    printf("Ingrese la nota de la evaluacion: \n");
    scanf("%f", &notaEvaluacion);

    // Proceso

    ponderadoAcd = notaAcd * 0.2;
    ponderadoApe = notaApe * 0.25;
    ponderadoAa = notaAa * 0.2;
    ponderadoEvaluacion = notaEvaluacion * 0.35;

    // Salida

    promedio = ponderadoAcd + ponderadoApe + ponderadoAa + ponderadoEvaluacion;

    printf("Su nota es: %f", promedio);

    return 0;

}
