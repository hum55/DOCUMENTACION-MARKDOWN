# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: HUMBERTO RAMIREZ GRUINTAL
## Actividad \#20 - Matrices doc

---

## Objetivo

El objetivo de esta práctica es comprender y aplicar operaciones algebraicas matriciales utilizando Microsoft Excel como herramienta de procesamiento. Se busca interpretar imágenes digitales como matrices de valores numéricos (píxeles), donde cada celda representa la intensidad de color o escala de grises.

A través de esta actividad, se demostrará cómo las operaciones de **suma, resta, multiplicación por un escalar, transposición y composición lineal** afectan visual y matemáticamente a la información contenida en las matrices originales.

---

## Programación de la hoja de Excel

A continuación, la explicación matemática y las fórmulas de Excel utilizadas para cada hoja de cálculo dentro del archivo 

### 1. Imágenes Base (Matrices Originales)
**Hojas:** `imagen1`, `imagen2`, `imagen3`, `imagen4`, `imagen5`

* **Descripción:** Estas hojas contienen los datos de entrada. Cada celda representa un píxel con un valor numérico. No contienen fórmulas, son valores constantes ($input$).
* **Representación:** Matriz $A$ de tamaño $m \times n$.

### 2. Suma de Matrices
**Hoja:** `suma`

* **Descripción:** Se realiza la adición aritmética de dos matrices. Esto resulta visualmente en la superposición de las dos imágenes originales.
* **Operación Matemática:**
  $$C_{ij} = A_{ij} + B_{ij}$$
* **Fórmula en Excel:**
  ```excel
  ='imagen1'!A1 + 'imagen2'!A1
  
  ### Resta de Matrices
**Hoja:** `resta`

* **Descripción:** Se calcula la diferencia aritmética entre dos matrices. Visualmente, esta operación es fundamental para detectar cambios, encontrar contornos o analizar variaciones de intensidad entre dos imágenes ("imagen1" e "imagen2").
* **Operación Matemática:**
  $$C_{ij} = A_{ij} - B_{ij}$$
* **Fórmula en Excel:**
  ```excel
  ='imagen1'!A1 - 'imagen2'!A1

  ### Multiplicación por Escalar (Escalado)
**Hoja:** `multi escalar`

* **Descripción:** Consiste en multiplicar cada elemento ($A_{ij}$) de la matriz `imagen2` por un número constante fijo (el escalar $k$).
    * Si el escalar $k$ está entre 0 y 1 (ejemplo: $k=0.5$), la intensidad de la imagen se **reduce** (oscurece).
    * Si $k$ es mayor a 1, la intensidad de la imagen se **incrementa** (aclara).
* **Operación Matemática:**
  $$R_{ij} = k \cdot A_{ij}$$
* **Fórmula en Excel:**
  ```excel
  ='imagen2'!A1 * 0.5

  ### 5. Transpuesta de una Matriz
**Hojas:** `trans1`, `TRAS2`, `TRAS3`, `TRAS4`, `TRAS5`

* **Descripción:** La transposición de una matriz (o imagen) consiste en **intercambiar sus filas por sus columnas**. Si la matriz original $A$ tiene una dimensión $m \times n$, la matriz transpuesta $A^T$ tendrá una dimensión $n \times m$. Visualmente, esto genera una rotación o reflejo de la imagen.
* **Operación Matemática:**
    La notación $A^T_{ij}$ significa que el elemento ubicado en la fila $i$ y columna $j$ de la matriz transpuesta es igual al elemento que estaba en la fila $j$ y columna $i$ de la matriz original $A$.
    $$A^T_{ij} = A_{ji}$$
* **Fórmula en Excel (Método de Matriz Dinámica):**
    Esta fórmula se introduce en la primera celda del rango de destino (ej. A1 de la hoja `trans1`) y se aplica a todo el rango de forma automática.
    ```excel
    =TRANSPONER('imagen1'!A1:Z30)
    ```
    *Nota: Si se usa una versión antigua de Excel que requiere referenciar celda por celda:*
    ```excel
    =INDICE('imagen1'!$A$1:$Z$30; COLUMNA(); FILA())
    ```

    ### 6. Composición Lineal (Combinación)
**Hoja:** `COMPOSI`

* **Descripción:** Esta operación implica la **suma de múltiples matrices** (`imagen1`, `imagen2`, etc.), donde cada matriz ha sido previamente multiplicada por un escalar distinto (llamado **coeficiente** o **peso**). El resultado es una matriz $R$ que combina las propiedades de todas las matrices de entrada de manera ponderada. En el procesamiento de imágenes, permite crear efectos complejos como superposiciones con distintos niveles de opacidad o aplicar filtros.
* **Operación Matemática:**
    La matriz resultante $R$ es la combinación lineal de las matrices $A, B, C, D, E$ con sus respectivos escalares $k_1, k_2, k_3, k_4, k_5$:
    $$R = k_1A + k_2B + k_3C + k_4D + k_5E$$
    A nivel de elemento:
    $$R_{ij} = k_1A_{ij} + k_2B_{ij} + k_3C_{ij} + k_4D_{ij} + k_5E_{ij}$$
* **Fórmula en Excel (Ejemplo de Celda A1):**
    ```excel
    =('imagen1'!A1 * 2) + ('imagen2'!A1 * 3) + ('imagen3'!A1 * 0.5) + ('imagen4'!A1 * 4) + ('imagen5'!A1 * 1)
    ```
 \hline
9 & 8 & 7 \\ \hline
6 & 5 & 4 \\ \hline
3 & 2 & 1 \\ \hline
\end{array}
\]

