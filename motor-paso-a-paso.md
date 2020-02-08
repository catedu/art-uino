#MOTOR PASO A PASO

Igual que el [electroimán](/electroiman.md), necesitamos un controlador que nos de la potencia necesaria para mover el motor, el ULN2003

![](/assets/2020-02-08 17_14_42-Window.png)

Imagen BY-NC-SA de [Luis Llamas](https://www.luisllamas.es/motor-paso-paso-28byj-48-arduino-driver-uln2003/)

También igual que el electroimán, necesitamos una potencia extra con las pilas:

![](/assets/2020-02-08 17_20_14-Window.png)

###Conexión

* Cuatro pines digitales del ARDUINO al IN1,IN2,IN3,IN4 del ULN2003 por ejemplo D10,D11,D12,D13
* El conector blanco del ULN2003 al motor paso a paso
* El (+) del ULN2003 al Vin del ARDUINO
* El (-) del ULN2003 al GND del ARDUINO 

![](/assets/2020-02-08 17_28_05-Window.png)

### Programación TEORIA

Utilizaremos la configuración sencilla en fase1 es decir:

![](https://www.luisllamas.es/wp-content/uploads/2016/08/arduino-motor-paso-paso-secuencia-1-fase.png)

Imagen BY-NC-SA de [Luis Llamas](https://www.luisllamas.es/motor-paso-paso-28byj-48-arduino-driver-uln2003/)

Es decir:

| Paso    | IN1=D10 | IN2=D11 |IN3=D12 |IN4=D13 |
|---------|---------|---------|--------|--------|
| Paso 1  | ON      | OFF     |OFF     |OFF     |
| Paso 2  | OFF     | ON      |OFF     |OFF     |
| Paso 2  | OFF     | OFF     |ON      |OFF     |
| Paso 2  | OFF     | OFF     |OFF     |ON      |

### Programación CON MBLOCK DEPENDIENDO DEL ORDENADOR

Si lo hacemos como siempre, por ejemplo con este programa

![](/assets/2020-02-08 17_39_27-Window.png)

>VERAS QUE VA MUUUUUUY LENTO 

¿Por qué? porque tiene que comunicarse con el ordenador constantemente

### Programación CON MBLOCK INDEPENDIENTE DEL ORDENADOR

En este caso sustituimos la bandera por este símbolo

![](/assets/2020-02-08 17_41_38-Window.png)

Entramos en Edición - vista arduino y pulsamos UPLOAD TO ARDUINO

![](/assets/2020-02-08 17_43_18-Window.png)

Esperamos un rato y ... TACHÁN !!! **VA MÁS RÁPIDO**

>OJO, AHORA EL ARDUINO PASA OLIMPICAMENTE DE MBLOCK para volverlo a su estado, repite las diapositivas 5-6-7 de la [página mBlock](/chapter1.md)

###+INFO

https://www.luisllamas.es/motor-paso-paso-28byj-48-arduino-driver-uln2003/
















