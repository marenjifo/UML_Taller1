# UML_Taller1 Ecosistemas de aplicaciones


## UML Código en Eclipse

## Main: Clase main que ejecuta todo el juego

### Atributos
- **log: Logica** Se inicializa la variable de tipo Logica

### Métodos
- **main(String[]):void:** Método que ejecuta toda la aplicación
- **settings():void:** Define las dimensiones del lienzo
- **setup():void:** Se inicializan las variables necesarias para ejecutar la aplicación
- **draw():void:** Método donde se pinta toda la interfaz gráfica
- **mousePressed():void:** Ejecuta las acciones del mouse

## Logica: Clase Logica que contiene la interfaz gráfica de la aplicación

### Atributos
- **app: PApplet** Creacion objeto PApplet
- **pantalla: int** Entero para crear un switch que permita cambiar las pantallas de la aplicación
- **fondos: PImage** Imágenes de las pantallas de juego
- **puntPigg: int** Variable para guardar puntaje de Piggy
- **puntHom: int** Variable para guardar puntaje de Hombre

### Métodos
- **Logica(PApplet)** Constructor de la clase Logica que recibe un PApplet
- **pintar():void:** Pinta todos los elementos gráficos de la aplicación
- **interaccionPiggy():void:** Método que define todas las interacciones y condiciones del personaje Piggy
- **interaccionHombre():void:** Método que define todas las interacciones y condiciones del personaje Hombre
- **ejecutarMouse():void:** Método que contiene acciones del mouse que comienzan la aplicación

## Servidor: Clase servidor para establecer conexion con un cliente

### Atributos
- **ss: ServerSocket** Escucha y espera la conexión de un cliente
- **s: Socket** Acepta un ServerSocket cuando se ha establecido una conexion con el cliente

### Métodos
- **enviar () : void** Datos que se envían del servidor al cliente

## Receptor: Clase Receptor que recibe información del cliente

### Atributos
- **s: Socket** Recibe conexion para crear flujo de datos

### Métodos
- **Receptor(Socket) : void:** Constructor de la clase Receptor

## Thread: Clase para crear hilos
- **run() : void:** Método que ejecuta el hilo

## Personaje: Clase que genera los personajes del juego

### Atributos
- **app:PApplet** Creación de objeto PApplet
- **x,y: int** Posición del personaje
- **vel: int** Velocidad del personaje
- **vida: int** Número de vidas del personaje
- **img: PImage[]** Arreglo de imágenes del personaje

### Métodos
- **Personaje(PApplet,int,int)** Constructor de la clase Personaje que recibe un PApplet y dos int
- **pintar():void:** Pinta los elementos gráficos de los personajes
- **mover():void:** Método que del movimiento del personaje Piggy
- **getX():int:** Método para saber la posición X del objeto
- **getY():int:** Método para saber la posición Y del objeto
- **setX():void:** Método para definir la posición X del objeto
- **setY():void:** Método para definir la posición Y del objeto
- **getVel():int:** Método para saber la velocidad del objeto
- **setVel():void:** Método para definir la velocidad del objeto

## Piggy: Clase del personaje #1 Piggy que hereda de Personaje
- **Piggy(PApplet,int,int)** Constructor de la clase Piggy que recibe un PApplet y dos int
- **pintar():void:** Pinta el personaje Piggy

## Hombre: Clase del personaje#2 hombre que hereda de Personaje
- **Hombre(PApplet,int,int)** Constructor de la clase Hombre que recibe un PApplet y dos int
- **pintar():void:** Pinta el personaje Hombre

## Objeto: Clase que genera los recogibles del juego

### Atributos
- **app:PApplet** Creación de objeto PApplet
- **x,y: int** Posición del objeto
- **img: PImage[]** Arreglo de imágenes del objeto

### Métodos
- **Objeto(PApplet,int,int)** Constructor de la clase Objeto que recibe un PApplet y dos int
- **pintar():void:** Pinta los elementos gráficos de los objetos
- **mover():void:** Método que define el movimiento del personaje Hombre
- **getX():int:** Método para saber la posición X del objeto
- **getY():int:** Método para saber la posición Y del objeto
- **setX():void:** Método para definir la posición X del objeto
- **setY():void:** Método para definir la posición Y del objeto

## Manzana: Clase del objeto Manzana que hereda de Objeto
- **Manzana(PApplet,int,int)** Constructor de la clase Manzana que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Manzana

## Llave: Clase del objeto Llave que hereda de Objeto
- **Manzana(PApplet,int,int)** Constructor de la clase Llave que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Llave

## Concentrado: Clase del objeto Concentrado que hereda de Objeto
- **Concentrado(PApplet,int,int)** Constructor de la clase Concentrado que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Concentrado

## Carne: Clase del objeto Carne que hereda de Objeto
- **Carne(PApplet,int,int)** Constructor de la clase Carne que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Carne

## Bala: Clase del objeto Bala que hereda de Objeto
- **Bala(PApplet,int,int)** Constructor de la clase Bala que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Bala
- **mover():void:** Determina el movimiento del objeto Bala

## Tornillo: Clase del objeto Tornillo que hereda de Objeto
- **Tornillo(PApplet,int,int)** Constructor de la clase Tornillo que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Tornillo

## UML Código en Android

## Main: Clase ejecutable que da inicio a toda la aplicación

### Atributos
- **btn_up: ImageButton** Recibe la información cuando se oprime el botón de movimiento hacia arriba
- **btn_down: ImageButton** Recibe la información cuando se oprime el botón de movimiento hacia abajo
- **btn_right: ImageButton** Recibe la información cuando se oprime el botón de movimiento hacia la derecha
- **btn_left: ImageButton** Recibe la información cuando se oprime el botón de movimiento hacia la izquierda
- **btn_attack: ImageButton** Recibe la información cuando se oprime el botón de ataque del personaje
- **iv_puntos: ImageView** Imagen del logo de puntos
- **iv_perso: ImageView** Imagen del personaje en juego
- **tv_puntaje: textView** Texto con puntos del personaje

### Métodos
- **onCreate(Bundle):protected void** Método que ejecuta toda la aplicación

## Cliente: Permite conexión con el servidor

### Atributos
- **s: Socket** Sirve para establecer conexion con el servidor

### Métodos
- **Cliente(MainActivity)** Constructor de la clase Cliente que recibe un objeto MainActivity
- **enviar(): void** Método que envia datos al servidor

## Receptor: Recibe toda la información enviada por el servidor

### Atributos
- **s: Socket** Recibe conexion para crear flujo de datos

### Métodos
- **Receptor(Socket)** Constructor de la clase Receptor que recibe un objeto Socket

## Thread: Clase que permite crear hilos
- **run() : void:** Método que ejecuta el hilo

## Interface OnMessage: Genera un patrón observer para mostrar visualmente lo requerido a partir de lo enviado por el servidor
- **onReceived(String) : void:** Método que recibe el mensaje enviado por el servidor


