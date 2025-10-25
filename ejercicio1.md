## Ejercicio 1

Un estudiante de la carrera de Computación necesita sacar el promedio de sus notas de la Unidad 1 en la asignatura Teoria de la Programación
para ello debe basarse en la siguiente rubrica
ACD: 20%
APE: 25%
AA: 20%
EVALUACIÓN: 35% ¿Cual seria el promedio sobre 10?

📝 Pseudocódigo

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
