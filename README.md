# BuscaminasConsolaKTenunciado

- Nombre de proyecto: BuscaMinas
  ![image.png](./image.png)
- Separar la lógica de pressentación de la lógica de negocio(dos capas
- Main.kt contendrá main() y todas las funciones que consideres necesarias para la interacción con el usuario.
- Main.kt no puede manipular directamente la modificación del tablero, existirá una función destapar(fila,columna) o similar pero no puede modificar directamente el tablero de juego
- Main.kt puede:
    - ordenar destapar una celda
    - leer el tablero, por ejemplo para imprimir, pero no puede modificar
    - consultar información de lectura como por ejemplo saber el estado del juego (finalizado o no, etc.)
- Por lo tanto, las clase/clases de Buscaminas.kt deben de cumplir el principio de ocultación de forma que que desde Main.kt sólo se puede modificar la información a través de las funciones públicas que ofrezcan las clases de Buscaminas.kt
- Buscaminas.kt al menos debe de contener una clase que se llame Buscaminas
- La clase Buscaminas se encarga de crear y gestionar el tablero de juego
- En esta versión de buscaminas se debe permitir colocar banderas (flags)
- El tablero de juego se puede implementar de muchas formas
  - Una matriz de enteros donde cada entero es un código que representa el estado de la celda
  - tres matrices paralelas para almacenar respectivamente valor, tapada/destapada, bandera/no bandera
  - Una única matriz donde cada celda es un objeto de clase Celda o similar que guarda la información de estado de una celda. Intenta usar ésta, es la más estructurada.
  - otros  
- Las dimensiones del tablero y la cantidad de minas debe ser configurable.
- La clase Buscaminas debe enviar excepción:
  -   Si el número de filas y/o columnas es <1 
  -   Si el número de minas es igual o mayor que el número de celdas del tablero debe enviar excepción
    
