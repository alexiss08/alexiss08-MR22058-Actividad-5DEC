# **MR22058-Actividad-5 DEC**

### **Actividad #5 evaluada diseño y estructura de computadoras**

En esta actividad, aprenderemos sobre el lenguaje ensamblador, específicamente utilizando NASM para el conjunto de instrucciones x86. El objetivo es entender cómo funcionan diferentes operaciones básicas en la arquitectura de computadoras a un nivel más bajo que los lenguajes de programación de alto nivel como Python o Java.

---

#### **Ejercicio 1: Resta de 3 enteros con 16 bits**

**Objetivo:** Realizar la resta de tres números enteros de 16 bits en lenguaje ensamblador x86 utilizando NASM.

**Variables utilizadas ax, dw:**
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

#### **Ejercicio 2: Multiplicación de dos números de 8 bits**

**Objetivo:** Realizar la multiplicación de dos números de un byte en lenguaje ensamblador x86 utilizando NASM.

**Variables utilizadas 8 bits ah, al, bl, db:**
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

---

#### **Ejercicio 3: División de dos números de 32 bits**

**Objetivo:** Realizar la división de dos números de 32 bits en lenguaje ensamblador x86 utilizando NASM.

**Variables utilizadas 32 bits eax, ebx ecx edx:**
- `num1` y `num2`: Son variables definidas en la sección .data que representan los dos números a dividir. Ambas están definidas como double words (dd).
- `mensaje`: Es una variable definida en la sección .data que contiene el mensaje "El resultado de la división es: " que se mostrará antes de imprimir el resultado.
- `len_mensaje`: Es una variable definida en la sección .data que contiene la longitud del mensaje.
- `linea`: Es una variable definida en la sección .data que contiene el carácter de salto de línea (0xA) para separar el mensaje del resultado.

**Proceso:**
1. Se mueven los valores de `num1` y `num2` a los registros eax y ebx respectivamente.
2. Se realiza la división de eax por ebx y se almacena el cociente en eax y el residuo en edx.
3. Se convierte el cociente a ASCII y se almacena en la memoria en la variable `resultado`.
4. Se imprime el mensaje "El resultado de la división es: ".
5. Se imprime el resultado de la división.
6. Se imprime un salto de línea para separar el mensaje del resultado.

