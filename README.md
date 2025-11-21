# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Jesús Omar Uc Domínguez
## Actividad #18 - Matrices Doc

---
# Ejercicio 1: Determinantes 2×2

**Calcula los determinantes:**


## 1. Primera matriz

$$
A =
\begin{pmatrix}
5 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

1. Calculamos los determinantes en diagonal.  
2. Multiplicamos 3 * 2 (-1) = -6  
3. Multiplicamos 5 * 1 (1) = 5  
4. Hacemos la resta correspondiente: 5 - 6 = -1

**A = det(A) = -1**


## 2. Segunda matriz

$$
B =
\begin{pmatrix}
-1 & 4 \\
2 & -8 \\
\end{pmatrix}
$$

1. Calculamos los determinantes en diagonal.  
2. Multiplicamos 2 * 4 (-1) = -8  
3. Multiplicamos (-1) (-8) (1) = 8  
4. Hacemos la resta correspondiente: 8 - 8 = 0  

**B = det(B) = 0**


## 3. Tercera matriz

$$
C =
\begin{pmatrix}
6 & 9 \\
2 & 3 \\
\end{pmatrix}
$$

1. Calculamos los determinantes en diagonal.  
2. Multiplicamos 2 * 9 (-1) = -18  
3. Multiplicamos 6 * 3 (1) = 18  
4. Hacemos la resta correspondiente: 18 - 18 = 0  

**C = det(C) = 0**


## 4. Cuarta matriz

$$
D =
\begin{pmatrix}
0 & 5 \\
-5 & 0 \\
\end{pmatrix}
$$

1. Calculamos los determinantes en diagonal.  
2. Multiplicamos (-5) * 5 (-1) = 25  
3. Multiplicamos 0 * 0 (1) = 0  
4. Hacemos la resta correspondiente: 25 - 0 = 25 

**D = det(D) = 25**

---

# Ejercicio 2: Regla de Sarrus

Usa Sarrus para calcular:

---

## 1. Primera matriz

$$
E =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
\end{pmatrix}
$$

1. Colocamos una línea debajo de la matriz  
2. Copiamos en orden las filas 1 y 2

$$
E =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
1 & 2 & 3 \\
0 & 1 & 4 \\
\end{pmatrix}
$$

3. Calculamos primero las diagonales negativas:

- 0 × 2 × 3 = 0  
- 1 × 6 × 4 = 24  
- 5 × 1 × (-3) = -15  

**TOTAL = 39**

4. Calculamos ahora las diagonales positivas:

- 1 × 1 × 0 = 0  
- 0 × 6 × 3 = 0  
- 5 × 2 × 4 = 40  

**TOTAL = 40**

5. Hacemos la resta correspondiente:  
40 − 39 = **1**

**E = det(E) = 1**

---

## 2. Segunda matriz

$$
F =
\begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 0 & -2 \\
\end{pmatrix}
$$

1. Colocamos una línea debajo de la matriz  
2. Copiamos en orden las filas 1 y 2

$$
F =
\begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 0 & -2 \\
2 & -1 & 3 \\
1 & 4 & 0 \\
\end{pmatrix}
$$

3. Calculamos primero las diagonales negativas:

- 1 × 0 × 3 = 0  
- 4 × 0 × 2 = 0  
- 3 × (-1) × (-2) = 36  

**TOTAL = 38**

4. Calculamos ahora las diagonales positivas:

- 2 × 4 × (-2) = -16  
- 1 × 0 × 3 = 0  
- 3 × (-1) × 0 = 0  

**TOTAL = -16**

5. Hacemos la resta correspondiente:  
38 − (−16) = 38 + 16 = **54**

**F = det(F) = 54**

---

# Ejercicio 3: Calcula usando cofactores (expandir por la fila o columna más conveniente) 

### 1.- 

$$ G =
\begin{pmatrix}
1 & 0 & 2\\
-1 & 3 & 1\\
2 & 0 & 1\\
\end{pmatrix}
$$

1. A la primera columna se agrega un símbolo positivo y en la siguiente negativo, asi sucesivamente con todas las columnas.
   
2. Tomamos el +1 de la fila 1 y columna 1, tapamos los números que estan debajo de el y tomamos solo los restantes de las filas 2 y 3.

```
1 | 3 1 |
  | 0 1 |
```

3. Hacemos lo mismo con el 0, es decir, tapamos los números debajo de el y agarramos los restantes de la fila 2 y 3.

```
0 | -1 1 |
  | 2 1  |
```

4. Lo mismo con el +2, ahora solo con los números restantes que no esten debajo de el.

```
2 | -1 3 |
  | 2 0  |
```

5. Hacemos multiplicaciones cruzadas de los números dentro de la matriz, como al sacar determinante, solo que despues multiplicamos por el número de afuera.

```
1 | 3 1 | = 1 + 3 = 3, 0 * 1 = 0. ENTONCES: 1(3 - 0)
  | 0 1 |
```

```
0 | -1 1 | = -1 * 1 = -1, 2 * -1 = -2. ENTONCES: 0(-1-2)
  | 2 1  |
```

```
2 | -1 3 | = -1 * 0 = 0, 2 * -3 = -6. ENTONCES: 2(0-6)
  | 2 0  |
```

6. Juntamos y resolvemos, respetando signos

- det(G) = 1(3-0) - 0(-1-2) + 2(0-6)
- det(G) = 3 - 12
- det(G) = -9

---

# Ejercicio 4: Dadas A y B, verifica que:

- det(AB) = det(A) * det(B)
- det(A^T) = det(A)

### Primer caso

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
1 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

### 1. Calculamos det(A)

A =  
| 2  1 |  
| 1  3 |

det(A) = (2)(3) - (1)(1) = 6 - 1 = **5**

---

### 2. Calculamos det(B)

B =  
| 1  2 |  
| 3  1 |

det(B) = (1)(1) - (2)(3) = 1 - 6 = **-5**

---

### 3. Calculamos AB

AB =  
| 2·1 + 1·3   ,   2·2 + 1·1 |  
| 1·1 + 3·3   ,   1·2 + 3·1 |

AB =  
| 5   5 |  
| 10  5 |

---

### 4. Calculamos det(AB)

det(AB) = (5)(5) - (5)(10) = 25 - 50 = **-25**

---

### 5. Verificamos det(AB) = det(A) * det(B)

det(A) * det(B) = 5 * (-5) = **-25**

Por lo tanto det(AB) **SI ES IGUAL** a det(A) * det(B)

---

### Segundo caso 

La matriz A es:

A =
| 2  1 |
| 1  3 |

Cuando calculamos la transpuesta Aᵀ, lo único que hacemos es intercambiar filas por columnas:

Aᵀ =  
| 2  1 |  
| 1  3 |

En este caso, la transpuesta es exactamente igual a la matriz original porque A es **simétrica**.  

Como la matriz no cambia al transponerla, su determinante tampoco puede cambiar. Por lo tanto:

- det(Aᵀ) = det(A)
- det(Aᵀ) = 5

Esto confirma la propiedad:  
**El determinante de una matriz siempre es igual al determinante de su transpuesta.**

---

# Ejercicio 5: Dado los vectores u = (3, 2) y v = (1, 4)

### a) Calcula el área del palalelogramo que forman

1. Pasamos a matriz los vectores

$$ A =
\begin{pmatrix}
3 & 2 \\
1 & 4 \\
\end{pmatrix}
$$

2. Sacamos su determinante
   
3. Multiplicar: 3 * 4 = 12, 1 * -2 = -2

4. Restamos: 12 - 2 = 10

5. Área es igual a 10

### b) ¿Cambia el área si intercambias los vectores?

No cambia ya que aunque se cambie el signo, el tamaño sigue siendo el mismo.

Es decir:

$$ A =
\begin{pmatrix}
1 & 4 \\
3 & 2 \\
\end{pmatrix}
$$

Si sacamos su determinante asi, nos da -10, cambia el signo pero no el tamaño.

### c) ¿Qué representa el signo del determinante?

Principalmente la dirección en que se ingresa el valor.

