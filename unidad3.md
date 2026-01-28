[Ir a la pagina anterior](index.md)  
# 👌Contenidos de la unidad  
[Click aqui](contenidosu3.md)  

# 🏫Principales dificultades  
Durante el desarrollo de la Unidad 3, la principal dificultad estuvo relacionada con la comprensión y aplicación del pase de parámetros por valor y por referencia. Aunque se logró entender la definición teórica de cada uno, resultó complicado llevar estos conceptos a la práctica dentro de un programa, especialmente al momento de decidir cuál utilizar en cada situación.

Asimismo, se presentó confusión en el uso de los operadores & y * en el pase por referencia, ya que no siempre fue claro dónde debían colocarse ni cómo acceder correctamente a los valores en memoria. Esta dificultad evidenció la necesidad de reforzar la práctica mediante ejercicios que permitan afianzar el uso correcto del pase de parámetros en la programación.

# 🎓Reflexion critica   
En la unidad 3 se nos mostro un mundo mucho más extenso de la programación, explicandose con detalle que existe más de un estilo o metodologia para programar, haciendo hincapie en la modularidad, demostrando como un problema complejo puede ser facilmente resuleto si lo dividimos por aprtes y resolvemos una por una.  

Esto ademas de usarlo como buenas pr+acticas ayudara en mi vida profesional para resolver problemas complejos. 

En adición, se nos hablo de un nuevo tipo de dato, "la estructura de datos estaticos", conociendo el método para agregar listas, matrices y cubos, algo que sera muy util para expandir mis conocimientos


# 🧱Tareas Entregadas   
## 🧾Proyecto academico integrador  

🔗[Black Mesa Bank Poster.pdf](https://github.com/user-attachments/files/24898899/Black.Mesa.Bank.Poster.pdf)  

Desarrollo grupal de un sistema bancario que simula el funcionamiento básico de un banco. Permite la creación de cuentas con nombre de usuario y PIN de 4 dígitos e iniciar de sesión con cuentas registradas.

Funcionalidades principales:

💰 Depósitos

💸 Retiros

📊 Consulta del estado de cuenta

📋 Visualización de cuentas existentes

**Aplicación de la modularidad:**

El sistema fue dividido en módulos para una mejor organización del código.

**Módulo pre-login:**

1. Menú principal.

2. Crear cuenta.

3. Salir del sistema.

**Módulo post-login:**

1. Depósitos.

2. Retiros.

3. Consulta de estado de cuenta.

Esta división permitió aplicar de forma práctica el concepto de modularidad, facilitando la comprensión y mantenimiento del programa.    

## 🧾APE 1  Construcción de funciones y procedimientos en un lenguaje de programación.

🔗 [Chillogallo_ape1_U3.pdf](https://github.com/user-attachments/files/24898930/Chillogallo_ape1_U3.pdf)  

Diseño de un algoritmo que calcula el promedio final de una asignatura. El cálculo se basa en el promedio de tres unidades académicas y cada unidad está compuesta por los siguientes componentes de aprendizaje:

📘 Aprendizaje autónomo

🧑‍🏫 Aprendizaje en contacto con el docente

🧪 Aprendizaje práctico experimental

📝 Evaluación sumativa

**Estructura del programa (modularidad):**

El programa fue dividido en funciones independientes, una para cada componente de aprendizaje de cada unidad.

Cada función:

1. Solicita las actividades realizadas durante el ciclo académico.

2. Aplica controles mediante condicionales.

3. Permite ingresar el número de tareas o actividades.

4. Calcula el promedio correspondiente al componente.

5. Cálculo final y programa principal:

Una función adicional se encarga de calcular el promedio final, tomando el promedio de cada unidad y aplicando un promedio general.

El main 🧩 actúa como el programa principal, desde donde se invocan todas las funciones desarrolladas, integrando el funcionamiento completo del sistema.

## 🧾Fundamentos de Python 1  
🔗 [Python_Essentials_1_certificate_dario-chillogallo-unl-edu-ec_534c76ed-b1cd-46e2-b665-235e4fb23651.pdf](https://github.com/user-attachments/files/24898965/Python_Essentials_1_certificate_dario-chillogallo-unl-edu-ec_534c76ed-b1cd-46e2-b665-235e4fb23651.pdf)  

Curso en línea Fundamentos de Python 1, desarrollado en la plataforma Cisco, como evidencia de cumplimiento, se entregó el certificado de aprobación emitido por la plataforma.

El curso estuvo orientado a introducir los conceptos básicos del lenguaje Python.

**Contenidos abordados:**

📜 Breve historia y contexto del lenguaje Python.

🖨️ Instrucciones básicas de entrada y salida (print, input).

🧠 Lógica básica de programación.

🔁 Bucles repetitivos.

🔀 Estructuras condicionales.

📋 Manejo de listas (agregar, eliminar y modificar elementos).

🧮 Introducción a matrices.

**Metodología del curso:**

El curso estuvo organizado en unidades progresivas.

Cada unidad incluía:

Ejercicios prácticos.

📝 Evaluaciones obligatorias.

Para avanzar al siguiente módulo era necesario obtener una calificación mínima, lo que garantizó la correcta comprensión de los contenidos antes de continuar.

## APE 2: Implementacion de funciones utlizando el paso de parametros por valor y referencia  

    #include <stdio.h>

    void calcularValorCliente(float *total){
    float playStation = 2.50, xbox = 2.00, nintendo = 1.50;
    float consola, valorApagar=0;
    int horas;
    do {
        printf("Ingresa la consola que utilizaste (1 = PlayStation, 2 = Xbox, 3 = Nintendo): ");
        scanf("%f", &consola);

        if (consola < 1 || consola > 3) {
            printf("Ingresa un valor valido\n");
        }
    } while (consola < 1 || consola > 3);

    if (consola == 1) {
        consola = playStation;
    } else if (consola == 2) {
        consola = xbox;
    } else if (consola == 3) {
        consola = nintendo;
    }

    printf("Ingresa la cantidad de horas que jugaste: ");
    scanf("%d", &horas);

    valorApagar = consola * horas;
    printf("El valor a pagar es: %.2f\n", valorApagar);
    *total += valorApagar;
    }

    void calcularValorRecaudado(int cantidadClientes){
    float total=0;
    for (int i = 0; i < cantidadClientes; i++){
        calcularValorCliente(&total);
    }
    printf("\nEl valor final recaudado por todas las atenciones es: %.2f\n", total);
    }


    int main() {
    int cantidadClientes;

    printf("Cantidad de clientes a atender: ");
    scanf("%d", &cantidadClientes);

    calcularValorRecaudado(cantidadClientes);

    return 0;
    }

En esta actividad realizamos un programa en lenguaje C permite calcular el valor a pagar por el uso de consolas de videojuegos (PlayStation, Xbox o Nintendo) según la cantidad de horas jugadas por cada cliente, y finalmente calcula el total recaudado por la atención de varios clientes.  

Usamos la modularidad para optimizar la solucion  

**Funciones:**  
**1. calcularValorCliente:**
Calcula el valor a pagar de un cliente individual según:

-El tipo de consola utilizada

-El número de horas jugadas

-Además, acumula el valor en el total general mediante un puntero.  

**2. alcularValorRecaudado**
**Proposito:**

Calcula el valor total recaudado tras atender a varios clientes.

**3. int main**

Indica la cantidad de clientes e invoca a las funciones




