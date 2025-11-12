# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Humberto Ramirez Gruintal 
## Actividad \#16 - Matrices doc

---
### Identificación de matrices

Matriz identidad, porque la diagonal está compuestos por solo unos y los elementos fuera de la diagonal son ceros.

$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

MUESTRA

Calcula la suma de A y B

$$ A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
9 & 10 & 11 \\
12 & 13 & 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
1 + 9 & 2 + 10 & 3 + 11 \\
4 + 12 & 5 + 13 & 6 + 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
10 & 12 & 14 \\
16 & 18 & 20 \\
\end{pmatrix}
$$

---
# OTRO EJERCICIO
# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Humberto Ramirez Gruintal
## Actividad \#16 - Matrices doc

---
# Identificación de matrices
## EJERCICIO 1

### Matriz identidad, porque la diagonal está compuesta por solo unos y los elementos fuera de la diagonal son ceros.
Además, es importante notar que al multiplicarla por otra matriz, esta no modifica los valores de la misma.

$$ A 
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

### Matriz diagonal, todos los valores fuera de la diagonal tienen un valor de 0.
Los elementos en la diagonal pueden ser distintos de 1, lo importante es que estén alineados diagonalmente.

$$ B
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5\\
\end{pmatrix}
$$

### Matriz cuadrada, tiene el mismo número de filas y columnas.
Este tipo de matriz permite calcular determinantes e inversas.

$$ C
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

### Matriz triangular superior. Todos los elementos debajo de la diagonal principal son cero.
Se utiliza frecuentemente en factorización de matrices.

$$ D
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

---

## EJERCICIO 2

### Suma de matrices A y B
Para sumar matrices, se suman elemento a elemento. Esto solo es posible si ambas matrices tienen la misma dimensión.

$$ A =
\begin{pmatrix}
2 & -1  \\
3 & 4  \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
5 & 2  \\
-1 & 3 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
2 + 5 & -1 + 2  \\
3 + -1 & 4 + 3 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
7 & 1 \\
2 & 7 \\
\end{pmatrix}
$$

---

### Resta de matrices (2A - B)
Primero se multiplica cada elemento de A por 2. Después, se resta elemento a elemento la matriz B.

$$ 2A  =
\begin{pmatrix}
4 & -2 \\
6 & 8 \\
\end{pmatrix}
$$

$$ 2A - B =
\begin{pmatrix}
4 - 5 & -2 - 2  \\
6 - -1 & 8 - 3 \\
\end{pmatrix}
$$

$$ 2A - B =
\begin{pmatrix}
-1 & -4 \\
7 & 5 \\
\end{pmatrix}
$$

---

### Producto AB
Para multiplicar matrices, se toma el producto punto entre filas de A y columnas de B.

$$ AB =
\begin{pmatrix}
(2 * 5 + -1 * -1) & (2 * 2 + -1 * 3)  \\
(3 * 5 + 4 * -1) & (3 * 2 + 4 * 3) \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
11 & 1 \\
11 & 18 \\
\end{pmatrix}
$$

Este resultado demuestra que la multiplicación de matrices no es elemento a elemento.

---

### Producto BA (no conmutativo)
Se demuestra que AB ≠ BA en la mayoría de los casos.

$$ BA =
\begin{pmatrix}
(5 * 2 + 2 * 3) & (5 * -1 + 2 * 4)  \\
(-1 * 2 + 3 * 3) & (-1 * -1 + 3 * 4) \\
\end{pmatrix}
$$

$$ BA=
\begin{pmatrix}
16 & 3 \\
7 & 13 \\
\end{pmatrix}
$$

Esto comprueba que la multiplicación matricial **no es conmutativa**.

---

### Transpuesta de A
La transpuesta consiste en intercambiar filas por columnas.

$$ AT =
\begin{pmatrix}
2 & 3  \\
-1 & 4  \\
\end{pmatrix}
$$

---

# EJERCICIO 3

Multiplicación de cadena

Las multiplicaciones deben realizarse siguiendo el orden indicado, ya que aunque se cumple la propiedad asociativa, los resultados intermedios pueden cambiar.

$$ A =
\begin{pmatrix}
1 & 2  \\
3 & 4  \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
2 & 0  \\
1 & 3 \\
\end{pmatrix}
$$

$$ C =
\begin{pmatrix}
1 & 1  \\
0 & 2 \\
\end{pmatrix}
$$

---

### Parte 1: AB

$$ AB =
\begin{pmatrix}
(1 * 2 + 2 * 1) & (1 * 0 + 2 * 3)  \\
(3 * 2 + 4 * 1) & (3 * 0 + 4 * 3) \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
4 & 6 \\
10 & 12 \\
\end{pmatrix}
$$

---

### Parte 2: (AB)C
Se toma la matriz resultante AB y se multiplica por C.

$$ (AB)C =
\begin{pmatrix}
(4 * 1 + 6 * 0) & (4 * 1 + 6 * 2)  \\
(10 * 1 + 12 * 0) & (10 * 0 + 12 * 2) \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
4 & 16 \\
10 & 24 \\
\end{pmatrix}
$$

---

## Verificación de que (AB)C = A(BC)

Esta propiedad es conocida como **asociativa** en la multiplicación de matrices.

### Parte 1: BC

$$ BC =
\begin{pmatrix}
(2 * 1 + 0 * 0) & (2 * 1 + 0 * 2)  \\
(1 * 1 + 3 * 0) & (1 * 1 + 3 * 2) \\
\end{pmatrix}
$$

$$ BC =
\begin{pmatrix}
2 & 2 \\
1 & 7 \\
\end{pmatrix}
$$

---

### Parte 2: A(BC)

$$ A(BC) =
\begin{pmatrix}
(1 * 2 + 2 * 1) & (1 * 2 + 2 * 7)  \\
(3 * 2 + 4 * 1) & (3 * 2 + 4 * 7) \\
\end{pmatrix}
$$

$$ A(BC) =
\begin{pmatrix}
4 & 16 \\
10 & 34 \\
\end{pmatrix}
$$

---

Con esta verificación podemos confirmar que la propiedad asociativa se cumple:  
$$(AB)C = A(BC)$$





