# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Jesús Omar Uc Domínguez
## Actividad #16 - Matrices Doc

---
### Ejercicio 1: Clasificar Matrices

**Identifica el tipo de cada matriz:**


$$ **A** =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

**A: Matriz Identidad**, porque la diagonal está compuestos por solo unos y los elementos fuera de la diagonal son ceros.

$$ **B** =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

**B: Matriz Diagonal**, porque todos los elementos fuera de la diagonal principal son 0 y los de la diagonal son (3, -2, 5).

$$ **C** =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

**C: Matriz Simétrica**, porque ambas diagonales (superior e inferior) son iguales.

$$ **D** =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

**D: Matriz Triangular Superior**, porque todos los elementos debajo de la diagonal principal son cero.

---
### Ejercicio 2: Operaciones Básicas

**Dadas las matrices:**

$$ **A** = 
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix},
\qquad
**B** = 
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

**Calcula:**

(a = **A + B**: Se suman las matrices elemento a elemento, ed decir cada número en la misma posición se suma.

$$ **A + B** =
\begin{pmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3 \\
\end{pmatrix} =
\begin{pmatrix}
7 & 1 \\
2 & 7 \\
\end{pmatrix}
$$

(b = **2A - B**: Primero se multiplica la matriz A por 2, luego se resta B elemento a elemento.

$$ **2A** = 
\begin{pmatrix}
2 * 2 & -1 * 2 \\
3 * 2 & 4 * 2 \\
\end{pmatrix} =
\begin{pmatrix}
4 & -2 \\
6 & 8 \\
\end{pmatrix}
$$

$$ **2A - B** =
\begin{pmatrix}
4 - 5 & -2 - 2 \\
6 - (-1) & 8 - 3 \\
\end{pmatrix} =
\begin{pmatrix}
-1 & -4 \\
7 & 5 \\
\end{pmatrix}
$$

(c = **AB**: Se multiplica fila por columna: cada elemento se obtiene multiplicando y sumando dichos valores de A y B.

$$ **AB** =
\begin{pmatrix}
2(5) + -1(-1) & 2(2) + -1(3) \\
3(5) + 4(-1) & 3(2) + 4(3) \\
\end{pmatrix} =
\begin{pmatrix}
10 + 1 & 4 + (-3) \\
15 +(-4) & 6 + 12 \\
\end{pmatrix} = 
\begin{pmatrix}
11 & 1 \\
11 & 18 \\
\end{pmatrix}
$$

(d = **BA**: Igual que en el anterior, pero ahora B está primero, por eso cambia el orden de las multiplicaciones.

$$ **BA** =
\begin{pmatrix}
5(2) + 2(3) & 5(-1) + 2(4) \\
-1(2) + 3(3) & -1(-1) + 3(4) \\
\end{pmatrix} =
\begin{pmatrix}
10 + 6 & -5 + 8 \\
-2 + 9 & 1 + 12 \\
\end{pmatrix} = 
\begin{pmatrix}
16 & 3 \\
7 & 13 \\
\end{pmatrix}
$$

(e = **A^T**: Se obtiene la transpuesta de A, intercambiando filas por columnas.

$$ **A** = 
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
\qquad
**A^T** = 
\begin{pmatrix}
2 & 3 \\
-1 & 4 \\
\end{pmatrix}
$$

---
### Ejercicio 3: Multiplicación en Cadena

**Dadas las matrices:**

$$ **A** = 
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix},
\qquad
**B** = 
\begin{pmatrix}
2 & 0 \\
1 & 3 \\
\end{pmatrix},
\qquad
**C** = 
\begin{pmatrix}
1 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

**Verifica que (AB)C = A (BC)**

Primero obtengo el resultado de las matrices multiplicadas entre paréntesis.

$$ **AB** =
\begin{pmatrix}
1(2) + 2(1) & 1(0) + 2(3) \\
3(2) + 4(1) & 3(0) + 3(4) \\
\end{pmatrix} =
\begin{pmatrix}
2 + 2 & 0 + 6 \\
6 + 4 & 0 + 12 \\
\end{pmatrix} = 
\begin{pmatrix}
4 & 6 \\
10 & 12 \\
\end{pmatrix}
$$

$$ **BC** =
\begin{pmatrix}
2(1) + 0(0) & 2(1) + 0(2) \\
1(1) + 3(0) & 1(1) + 3(2) \\
\end{pmatrix} =
\begin{pmatrix}
2 + 0 & 2 + 0 \\
1 + 0 & 1 + 6 \\
\end{pmatrix} = 
\begin{pmatrix}
2 & 2 \\
1 & 7 \\
\end{pmatrix}
$$

Luego multiplico los resultados en sus respectivas operaciones: “(AB)C” y “A(BC)”.

$$ **(AB)C** =
\begin{pmatrix}
4(1) + 6(0) & 4(1) + 6(2) \\
10(1) + 12(0) & 10(1) + 12(2) \\
\end{pmatrix} =
\begin{pmatrix}
4 + 0 & 4 + 12 \\
10 + 0 & 10 + 24 \\
\end{pmatrix} = 
\begin{pmatrix}
4 & 16 \\
10 & 34 \\
\end{pmatrix}
$$

$$ **A(BC)** =
\begin{pmatrix}
1(2) + 2(1) & 1(2) + 2(7) \\
3(2) + 4(1) & 3(2) + 4(7) \\
\end{pmatrix} =
\begin{pmatrix}
2 + 2 & 2 + 14 \\
6 + 4 & 6 + 28 \\
\end{pmatrix} = 
\begin{pmatrix}
4 & 16 \\
10 & 34 \\
\end{pmatrix}
$$








