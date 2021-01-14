#BUZZER ACTIVO

![](https://catedu.github.io/domotica-con-arduino/assets/buzzer.jpg)

La diferencia con el pasivo es que no es necesario enviarle pulsos para que emita una frecuencia, sólo tenemos que dar la orden y él reproduce un tono.

###Conexión

* GND a GND y VCC a 5V (ojo que están a los dos extremos, marcados en rojo y en negro)
* OUT a un pin digital, por ejemplo D13

![](/assets/2020-02-06 12_53_57.jpg)

###Programación

Ojo que funciona con lógica negativa es decir:

* si queremos que suene tenemos que enviar un LOW.
* si queremos que no suene tenemos que enviar un HIGH

![](/assets/2020-02-06 12_55_54.jpg)

###Jugamos
Pulsamos la tecla espacio y ... PIIIIT



