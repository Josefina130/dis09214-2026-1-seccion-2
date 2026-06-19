# sesión 06 - 19/06

## SONIDO  
loadSound()  
### * Paso 1.
Subir archivos en formato .mp3 o .wav. Como recomendacion usar nombres de archivos cortos. Hacer una carpeta llamada ASSETS.

### * Paso 2.  
Declarar y precargar el sonido. dunction preload()  
Creamos ina variable global al inicio del código para guardar nuestro sonido. Usamos la función function preload() inicializamos nuestra variable y cargamos el sonido con loadSound()

### * Paso 3.  
Activar mi sonido.  
Le damos play al sonido en el function setup con: nombreVariable.play(); Con esta instrucción, el sonido va a comenzar cuando le damos play a a nuestro sketch.


## Métodos de control del sonido:
nombreVariable.play(); Reproduce el sonido una vez  
nombreVariable.loop(): Reptoduce el sonido en bucle infinito  
nombreVariable.stop(): Detiene el sonido por completo  
nombreVariable.pause(): Pausa el sonido en el segundo actual  

nombreVariable.setVolume(valor):  Modifica el volumen. Recibe un número entre 0.0 (silencio) y 1.0 (volumen máximo)   
nombreVariable.Rate

## Métodos de consulta o estados del sonido  
nombreVariable.isPlaying(): Devuelve true si el sonido está sonando en este momento y false si no. 
nombreVariable.isPaused(): Devuelve true si el sonifo fue congelado con puse()

### DESAFÍO CLASE  
radio  
play/pause
