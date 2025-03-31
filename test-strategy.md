#Plan de Ataque 

## Descripcion de errores encontraodos y Souciones
A continuacion se muestra la lista de los errores encontrados en el programa TEST-QA-BANRURAL

## 1
### Error
Me percato que el addEventListener esta mal escrito ya que genera errores al pulsar el boton ya que no realiza una accion.

### Solucion
Se modifica el addeventListener a addEventListener en la linea 87 y 95.

## 2
### Error 
El programa indica que son 10 intentos para adivinar el numero de 1 a 100.

### Solucion
Se modifica la constante de ATTEMPS de 5 a 10.

## 3
### Error
Se encuentra que en el Form el input guessField, esta en tipo "text".

### Solucion 
Se modifica el input guessField de "text" a "number".

## 4
### Error
Se encuentra que el selector lowOrHi tiene error de sintaxis.

### Solucion
Se modifica el selector lowOrHi a .lowOrHi.

## 5
### Error
El numero aleatorio se generaba con Math.random()*10 lo que generaba numero de 0 a 9.

### Solucion
Se modifico a (Math.random() * 100) + 1 para que genere los numeros de 0 a 100 en la linea 44 y 114.

## 6
### Error
Se encontro un error cuando muestra los mensajes de felicitaciones e incorrecto, ya que felicitaciones lo muestra en color rojo y el de incorrecto lo muestra en color verde.

### Solucion 
Se modifican las linea de codigo 71 de 'red' a 'green' y la linea 75 de 'green' a 'red'.

## 7
### Error
Cuando el usuario realiza 5 intentos, el juego finaliza con el mensaje "¡Pérdistes!", a pesar de que no debería terminarse hasta que el usuario haya realizado 10 intentos o haya adivinado correctamente el número.

### Solucion
Se corrigió la condición en el bloque `else if` que evalúa cuando el número de intentos ha alcanzado el límite (`ATTEMPS`). Ahora, el juego finalizará correctamente después de 10 intentos o cuando el usuario adivine el número. Además, se corrigió el mensaje para que aparezca cuando el usuario haya agotado los intentos.

## 8
### Error
El juego permite ingresar numeros decimales y mayores a 100

### Solucion
Se hace una validacion para que nos aseguremos que los numeros sean enteros y no mayores a 100 de la linea 60 a 65.