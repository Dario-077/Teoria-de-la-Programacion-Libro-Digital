[volver a la pagina anterior](unidad3.md)
# Modularidad  
Indispensable al tener algoritmos largos y complejos  
Consiste en dividir el programa grande (padre) en subprogramas pequeños (hijos)[12]
Con eso logramos que:  
1. Reducir la complejidad
2. Atender la solucion por separado
3. "Divide y venceras"
## Pase de parametros por referencia  
Método para pasar argumentos a funciones compartiendo la dirección de memoria de
la variable original, NO UNA COPIA. 
Esto permite que:
1. Cualquier modificación hecha dentro de la función afecte directamente al valor original
2. Es la ideal para modificar objetos compuestos o grandes estructuras de datos sin gastar memoria adicional en copiarlos. 
### Ejercicio

## Pase de parametros por valor
Se envía una copia del dato original a una función. La función trabaja con esta copia local en un espacio de memoria independiente, por lo que
cualquier modificación realizada dentro no afecta a la variable original. 
Muy útil para mantener la integridad de los datos
