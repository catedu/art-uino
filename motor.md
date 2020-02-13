#MOTOR

![](/assets/2020-02-13 19_52_49-Window.png)
###Conexiones
Si quereis usar un motor, no se puede conectar diréctamente al Arduino, necesita el LM298N y las pilas.

![](https://www.luisllamas.es/wp-content/uploads/2016/05/arduino-l298n-conexion.png)

CC-BY-NC [Luis Llamas](https://www.luisllamas.es/arduino-motor-corriente-continua-l298n/)

Aunque se puede usar dos motores, nosotros sólo vamos a usar el Motor A, D6, D7 y D8 con estas conexiones:

* Motor A al motor
* Vm al Vin del ARDUINO
* GND al GND del ARDUINO
* ENA al D6 **OJO SON DOS PINES** quitaremos el jumper y conectaremos los dos al D6 para ello usaremos la Protoboard
* IN1 al D7
* IN2 al D8

También usaremos el [LedRGB con las mismas conexiones que se usaron en esta página](/led-rgb.md) para visualizar el giro

![](/assets/2020-02-13 20_00_05-Window.jpg)

###Programamos

El funcionamiento es muy sencillo:

* D6=high D7=high D8=low giro en un sentido
* D6=high D7=low D8=high giro en el otro sentido
* D6=low stop

Pondremos los pines 12 y 13 en algo en un sentido y en otro para visualizar el giro en el LED RGB:

![](/assets/2020-02-13 20_03_27-Window.png)

###Jugamos

Pulsamos la tecla ← o la tecla → para funcionar el motor, paramos con la tecla espacio




