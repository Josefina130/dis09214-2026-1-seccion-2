# sesión 09 - 05/06 Apuntes
---
## ESTADO Y CÁMARA WEB  
*¿Cómo crear sketch con estados diferentes?*  

#### Paso 1:  
**Crear y definir variable de estados**, al principio tu codigo debe crear variables que guarden la pantalla en la que estamos.  
*let estado = 0; // 0 = Inicio, 1 = Experiencia, 2 = Final*  

#### Paso 2:(function setup)  
**Creamos un lienzo**  
*function setup(){  
createCanvas(400,400);  
textAlign (CENTER,CENTER);  
textSize(24);*  

#### Paso 3:  
Crea la estructura del estado. **(function draw)**  
*Aquí usamos un switch dependiendo del valor de la variable estado, el programa dibujará una cosa u otra.*  

#### Paso 4:  
Crea la estructura del estado (funciones propias)  
*Ahora creamos las funciones que inventamos en el paso anterior. Cada una tendrá un diseño y un color diferente para que se note el cambio.*
Programar visualmente cada estado **(funciones propias)**   

#### Paso 5:   
La logica del cambio y el reinicio
*Para pasar de un estado a otro y lograr que vuelva al comienzo usamos la función *mousepressed* cada vez que haga clic la variable aumentara si llega a 3 después del estado 2 volverá a 0.*  


### Hay muchas formas de cambiar de un estado a otro  

1. ***Interacción con el teclado:***
- Por barra espaciadora o enter:
- Por teclas específicas (ej. Números): Puedes hacer que la tecla 1 te lleve al inicio, la 2 a la experiencia y la 3 al final.

2. ****Botón real en la pantalla:***
- En lugar de hacer clic en cualquier parte de la pantalla, puedes crear un botón real de *HTML* usando la *librería de p5.js*. *Esto es mucho más profesional para menús.*

3. ***Zona de clic (Botones dibujados con rect o ellipse):***
- Si no quieres usar botones de *HTML* y prefieres dibujar tus propios botones con rect(), puedes evaluar si el *mouse estaba dentro de esa caja al hacer clic.*

4. ***Interacciones automaticas (Por tiempo):***
-Por Tiempo (Temporizador): Ideal para una pantalla de introducción *(Splash Screen)* que dura 3 segundos y pasa sola al menú.

### CÁMARA WEB:  
**createCapture(VIDEO);**  
1. Crear la variable para la captura, declarar una variable global que guardará el flujo de video de tu cámara web.
   
2. Inicializar la cámara en el function *setup()* utilizamos el comando especial *createCapture(VIDEO)* esto le pedirá permiso al navegador para encender la cámara del computador. También definimos tamaño con
*captura.size(x,y);* y es muy importante agregar *captura.hide();* para que esconda el video que HTML pone abajo por default.

3. Dibujar la cámara en el function *draw()* usamos la función *image()*. p5.js toma cada cuadro *(frame)* de la cámara y lo dibuja en el lienzo en tiempo real.


