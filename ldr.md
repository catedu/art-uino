#SENSOR DE LUZ : RESISTENCIA LDR

El LDR es una resistencia que varía su valor con la luz, cuanto más OSCURO más grande es su valor, por lo tanto por la ley de Ohm este módulo nos da una señal analógica que aumenta con la oscuridad. 

![](https://catedu.gitbooks.io/domotica-con-arduino/content/assets/2019-03-07%2019_34_24-Window.jpg)

###Conexión

* VCC y GND a 5V y GND
* OUT a una salida digital cualquiera por ejemplo D13

#####Calibramos
Sin taparlo con un destornillador fino, movemos el potenciómetro (marcado en verde) **justo hasta que el segundo led se encienda** (marcado en amarillo)

![](/assets/2020-02-06 12_36_25.jpg)

###Programamos

Este no va al revés es decir si tapamos es un 1 y si no tapamos es un 0 luego:

![](/assets/2020-02-06 12_40_51.jpg)

###Jugamos

Si pongo la mano, el oso nos saluda, sino: está pensando :

![](/assets/2020-02-06 11_31_49.jpg)

