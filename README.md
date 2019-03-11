# Taller de interacción

## Propósito

Estudiar las tres tareas universales de interacción en entornos virtuales.

## Tareas

Escoja una de las siguientes tres:

1. Emplee un [dispositivo de interfaz humana](https://en.wikipedia.org/wiki/Human_interface_device) no convencional para controlar una escena. Refiérase al ejemplo [SpaceNavigator](https://github.com/VisualComputing/frames/tree/master/examples/basics/SpaceNavigator). Se puede emplear la escena del [punto 2 del taller de transformaciones](https://github.com/VisualComputing/Transformations_ws)
2. Implemente una aplicación de _cámara en tercera persona_. Refiérase al ejemplo [FlockOfBoids](https://github.com/VisualComputing/frames/tree/master/examples/demos/FlockOfBoids).
3. Implemente una aplicación de _control de la aplicación_ (e.g., ["marking menus"](https://www.youtube.com/watch?v=twR_yxuHw24) o [vistas auxiliares](https://www.youtube.com/watch?v=Kr6-_NT_olo&feature=youtu.be&t=214)).

En cualquier caso se puede emplear la librería [frames](https://github.com/VisualComputing/frames) y/o cualquier otra.

## Integrantes

Máximo tres.

Complete la tabla:

| Integrante | github nick |
|------------|-------------|
|  Juan David Saab          |   juansaab          |


## Informe

Se realizó la propuesta número 1. Controlar una escena usando un HID no convencional.

Para la realización de este taller se tuvo en cuenta un modelo de interacción con un ojo observador de escena. El sistema de coordenadas del ojo se traslada para transmitir la sensación de control de la aplicación. La aplicación fue desarrollada utilizando P5.js y como sistema de interfaz humana se empleó la cámara, con un algoritmo de detección de emociones desarrollado por @auduno [clmtrackr](https://github.com/auduno/clmtrackr).

El desarrollo del taller incluyó las siguientes etapas:

1. Definición de una escena sencilla compuesta por dos cajas con textura, ubicadas en un espacio tridimensional.
2. Definición de un objeto "eye" (cámara), haciendo uso de la librería p5EasyCam.
3. Definición de funciones de interacción para realizar movimientos a la cámara bajo dos acciones específicas.
4. Modificación de librería de detección de emociones con webcam, para usarla como interfaz de control de la aplicación.

Para ejecutar el programa, es necesario correr un servidor local.

Esto puede realizarse con la librería SimpleHTTPServer de Python
```python -m SimpleHTTPServer 8000```

Un ejemplo del código corriendo se puede apreciar en el siguiente GIF.

![](interaction.gif)


## Entrega

Fecha límite Domingo 10/3/19 a las 24h.
