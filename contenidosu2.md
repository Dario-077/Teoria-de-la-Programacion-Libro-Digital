[Regresar a la pagina anterior](unidad2.md)  

# Estructuras condicionales  
## If (Condicional simple)
### Definición:
  La estructura condicional If nos indica una condición, esta sera evaluada como un dato booleano, si este resulta verdadero el bloque de código se jecutara, caso contrario el programa pasa a la siguiente linea
### Estructura:
- If (condición){
         bloque se código
        }
  OJO: Puede haber más de una instrucción
 ### Ejemplo   

## If- esle  (Condicional doble)  
### Definicion  
Es un complemento de la estructura "If", mantiene la lógica de ejecución mediante el resultado de una condición, sin embargo, aqui se agrega la palabra reservada *else* que contiene la instrucción que se ejecutara en caso de que la condición inciial resulte falsa  
### Estructura  
If (Condición){
  bloque de código
  } else {
    bloque de código secundario
    }   
###  Ejemplo    

## Switch (Condicional casacada)  
### Definición  
Condicional usado en caso de un algoritmo de seleccion multiple, es obligatorio asignarle un valor al que se regira el Switch, puede ser una variable, además, se le ingresara la lista de los posibles casos de respuestas y el bloque de código perteneciente a cada una de las mismas.  
OJO: Es importante agregar la palabra reservada "default" en caso de que no se asigne ningun valor esperado y agregar su respectivas instrucciones. En adicion se agrega la palabra "break", para indicar el fin de un caso
### Estructura  
switch(variable){
  case 'A': instruccion
    break;
  case 'B': Instruccion
    break;
  default: Instruccion
}  
### Ejercicio  

# Estructuras repetitivas o Bucles  
## While  
### Definicion  
La estructura While funciona en base de una condicion especifica, el programa primero evaluara si la condicion en cuestion es verdadera para comenzar a ejecutar las instrucciones, esto es importante de tomar en cuenta. El código se ejecutara siempre que la condición sea True y una vez esto cambie saldra del bucle  
**Tip**:   
- Agregar un contador para que este sea la condición a cumplir
- Plantear bien la sintaxis para que no se ejcute un bucle infinito

    


      
