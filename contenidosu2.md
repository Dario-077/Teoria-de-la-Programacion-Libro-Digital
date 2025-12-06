[Regresar a la pagina anterior](unidad2.md)  

# 📘Estructuras condicionales  
## 🔠If (Condicional simple)
### 📝Definición:
  La estructura condicional If nos indica una condición, esta sera evaluada como un dato booleano, si este resulta verdadero el bloque de código se jecutara, caso contrario el programa pasa a la siguiente linea
### 🧩Estructura:
<img width="507" height="248" alt="image" src="https://github.com/user-attachments/assets/bc019528-3b5b-4692-8310-210e5bf0513f" />

 ### 🟩💻Ejemplo práctico  
 #### 📎Contextualizacion: 
Dados tres numeros decimales mostrar el promedio y si este es mayor o igual a 12
mostrar el mensaje "Nota aprobatoria"  
### 👨‍💻Código en C  
#include <stdio.h>
int main(){

    //Datos de entrada

    float numero1, numero2, numero3, promedio;

    printf("Ingrese la nota del numero 1: \n");
    scanf("%f", &numero1);

    printf("Ingrese la nota del numero 2: \n");
    scanf("%f", &numero2);

    printf("Ingrese la nota del numero 3: \n");
    scanf("%f", &numero3);

    //Proceso
 
    promedio = ((numero1 + numero2 + numero3)/3);

    if(promedio >= 12){
        printf("Su promedio %f es aprobatorio", promedio);

    }
    return 0;
}  

#### 🟦➡️🟧➡️🟩Diagrama de flujo
<img width="382" height="447" alt="image" src="https://github.com/user-attachments/assets/7bdf9cf2-6410-4120-943f-9f7b6efe0760" />

## 🔠If- else  (Condicional doble)  
### 📝Definicion  
Es un complemento de la estructura "If", mantiene la lógica de ejecución mediante el resultado de una condición, sin embargo, aqui se agrega la palabra reservada *else* que contiene la instrucción que se ejecutara en caso de que la condición inciial resulte falsa  
### 🧩Estructura  
<img width="496" height="257" alt="image" src="https://github.com/user-attachments/assets/9e228336-b186-4bbb-bab8-a073240f539e" />

###  🟩💻Ejemplo  
#### 📎Contextualizacion:
Dado como dato el sueldo del trabajador (en S), considere un aumento del 45% si su sueldo es 
inferior a 1000, de lo contrario realiza un descuento del 10%. Mostrar el sueldo con aumento o descuento  
####  👨‍💻Código en C  
#include <stdio.h>

int main(){}

    float sueldo, sueldo1, sueldo2;

    printf("Ingrese el sueldo en Dolares estadounidenses: \n");
    scanf("%f", &sueldo);

    if(sueldo < 1000){
        sueldo1 = ((sueldo * 0.45) + sueldo);
        printf("El sueldo sera: %.2f  : \n", sueldo1);
    } else{
        sueldo2 = (sueldo - (sueldo * 0.1));
        printf("El sueldo sera: %.2f  : \n", sueldo2);
    }
    return 0;
    }
#### 🟦➡️🟧➡️🟩Diagrama de flujo  
<img width="544" height="375" alt="image" src="https://github.com/user-attachments/assets/05f9fe15-1671-48b2-b721-be7a49647819" />


## 🔠Switch (Condicional cascada)  
### 📝Definición  
Condicional usado en caso de un algoritmo de seleccion multiple, es obligatorio asignarle un valor al que se regira el Switch, puede ser una variable, además, se le ingresara la lista de los posibles casos de respuestas y el bloque de código perteneciente a cada una de las mismas.  
OJO: Es importante agregar la palabra reservada "default" en caso de que no se asigne ningun valor esperado y agregar su respectivas instrucciones. En adicion se agrega la palabra "break", para indicar el fin de un caso
### 🧩Estructura  

  <img width="420" height="306" alt="image" src="https://github.com/user-attachments/assets/e5a1a0a7-0316-42ae-b5cf-87030cfe84c6" />

  
### 🟩💻Ejercicio  
#### 📎Contextualizacion:
Algoritmo que imprima el nombre de los días de la semana  
#### 👨‍💻Código en C  
#include <stdio.h>

//getchar: Libera espacio en la memoria (buenas practicas)


int main(void){

    int dia;

    printf("Ingrese el dia de la semana en numero, del 1 al 7: \n");
    scanf("%i", &dia);
    getchar();

    switch(dia){
        case 1: 
            printf("El dia es Lunes \n");
            break;
        
        case 2:
            printf("El dia es Martes \n");
            break;

        case 3:
            printf("El dia es Miercoles \n");
            break;

        case 4:
            printf("El dia es Juebebes \n");
            break;

        case 5:
            printf("El dia es Viernesote \n");
            break; 

        case 6:
            printf("el dia es Sabado \n");
            break;

        case 7:
            printf("el dia es Domingo \n");
            break;

        default:
            printf("Numero no valido");
            break;

    return 0;
#### 🟦➡️🟧➡️🟩Diagrama de flujo  
<img width="678" height="328" alt="image" src="https://github.com/user-attachments/assets/a78f953c-32d7-43af-8ef4-ca5b9647d0ce" />


# 📘Estructuras repetitivas o Bucles  
## 🚀While  
### 📝Definicion  
La estructura While funciona en base de una condicion especifica, el programa primero evaluara si la condicion en cuestion es verdadera para comenzar a ejecutar las instrucciones, esto es importante de tomar en cuenta. El código se ejecutara siempre que la condición sea True y una vez esto cambie saldra del bucle  
**Tip**:   
- Agregar un contador para que este sea la condición a cumplir
- Plantear bien la sintaxis para que no se ejcute un bucle infinito
### 🧩Estructura 
<img width="255" height="156" alt="image" src="https://github.com/user-attachments/assets/3c8bc75a-9bc5-4330-b825-088b81114493" />  

### 🟩💻Ejercicio  
#### 📎Contextualizacion
Algoritmo que permita visualizar la tabla del 6
#### 👨‍💻Código en C:  
int numero, producto, MULTIPLICADOR;
    
    numero = 0;
    MULTIPLICADOR = 6;
    
    printf("La tabla del 6 es: \n ");

    while(numero <= 11){
        numero += 1;
        producto = numero * MULTIPLICADOR;
        printf(" %i * %i = %i \n", numero, MULTIPLICADOR, producto);
        
    }
    return 0;
    }
#### 🟦➡️🟧➡️🟩Diagrama de flujo:   
<img width="442" height="467" alt="image" src="https://github.com/user-attachments/assets/879af00f-017f-42b0-9056-3903c2fa81d6" />


## 🚀Do- While  
### 📝Definicion  
Un bucle que ejecuta un bloque de código hasta que la condicion evaluada sea False. Es similar al While, sin embargo en este se toma en cuenta en que si o si se ejecutara al menos una vez las instrucciones, despues de esa primera ejecucion, se verificara si la condicion es correcta.  
**TIP**:
- Se recomienda usar un contador para que que este se encargue de actuar a forma de condición
### 🧩Estructura  
<img width="457" height="231" alt="image" src="https://github.com/user-attachments/assets/3dcb0dfc-c8e5-42f3-b6c8-c884107bbc1e" />   

### 🟩💻Ejercicio  
#### 📎Contextualizacion
Realizar la division de dos numeros enteros, validar el denominador diferente de 0
#### 👨‍💻Código en C
int main(){
float divisor, cociente, dividendo;

    printf("Ingrese el dividendo: \n");
    scanf("%f", dividendo);

    do{
         printf("Ingrese el divisor: \n");
         scanf("%f", divisor);
    } while (divisor == 0);
    
    printf("Ingrese el divisor:\n ");
    scanf("%f", divisor);
    cociente = (dividendo / divisor) ;

    printf("El cociente es: %f \n", cociente);

    return 0;
    
}
#### 🟦➡️🟧➡️🟩Diagrama de flujo  
<img width="319" height="438" alt="image" src="https://github.com/user-attachments/assets/7563cdcb-92a3-466f-a975-9fe28d72d72c" />

## 🚀For 
### 📝Definición 
El bucle For, se usa especificamente cuando ya se saben las repeticiones precisas que requiere el algoritmo, a diferencia de la estructura anterior, aqui se colocan 3 datos importantes al inicio.  
**Tip**
- Se debe escoger muy bien la variable que cumplira la condicion, aumento e inializacion, se recomieda usar el contador
### 🧩Estructura  
<img width="619" height="190" alt="image" src="https://github.com/user-attachments/assets/4dcb721c-f7a6-429e-b345-82ff47f2ff22" />  

### 🟩💻Ejercicio  
#### 📎Contextualizacion
Obtener el factorial de "n" ingresado por el usuario  
#### 👨‍💻Código en C  

int main(){
 long long n, contad;
    long long resul = 1;

    printf("Ingrese un numero: \n");
    scanf("%lld", &n);

    for(contad = 1 ; contad <= n; contad ++){
        resul = resul * contad; 
    }
    printf("El factorial es: %llu \n", resul);
    return 0;
}

#### 🟦➡️🟧➡️🟩Diagrama de flujo  

<img width="330" height="468" alt="image" src="https://github.com/user-attachments/assets/893abca1-337a-414f-ae91-b811195d5446" />

