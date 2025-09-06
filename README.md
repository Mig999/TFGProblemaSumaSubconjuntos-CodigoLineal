# TFG Problema Suma Subconjuntos y Codigo Lineal

En este repositorio expongo el código que usé en mi TFG sobre criptografía y problemas NP. La idea principal es generar un sistema criptográfico a partir de problemas NP. Estos problemas se escogen como casos particulares fácilmente resolubles y después se camuflan como casos generales. En este caso la clave privada te permite deshacer las transformaciones aplicadas al problema y revertirlo a su versión fácil. Por último, se aplican algoritmos genéticos para intentar romper estos criptosistemas. El resultado es que los criptosistemas son bastante resistentes y los algoritmos genéticos no son una buena técnica para enfrentarlos al carecer de una correcta función de perdida.

## Problem de Suma de Subconjuntos

Dado una lista de enteros positivos y dada un valor suma objetivo, se debe de devolver los valores de la lista que se deben sumar para obtener el valor objetivo

## Problema de Código lineal

Dada una matriz lineal que permita recuperar errores con la que se codificarán los mensajes, en nuestro caso matrices goopa. Se le aplica al mensaje codificado el máximo número de errores que la matriz permite corregir y, después, se transforma la matriz mediante matrices regulares en otra genérica. La matriz obtenida será la clave pública y las matrices con las que modificamos la original la privada.

## Algoritmos genéticos

Para intentar romper los criptosistemas que usan estos problemas NP usamos algoritmos genéticos. Estos algoritmos parten de posibles soluciones aleatorias, calculan como de cerca se encuentran de la solución correcta y de las mejores soluciones actuales crean una nueva generación de soluciones mezclandolas entre ellas.

Para estos criptosistemas en particular no se puede obtener una buena función para calcular como de cerca nos encontramos de la solución correcta. Por tanto, no obtenemos buenos resultados por este método.
