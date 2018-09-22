# UML_Taller1 Ecosistemas de aplicaciones


## UML Código en Eclipse

### Main
- **main(String[]):void:** Método que ejecuta toda la aplicación
- **settings():void:** Define las dimensiones del lienzo
- **setup():void:** Se inicializan las variables necesarias para ejecutar la aplicación
- **draw():void:** Método donde se pinta toda la interfaz gráfica
- **mousePressed():void:** Ejecuta las acciones del mouse

### Logica
- **Logica(PApplet)** Constructor de la clase Logica que recibe un PApplet
- **pintar():void:** Pinta todos los elementos gráficos de la aplicación
- **interaccionPiggy():void:** Método que define todas las interacciones y condiciones del personaje Piggy
- **interaccionHombre():void:** Método que define todas las interacciones y condiciones del personaje Hombre
- **ejecutarMouse():void:** Método que contiene acciones del mouse que comienzan la aplicación

### Servidor
- **enviar () : void** Datos que se envían del servidor al cliente

### Receptor
- **Receptor(Socket) : void:** Constructor de la clase Receptor

### Thread
- **run() : void:** Método que ejecuta el hilo

### Personaje
- **Personaje(PApplet,int,int)** Constructor de la clase Personaje que recibe un PApplet y dos int
- **pintar():void:** Pinta los elementos gráficos de los personajes
- **mover():void:** Método que del movimiento del personaje Piggy
- **getX():int:** Método para saber la posición X del objeto
- **getY():int:** Método para saber la posición Y del objeto
- **setX():void:** Método para definir la posición X del objeto
- **setY():void:** Método para definir la posición Y del objeto
- **getVel():int:** Método para saber la velocidad del objeto
- **setVel():void:** Método para definir la velocidad del objeto

### Piggy
- **Piggy(PApplet,int,int)** Constructor de la clase Piggy que recibe un PApplet y dos int
- **pintar():void:** Pinta el personaje Piggy

### Hombre
- **Hombre(PApplet,int,int)** Constructor de la clase Hombre que recibe un PApplet y dos int
- **pintar():void:** Pinta el personaje Hombre

### Objeto
- **Objeto(PApplet,int,int)** Constructor de la clase Objeto que recibe un PApplet y dos int
- **pintar():void:** Pinta los elementos gráficos de los objetos
- **mover():void:** Método que define el movimiento del personaje Hombre
- **getX():int:** Método para saber la posición X del objeto
- **getY():int:** Método para saber la posición Y del objeto
- **setX():void:** Método para definir la posición X del objeto
- **setY():void:** Método para definir la posición Y del objeto

### Manzana
- **Manzana(PApplet,int,int)** Constructor de la clase Manzana que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Manzana

### Llave
- **Manzana(PApplet,int,int)** Constructor de la clase Llave que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Llave

### Concentrado
- **Concentrado(PApplet,int,int)** Constructor de la clase Concentrado que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Concentrado

### Carne
- **Carne(PApplet,int,int)** Constructor de la clase Carne que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Carne

### Bala
- **Bala(PApplet,int,int)** Constructor de la clase Bala que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Bala
- **mover():void:** Determina el movimiento del objeto Bala

### Tornillo
- **Tornillo(PApplet,int,int)** Constructor de la clase Tornillo que recibe un PApplet y dos int
- **pintar():void:** Pinta el objeto Tornillo

## UML Código en Android

### Main
- **onCreate(Bundle):protected void** Método que ejecuta toda la aplicación

### Cliente
- **Cliente(MainActivity)** Constructor de la clase Cliente que recibe un objeto MainActivity
- **enviar(): void** Método que envia datos al servidor

### Receptor
- **Receptor(Socket)** Constructor de la clase Receptor que recibe un objeto Socket

### Thread
- **run() : void:** Método que ejecuta el hilo

### Interface OnMessage
- **onReceived(String) : void:** Método que recibe el mensaje enviado por el servidor


