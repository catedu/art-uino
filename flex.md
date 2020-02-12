#RESISTENCIA FLEX
Es una resistencia que cuanto más se dobla más resistencia ofrece, desde 25k hasta 125k

[![Datasheet Sparkfun](/assets/2020-02-12 12_13_26.jpg)](https://www.sparkfun.com/datasheets/Sensors/Flex/flex22.pdf)

###Conectamos

Para utilizar esta resistencia haremos un **[DIVISOR DE TENSIÓN](https://es.wikipedia.org/wiki/Divisor_de_tensi%C3%B3n)** que consistirá en poner dos resistencias en serie y repartirá la tensión total entre 0V y 5V en las dos resistencias, **el punto medio** será un punto que tendrá una tensión variable en función de las dos resistencias, como la FLEX es variable, esa tensión es variable y ya tenemos la entrada **analógica**:

![](/assets/2020-02-12 12_24_30.jpg)

Es decir:

* La resistencia FLEX entre masa GND del ARDUINO (cable negro) y un punto en la placa protoboard
* ese punto medio conectarlo a una entrada analógica, por ejemplo A0 (cable amarillo)
* Una resistencia de valor parecida a la Flex de decenas de K entre ese punto y +5V (cable rojo en la foto)

![](/assets/2020-02-12 12_25_13.jpg)

###Programamos

![](/assets/2020-02-12 12_10_01.jpg)

###Jugamos

Si doblamos la FLEX el oso nos da distintos valores, para una resistencia de 47k tenemos sin doblar :

![](/assets/2020-02-12 12_09_31.jpg)

Y totalmente doblado (90º)

![](/assets/2020-02-12 12_09_52.jpg)


