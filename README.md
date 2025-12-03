# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Humberto Ramirez Gruintal 
## Actividad \#22 - Matrices doc

# Ejercicio 1: Resolver con todos los métodos

Sistema de ecuaciones:

1) x + y + z = 6  
2) 2x - y + z = 3  
3) x + 2y - z = 2  

# a) Método de Gauss (Eliminación Gaussiana)

Objetivo: Llegar a una matriz escalonada.

**Paso 1: Matriz Inicial**

| 1 | 1 | 1 | 6 |
|---|---|---|---|
| 2 | -1 | 1 | 3 |
| 1 | 2 | -1 | 2 |

**Paso 2: Hacer ceros debajo del primer 1**

- F2 = F2 - 2F1  
- F3 = F3 - F1  

| 1 | 1 | 1 | 6 |
|---|---|---|---|
| 0 | -3 | -1 | -9 |
| 0 | 1 | -2 | -4 |

**Paso 3: Intercambiar F2 y F3**

| 1 | 1 | 1 | 6 |
|---|---|---|---|
| 0 | 1 | -2 | -4 |
| 0 | -3 | -1 | -9 |

**Paso 4: Eliminar el -3**

- F3 = F3 + 3F2

| 1 | 1 | 1 | 6 |
|---|---|---|---|
| 0 | 1 | -2 | -4 |
| 0 | 0 | -7 | -21 |

**Paso 5: Sustitución hacia atrás**
- z = 3  
- y = 2  
- x = 1  

---

# b) Método de Gauss-Jordan

Partimos de:

| 1 | 1 | 1 | 6 |
|---|---|---|---|
| 0 | 1 | -2 | -4 |
| 0 | 0 | -7 | -21 |

**Paso 1: F3 / -7**

| 1 | 1 | 1 | 6 |
|---|---|---|---|
| 0 | 1 | -2 | -4 |
| 0 | 0 | 1 | 3 |

**Paso 2: Hacer ceros arriba**

- F2 = F2 + 2F3  
- F1 = F1 - F3  

| 1 | 1 | 0 | 3 |
|---|---|---|---|
| 0 | 1 | 0 | 2 |
| 0 | 0 | 1 | 3 |

**Paso 3: F1 = F1 - F2**

| 1 | 0 | 0 | 1 |
|---|---|---|---|
| 0 | 1 | 0 | 2 |
| 0 | 0 | 1 | 3 |

Resultados: x = 1, y = 2, z = 3

---

# c) Método de Matriz Inversa

Matriz A:

| 1 | 1 | 1 |
|---|---|---|
| 2 | -1 | 1 |
| 1 | 2 | -1 |

Det = 7

**Inversa (1/7 · adj(A))**

| -1 | 3 | 2 |
|----|---|---|
| 3 | -2 | 1 |
| 5 | -1 | -3 |

**Multiplicación por B = (6,3,2)**  
x = 1  
y = 2  
z = 3  

---

# d) Regla de Cramer

Det(A) = 7

**Determinante X**

| 6 | 1 | 1 |
|---|---|---|
| 3 | -1 | 1 |
| 2 | 2 | -1 |

Det X = 7  
x = 7/7 = 1

**Determinante Y**

| 1 | 6 | 1 |
|---|---|---|
| 2 | 3 | 1 |
| 1 | 2 | -1 |

Det Y = 14  
y = 14/7 = 2

**Determinante Z**

| 1 | 1 | 6 |
|---|---|---|
| 2 | -1 | 3 |
| 1 | 2 | 2 |

Det Z = 21  
z = 21/7 = 3

---

# Ejercicio 2: Identificar tipo de solución

### a)
x + y = 3  
2x + 2y = 6  

→ Infinitas soluciones.

### b)
x + y = 3  
2x + 2y = 7  

→ Ninguna solución.

### c)
x + y = 3  
x − y = 1  

→ Solución única.

---

# Ejercicio 3: Sistema 4x4

Sistema:

1) x + y + z + w = 10  
2) 2x + y − z + w = 5  
3) x − y + z − w = 1  
4) x + y − z + 2w = 8  

Soluciones:

- z = 3.5  
- w = 5  
- x = 2  
- y = -0.5  

---

# Ejercicio 4: Aplicación práctica (Mix de Productos)

Sistema:

- 2P + 1S + 3U = 100  
- 3P + 1S + 2U = 120  
- 1P + 2S + 1U = 80  

Resultados:

- P = 27.5  
- S = 22.5  
- U = 7.5  

---
