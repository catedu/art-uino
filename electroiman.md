#ELECTROIMÁN O SOLENOIDE

El electroimán no se puede conectar diréctamente, utilizaremos un transistor el [IRF520N](https://www.luisllamas.es/arduino-transistor-mosfet/) que amplifique la señal del Arduino, pues no tiene potencia para mover el electroimán

Para dar esa potencia utilizaremos otra fuente externa, unas pilas:

![](/assets/2020-02-08 17_00_58-Window.png)

###Conexiones

* SIG del IRF520N a una salida digital por ejemplo D13
* VCC del IRF5020N al 5V del ARDUINO
* Los dos GND del IRF520N a GND del ARDUINO
* V+ y V- del IRF5020N al solenoide (da igual el orden)
* VIN del IRF520N al VIN del ARDUINO (son los voltios de la pilas)

![](/assets/2020-02-08 17_08_36-Window.png)

###Programamos

![](/assets/2020-02-08 17_09_32-Window.png)

### Jugamos

Pulsamos la tecla espacio ¿qué ocurre?


