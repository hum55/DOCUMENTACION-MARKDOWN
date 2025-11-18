# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Humberto Ramirez Gruintal
## Actividad \#16 - Matrices doc

---

# Cálculo de determinantes
## EJERCICIO 1

### Determinante de una matriz 2×2
Para una matriz de la forma:

$$
A=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$

la fórmula del determinante es:

$$
\det(A) = ad - bc
$$

---

### Aplicación de la fórmula a la matriz dada

$$
A=
\begin{pmatrix}
4 & 5 \\
-3 & 2 \\
\end{pmatrix}
$$

Identificamos:

- \(a = 4\),  
- \(b = 5\),  
- \(c = -3\),  
- \(d = 2\).

Sustitución:

$$
\det(A) = (4)(2) - (5)(-3)
$$

Desarrollo:

$$
\det(A) = 8 - (-15) = 8 + 15 = 23
$$

Resultado:

$$
\boxed{23}
$$

---

# EJERCICIO 2  
## Determinante de la matriz B

Dada la matriz triangular superior:

$$
B=
\begin{pmatrix}
3 & 5 & 7 \\
0 & -3 & 1 \\
0 & 0 & -9 \\
\end{pmatrix}
$$

### Propiedad importante  
En una **matriz triangular** (superior o inferior), el determinante es simplemente el **producto de los elementos de la diagonal principal**.

Diagonal principal de B:

- \(3\)
- \(-3\)
- \(-9\)

Cálculo:

$$
\det(B) = (3)(-3)(-9)
$$

Desarrollo:

$$
\det(B) = -9 \cdot (-9) = 81
$$

Resultado:

$$
\boxed{81}
$$

---

# EJERCICIO 3  
## Determinante de la matriz C

Dada la matriz:

$$
C=
\begin{pmatrix}
8 & 7 & 6 \\
15 & 2 & 3 \\
2 & 4 & 10 \\
\end{pmatrix}
$$

Para calcular su determinante utilizamos la **regla de Sarrus** (válida para matrices 3×3).

---

### Regla de Sarrus

Extendemos las dos primeras columnas:

\[
\begin{vmatrix}
8 & 7 & 6 \\
15 & 2 & 3 \\
2 & 4 & 10 \\
\end{vmatrix}
=
\begin{matrix}
8 & 7 & 6 & 8 & 7 \\
15 & 2 & 3 & 15 & 2 \\
2 & 4 & 10 & 2 & 4 \\
\end{matrix}
\]

### Suma de diagonales positivas

\[
(8)(2)(10) + (7)(3)(2) + (6)(15)(4)
\]

\[
= 160 + 42 + 360 = 562
\]

### Suma de diagonales negativas

\[
(6)(2)(2) + (8)(3)(4) + (7)(15)(10)
\]

\[
= 24 + 96 + 1050 = 1170
\]

### Determinante

\[
\det(C) = 562 - 1170 = -608
\]

Resultado:

$$
\boxed{-608}
$$

---

# EJERCICIO 4  
## Determinante del producto \(BC\)

Recordemos una propiedad importante:

### Propiedad fundamental  
\[
\det(BC) = \det(B) \cdot \det(C)
\]

Ya tenemos:

- \(\det(B) = 81\)
- \(\det(C) = -608\)

Entonces:

\[
\det(BC) = (81)(-608)
\]

Cálculo:

\[
81 \cdot -608 = -49248
\]

Resultado final:

$$
\boxed{-49248}
$$

---





