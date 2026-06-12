# sesión 06 - 12/06

## Diseño Responsivo  
(windowResized)

## ¿como crear skeych que se adepte a diferentes estados de pantalla?

### * Paso 1.  
Crear un canva con dimensiones dinámicas  
Para esto usaremos las variables integradas en el sistema: (windowWidth y WindowHeight) estas variables leen constantemente el ancho y alto disponible de la ventana del navegador.

### * Paso 2.  
Crear un evento windowResized()  
Si el usuario estira o encoge la ventana del navegador, el lienzo se adaptará al tamaño de la ventana en tiempo real.

### * Paso 3.  
Usar valores relativos  
Ahora p5.js actualiza estas variables width y height automaticamente con el tamaño actual del lienzo. Entonces ahora todos los valores de posición y tamaño que ocupames los tenemos que pensar en relación proporcional a esas variables.  
Usaremos fracciones y proporciones  
Ej: Caentro del lienzo( width/2 y heigth/2)  
Ej: A un cuarto de pantalla en eje x: (width * 0,25)

