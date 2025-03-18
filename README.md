# BuscaminasConsolaKTenunciado

# BuscaminasEnunciadoKT
## Se Pide hay que actualizar dibujo y estructura
- Nombre de proyecto: BuscaMinas
- Separar el interface de usuario de la lógica del juego.  Habrá dos paquetes. Uno se llamará principal y contiene la clase InterfaceConsola que contiene el main() . El otro se llamará buscaminas y contendrá la clase BuscaMinas que controlan la lógica del juego. 

![image.png](./image.png)


- La clase InterfaceConsola puedes hacerla sencillita para no gastar tiempo con la E/S. Si te apetece hacerla compleja ¡no problem!
- En la clase BuscaMinas todo private excepto lo que se requiera expresamente public. 
- Hay que cumplir en la clase BuscaMinas el principio de ocultación tanto para tipos primitivos como para referencias.
- Generar javadoc para la clase BuscaMinas de forma que leyendo la ayuda de los métodos públicos otro programador que quiera hacer otra Interface, pueda manejar tu clase sin necesidad de leer el código java de tu clase. Esfuérzate en diseñar una parte pública compresible para otros. Recuerda que casi siempre "se escribe el código para otros".
- El proyecto, además de por supuesto el código fuente, contiene  también un jar ejecutable 

## Algunas ideas para escribir las clase BuscaMinas


- Utilizar dos matrices paralelas. Una almacena de cada casilla un número de 0-9 y la otra almacena de cada casilla si está destapada o no. La posibilidad de marcar una casilla como sospechosa de mina (la banderita del juego gráfico) puedes olvidarte de ella para simplificar tu código. No es obligatorio en absoluto que uséis matrices paralelas. Hay otros enfoques, por ejemplo usar una única matriz donde cada elemento sea de la clase Celda que será un objeto con dos campos, uno para almacenar valor y otro estado(tapado/destapado). Y hay muchos otros enfoques. Pero dicho esto, trabajar con dos matrices paralelas está bien.

- cómo calcular las adyacencias. Repasa los boletínes de arrays multidimensionales si no recuerdas o no dominas el concepto.

- destapar una casilla con valor 0 =>hacer un destapado recursivo. Si una celda vale 0 entonces tengo que ir mirando “alrededor” si puedo destapar sus posibles 8 vecinas.
- avanza progresivamente. Primero tienes que estar seguro que genera bien el tablero inicial con las minas, luego puedes empezar a programar el juego comprobando que destapa correctamente, funciona y termina el juego correctamente, añadimos la posibilidad de marcar una celda como sospechosa de mina, ...
- aplica todo lo que aprendiste con la tarea de SieteYMedia para estar seguro que separas la capa de presentación de los datos de la capa de la lógica del juego
- comprueba que cumple el principio de ocultación.
