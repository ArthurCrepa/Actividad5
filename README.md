#ACTIVIDAD5
---
---

En el presente repositorio se ha agregado el código fuente de "memory" 
Recuperado de: https://grantjenks.com/docs/freegames/memory.html . En el código original, debemos de completar seleccionar dos cuadras los cuales tengan el mismo valor numérico, si estos número coinciden revelarán parte de una imagen, se debe de repetir este proceso hasta haber revelado toda la imagen. Este juego se basa en la memoria del usuario 

Se nos ha pedido realizar lo siguiente:

1)Contar y desplegar el número de taps
-
2)Detectar cuando todos los cuadros se han destapado
-
3)Central el dígito en el cuadro
-
4)Como un condimento de innovación al juego, Podrías utilizar algo diferente a los dígitos para resolver el juego y que al usuario le ayude a tener mejor memoria ?
-

Explicaciones
***


*Primer Caso:* Primero, necesitábamos implementar un contador de las veces que presionamos un cuadro, siendo registrado bajo el nombre de *tabs*. Este registro de tabs aumenta únicamente si está dentro de los cuadros, si alguno de estos ya estaba resuelto ( ya se visualiza la imagen ) tabs no registrará este mismo. Así mismo, se nos pidió poder visualizar la cantidad de veces que presionamos este dentro la ventana de juego, más no dentro del mismo tablero. Usamos write para poder escribir Tabs en la ventana y fue ajustada para ser visualizada (pues si lo dejábamos sin modificaciones este estaría detrás del tablero).

*Segundo Caso:* Para verificar que el juego esté completo, el programa realizado se asegura de contar cuántos cuadros siguen escondidos, si no hay ninguno este terminará y anunciará que has terminado.

*Tercer Caso:* La función square() dibuja los cuadros y la función draw() se encarga de centrar las letras o números dentro de estos cuadros. Para lograr esto, se utilizan las funciones xy() y goto() para colocar el texto en las coordenadas exactas dentro de cada cuadro. Se añade un ajuste de posición con goto(x + 25, y + 8) para que las letras o números queden centrados vertical y horizontalmente en el cuadro.

*Cuarto Caso:* 
En lugar de usar solo dígitos, el código introduce letras del alfabeto en la lista tiles, que contiene tanto letras como números. Esto incrementa el desafío para la memoria del usuario, ya que debe recordar combinaciones de letras y números. La función tap() gestiona los toques y, si dos baldosas coinciden, se revela la letra o número correspondiente. Este cambio añade un elemento nuevo al juego, mejorando la capacidad de retención del jugador al introducir un conjunto más variado de símbolos.
