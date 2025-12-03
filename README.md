# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Jesús Omar Uc Domínguez
## Actividad #22 - Resolución de Sistemas de Ecuaciones por Métodos Matriciales

---

# Ejercicio 1 — Resolver el sistema por todos los métodos

Sistema original:

$`\begin{cases}
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
`$

---

## Método Gauss  

El método de Gauss consiste en transformar la matriz aumentada en una forma escalonada mediante operaciones elementales, permitiendo resolver el sistema por sustitución hacia atrás.

### Matriz aumentada inicial  

$`\begin{bmatrix}
1 & 1 & 1 & | & 6 \\
2 & -1 & 1 & | & 3 \\
1 & 2 & -1 & | & 2
\end{bmatrix}`$

### Operaciones realizadas

1. (F2 ---> F2 - 2.F1)  
2. (F3 ---> F3 - F1)  
3. (F3 ---> F3 + F2)

### Resultado escalonado

$`\begin{bmatrix}
1 & 1 & 1 & | & 6 \\
0 & -3 & -1 & | & -9 \\
0 & 0 & 2 & | & 4
\end{bmatrix}`$

### Soluciones

+ (z = 2)  
+ (y = 3)  
+ (x = 1)

---

## Método Gauss–Jordan  

Este método continúa el proceso hasta obtener una matriz identidad, dejando explícitas las soluciones sin necesidad de sustitución.

Partimos de la forma escalonada anterior:

$`\begin{bmatrix}
1 & 1 & 1 & | & 6 \\
0 & -3 & -1 & | & -9 \\
0 & 0 & 2 & | & 4
\end{bmatrix}`$

### Operaciones realizadas

1. (F3 ---> 1/2.F_3)  
2. (F2 ---> F2 + F3)  
3. (F1 ---> F1 - F3)  
4. (F1 ---> F1 - F2)

### Resultado final en forma reducida

$`\begin{bmatrix}
1 & 0 & 0 & | & 1 \\
0 & 1 & 0 & | & 3 \\
0 & 0 & 1 & | & 2
\end{bmatrix}`$

---

## Matriz inversa  

### Matriz de coeficientes

$`A = \begin{bmatrix}
1 & 1 & 1 \\
2 & -1 & 1 \\
1 & 2 & -1
\end{bmatrix}`$

### Vector de resultados

$`B = 
\begin{pmatrix}
6 \\ 3 \\ 2
\end{pmatrix}
`$


### Resultado  

$`X = A^{-1} B =
\begin{pmatrix}
1 \\ 3 \\ 2
\end{pmatrix}
`$


---

## Regla de Cramer  

Se usa el determinante de la matriz y los determinantes de matrices modificadas para cada variable.

- Determinante:

$$
\det(A) = 6
$$

- Se reemplazan columnas según la variable a calcular.

### Resultados

+ (x = 1)  
+ (y = 3)  
+ (z = 2) 

---

# **Solución final del Ejercicio 1**  

$$
(x, y, z) = (1, 3, 2)
$$

---

# Ejercicio 2 — Tipo de solución

### a)  
Sistema **dependiente** → tiene **infinitas soluciones**.

### b)  
Sistema **incompatible** → **no tiene solución**.

### c)  
Sistema **compatible determinado** → **solución única**.

---

#  Ejercicio 3 — Sistema 4×4

Sistema a resolver:

$`
\begin{cases}
x + y + z + w = 10 \\
2x + y - z + w = 5 \\
x - y + z - w = 1 \\
x + y - z + 2w = 8
\end{cases}
`$

### Matriz aumentada inicial

$`\begin{bmatrix}
1 & 1 & 1 & 1 & | & 10 \\
2 & 1 & -1 & 1 & | & 5 \\
1 & -1 & 1 & -1 & | & 1 \\
1 & 1 & -1 & 2 & | & 8
\end{bmatrix}`$

### Resultado después de Gauss

$`\begin{bmatrix}
1 & 1 & 0 & 0 & | & 3 \\
0 & 1 & 0 & 1 & | & 4 \\
0 & 0 & 1 & 1 & | & 3 \\
0 & 0 & 0 & 1 & | & 1
\end{bmatrix}`$

Soluciones:

$w = 1$  
$z = 2$  
$y = 3$  
$x = 0$

---

# Ejercicio 4 — Aplicación práctica

Matrices de producción:  
Productos: Premium (P), Standard (S), Utilitario (U)  
Materias: res (R), pollo (Q), cerdo (C)

### Sistema de ecuaciones

$`\begin{bmatrix}
2 & 1 & 3 | & P \\
3 & 1 & 2 | & S \\
1 & 2 & 1 | & U
\end{bmatrix}`$


### Reducción por Gauss

$`\begin{bmatrix}
1 & 0 & 1 & | & 20 \\
0 & 1 & 1 & | & 40 \\
0 & 0 & 1 & | & 20
\end{bmatrix}`$

### Resultados

$U = 20$

$S = 20$

$P = 0$

---

