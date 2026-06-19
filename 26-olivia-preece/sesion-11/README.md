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

### * Paso 4.  
Incluir un factor de referencia  
referencia = min(width, height)  
Creamos una varable global (referencia) y la asignamos para que calcule el mínimo. Observa el ancho y el alto de la ventana, los compara, y se queda solo con el que sea más pequeño en ese momento.

### * Paso 5.   
Usar translate - push y pop  
Consejo para proyectos complejos  
En lugar de hacer matemáticas complejas en cada rect() o ellipse (), usamos translate() para "mover el origen del mundo" y siempre utilizando push() y pop() para cada figura o elemento. 

### DESAFÍO DE CLASE  
Bandera de chile diseño responsivo LO LOGRE YUJU

## Agregar Imágenes loadImage()  
### * Paso 1 Subir la imagen a p5  
Hacer clic en la pequeña flecha hacia la derecha(>) ubicada en la esquina superior izquierda del editor (debajo del botón de play). Esto aabre el menú de archivos laterales. Hacer clic en el ícono de + o el menú desplegable junto a Files. Seleccionar Upload file (Subir archivo). Arrastrar la imagen o buscarla en el computador. Recomendación: usar nombres de archivos cortos y con mínusculas y sin espacios. Hacer una carpeta llamada ASSETS.



