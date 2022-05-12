# Aprendiendo-Sass
Este repositorio contiene los fundamentos basicos de sass
## ¿Por qué creo que sas es mejor para desarrollo?
Lo primero es que sass ayuda en un desarrollo de frontend mucho más rápido puesto que puedes declarar variabless y asignarlas directamente a los stilos que queramos.
Esto representa una ventaja frente a la declaración de variables CSS deben estar encerradas en un bloque. 
Además de que en CSS se debe hacer uso de la función var() para poder utilizar variables.

***


### Ejemplo
CSS
```
body {
  /* Declaración */
  --color: red;

  /* Usando la variable */
  color: var(--color);
}
```
SASS
```
/* Declaración */
$color: red;

body {
  /* Usando la variable */
  color: $color;
}
```
***

También dispone de operaciones aritmétcas en SASS se hace como en cualquier otro lenguaje, mientras que en CSS necesitamos la función calc().

***
##Interpolacion
Una gran ventaja es que no sólo podemos guardar valores, sino el dato que deseemos e interporlar la variable. El uso más frecuente de esto es el de poder crear selectores con variables. 
Ejemplo:
```
$red: red;

// Compila a .container.red 
.container.#{$red} {
  color: $red;
}
```
