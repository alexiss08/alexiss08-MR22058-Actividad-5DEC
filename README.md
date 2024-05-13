# **MR22058-Actividad-5DEC**

### **Actividad #5 evaluada diseño y estructura de computadoras**

El propósito de esta actividad es familiarizarse con el lenguaje ensamblador, específicamente NASM, utilizando el conjunto de instrucciones x86.

---

#### **Ejercicio 1: Resta de 3 enteros con 16 bits**

**Objetivo:** Realizar la resta de tres números enteros de 16 bits en lenguaje ensamblador x86 utilizando NASM.

**Variables utilizadas:**
- `num1`, `num2` y `num3`: Son variables definidas en la sección .data que representan los tres números a restar. Todas están definidas como words (dw).
- `mensaje`: Es una variable definida en la sección .data que contiene el mensaje "El resultado de la resta es: " que se mostrará antes de imprimir el resultado.
- `len_mensaje`: Es una variable definida en la sección .data que contiene la longitud del mensaje.
- `linea`: Es una variable definida en la sección .data que contiene el carácter de salto de línea (0xA) para separar el mensaje del resultado.

**Proceso:**
1. Se mueven los valores de `num1`, `num2` y `num3` a los registros ax, bx y cx respectivamente.
2. Se restan los valores de `num2` y `num3` a ax.
3. Se convierte el resultado a ASCII y se almacena en la memoria en la variable `resultado`.
4. Se imprime el mensaje "El resultado de la resta es: ".
5. Se imprime el resultado de la resta.
6. Se imprime un salto de línea para separar el mensaje del resultado.

---

#### **Ejercicio 2: Multiplicación de dos números de un byte**

**Objetivo:** Realizar la multiplicación de dos números de un byte en lenguaje ensamblador x86 utilizando NASM.

**Variables utilizadas:**
- `num1` y `num2`: Son variables definidas en la sección .data que representan los dos números a multiplicar. Ambas están definidas como bytes (db).
- `mensaje`: Es una variable definida en la sección .data que contiene el mensaje "El resultado es: " que se mostrará antes de imprimir el resultado.
- `linea`: Es una variable definida en la sección .data que contiene el carácter de salto de línea (0xA) para separar el mensaje del resultado.

**Proceso:**
1. Se mueven los valores de `num1` y `num2` a los registros al y bl respectivamente.
2. Se realiza la multiplicación de al por bl y se almacena el resultado en ax.
3. Se convierte el resultado a ASCII y se almacena en la memoria en la variable `resultado`.
4. Se imprime el mensaje "El resultado es: ".
5. Se imprime el resultado de la multiplicación.
6. Se imprime un salto de línea para separar el mensaje del resultado.
