🔗[volver a la pagina anterior](unidad3.md)
# 🧩Modularidad  
Indispensable al tener algoritmos largos y complejos  
Consiste en dividir el programa grande (padre) en subprogramas pequeños (hijos)[12]  

⚙️Con eso logramos que:  
1. Reducir la complejidad
2. Atender la solucion por separado
3. "Divide y venceras"
## 📤📥Pase de parametros por referencia  
Método para pasar argumentos a funciones compartiendo la dirección de memoria de
la variable original, NO UNA COPIA.  

Esto permite que:
1. Cualquier modificación hecha dentro de la función afecte directamente al valor original
2. Es la ideal para modificar objetos compuestos o grandes estructuras de datos sin gastar memoria adicional en copiarlos. 
### 💻Ejercicio  


<img width="650" height="490" alt="image" src="https://github.com/user-attachments/assets/4ec3b95d-38f5-42c2-9c65-38d3cf8b258a" />

## 🧷Pase de parametros por valor
Se envía una copia del dato original a una función. La función trabaja con esta copia local en un espacio de memoria independiente, por lo que
cualquier modificación realizada dentro no afecta a la variable original.  

Muy útil para mantener la integridad de los datos
### 💻Ejercicio  

<img width="720" height="537" alt="image" src="https://github.com/user-attachments/assets/aa292328-68ac-45b2-83ff-ab252b69f0a6" />

# 📊Estructura de datos estaticos  
Es un tipo de dato más elaborado, es decir, esta construido a partir de otros
tipos de datos.
Puede ser:  

Homogeneo: Si todos los elementos que la forman son del mismo tipo  

Heterogeneo: Si sus elementos son de más de un tipo  

Se considera estatica, porque ya posee un tamaño fijo desde antes de la ejecución, el cual no puede ser modificado[13]  

## ➡️Arrays (unimensionales)  
El tipo de arreglo más sencillo, es similar a una lista   
### 💻Ejercicio 

<img width="754" height="424" alt="image" src="https://github.com/user-attachments/assets/2f8770e7-4d6a-40cd-9383-1247be2a5835" />


## 🟦🟦Bidimensionales  
Tmabien denominado matriz, porque presenta más complejidad con valores dispuestos en filas y columnas  
### 💻Ejercicio
<img width="750" height="422" alt="image" src="https://github.com/user-attachments/assets/51d1a7b2-00cd-4c45-b3d7-7107ccb1a81f" />  

<img width="532" height="357" alt="image" src="https://github.com/user-attachments/assets/e2982750-1f73-426a-9744-ef4891c116ad" />



## 🧊Tridimensionales  
Los cubos son el ejemplo de mayor complejidad en cuanto a arreglos estaticos, 
presentan valores que se encuentran a lo largo, ancho y profundo (o tambien de minado capa) de un plano  
### 💻Ejercicio
<img width="786" height="442" alt="image" src="https://github.com/user-attachments/assets/a06714d6-54f8-4a40-a736-c1c4191be969" />




