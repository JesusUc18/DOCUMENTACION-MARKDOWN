# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Jesús Omar Uc Domínguez
## Actividad #22 - Resolución de Sistemas de Ecuaciones por Métodos Matriciales

---

# Ejercicio 1 — Resolver el sistema por todos los métodos

Sistema original:

\[
\begin{cases}
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
\]

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

1. \( F_2 \leftarrow F_2 - 2F_1 \)  
2. \( F_3 \leftarrow F_3 - F_1 \)  
3. \( F_3 \leftarrow F_3 + F_2 \)

### Resultado escalonado

$`\begin{bmatrix}
1 & 1 & 1 & | & 6 \\
0 & -3 & -1 & | & -9 \\
0 & 0 & 2 & | & 4
\end{bmatrix}`$

### Solución por sustitución

- De la última fila: \( 2z = 4 \Rightarrow z = 2 \)  
- Sustituyendo en la segunda fila:  
  \( -3y - 1(2) = -9 \Rightarrow y = 3 \)  
- Finalmente en la primera:  
  \( x + 3 + 2 = 6 \Rightarrow x = 1 \)

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

1. \( F_3 \leftarrow \frac{1}{2}F_3 \)  
2. \( F_2 \leftarrow F_2 + F_3 \)  
3. \( F_1 \leftarrow F_1 - F_3 \)  
4. \( F_1 \leftarrow F_1 - F_2 \)

### Resultado final en forma reducida

$`\begin{bmatrix}
1 & 0 & 0 & | & 1 \\
0 & 1 & 0 & | & 3 \\
0 & 0 & 1 & | & 2
\end{bmatrix}`$

---

## Matriz inversa  

Para resolver \( AX = B \) se calcula \( X = A^{-1}B \).

### Matriz de coeficientes

$`A = \begin{bmatrix}
1 & 1 & 1 \\
2 & -1 & 1 \\
1 & 2 & -1
\end{bmatrix}`$

### Vector de resultados

$B = \begin{bmatrix} 6 \\ 3 \\ 2 \end{bmatrix}$

$X = A^{-1}B$

### Resultado  

$X = \begin{bmatrix} 1 \\ 3 \\ 2 \end{bmatrix}$

---

## Regla de Cramer  

Se usa el determinante de la matriz y los determinantes de matrices modificadas para cada variable.

- Determinante:

$\( \det(A) = 6$

- Se reemplazan columnas según la variable a calcular.

### Resultados

- x = 1 
- y = 3 
- z = 2 

---

# **Solución final del Ejercicio 1**  

$(x,y,z) = (1,3,2)$

---
