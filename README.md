# Proyecto final 2023

# Matemáticas para Ciencia de Datos

## Integrantes

- B. M. José Carlos
- C. F. Axel
- E. F. Mario

## Planteamiento del problema

**Considere una imagen que consta de un rectángulo de, digamos, 200×300 píxeles donde cada valor es un número entero entre 0 y 255. El archivo de imagen se puede codificar en una A matriz grande (200 × 300) con valores enteros en este rango y viceversa e.g. http://facundoq.github.io/courses/images/res/04_imagenes_numpy.html. Las imágenes que solemos ver tienen mucha estructura y contienen información descrita con mucha precisión, sin embargo es posible recodificar la información con menos datos. Una idea natural es usar la SVD de la matriz A. Dada una imagen, es posible elegir un $k$, tal que $σ_{k+1}$ sea lo suficientemente pequeño para considerar que $A^{(k)}$ es cercana a $A$, e.g. $σ_{k+1}$ < $1$, ver (1). La idea intuitiva, es que imágenes provenientes de la realidad tienen una estructura rica, no son representadas por matrices aleatorias, por tanto, la información relevante debe estar incluída en la matriz $A^{(k)}$, con un $k$ mucho menor a $r$ = rank $A$.**

## Instrucciones

1. Haz un programa que dada una matriz $A$ y $k$ regrese $A^{(k)}$, $σ_1$, . . . $σ_{k+1}$. Usa la librería https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html.

2. Crea una matriz de la "imagen en blanco". ¿Cuál es el rank de esa matriz? Responde la misma pregunta con la matriz corespondiente a una imagen nítida de la bandera de Indonesia y también de la bandera Italiana.

3. Elija una fotografía de tu interés. Encuentra la mejor aproximación de rango $k$ para $k$ = 2, 5, 10, 15. Conviértelos a imagen otra vez y obsérvalas junto con la imagen original. Puedes probar con otras imágenes y valores de $k$.
