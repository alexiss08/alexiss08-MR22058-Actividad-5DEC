# **MR22058-Actividad-5DEC**
### **Actividad # 5 evaluada diseño y estructura de ccomputadoras** 

El proposito de esta actividad es que podamos familiarizarnos con el lenguaje ensamblador 
mas especificamente el lenguaje NASM en el cual cada uno de los archivos de texto subidos
a continuacion cada uno tiene un proposito en especifico en lenguaje ensamblador x86

#### **Ejercicio 1 resta de 3 enteros con 16 bits**
Este ejercicio realiza la resta de tres números enteros con formato de 16 bits (dw o double word).
Las variables están definidas en la sección .data.

- num1, num2, y num3 son las variables con los valores iniciales a restar.
- mensaje contiene el mensaje a mostrar antes de imprimir el resultado.
- len_mensaje es la longitud del mensaje.
- linea es un salto de línea para separar el mensaje del resultado.
En la sección .text, se realiza la resta de los números y se convierte el resultado a ASCII 
para mostrarlo correctamente. Finalmente, se imprime el mensaje y el resultado, seguido de un salto de línea.
