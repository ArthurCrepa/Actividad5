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

*Tercer Caso:* 

*Cuarto Caso:* 
