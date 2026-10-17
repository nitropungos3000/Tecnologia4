<p align="center">
<img src="Imágenes/Teleco games.jpg" width="300" height="300" />
</p>

# Teleco Games

Bienvenidos al proyecto número 4 llamado Teleco Games. En esta ocasión, vamos a 

## 1ª parte del proyecto: Desarrollo individual de una idea inicial

En esta primera parte del proyecto, vamos a seguir los pasos del primero. Primero vamos a desarrollar una idea primeriza que nos ayudará a situarnos en el tema. Posteriormente, nos juntaremos en parejas con la misma persona que en el proyecto 1. Y, finalmente, nos juntaremos en gran grupo para decidir una idea que posteriormente pondremos en marcha para los Teleco Games.

En mi ocasión, he utilizado la IA de Google, Gemini, para que me aporte una lluvia de ideas con la que poder comenzar. Me ha comentado varias opciones, tales como una papelera inteligente, que detecte cuando está llena o vacía y te avisa por una nontificación en el teléfono o un chat bot en la app Telegram; también un sistema de riego, utilizando bombas de agua con temporizador controladas por una placa bien sea Arduino, ESP32, Raspberry Pi y demás; y por la que finalmente me he dacantado como inicio, una caseta inteligente para pájaros, pricipalmente.

### Desarrollo de la idea
Ahora que he mencionado mi idea paso a desarrollarlla. Los principales elementos que utilizaríamos serían los siguientes (los cuales explicaré cada uno): placa ESP32 o Arduino (preferiblemente ESP32 ya que cuenta con módulo Wi-FI y Bluetooth, crucial para el requisito de telecomunicaciones), servomotor, bomba de agua, impresora 3D, cortadora láser, placa solar en miniatura para la alimentación de componentes y placa, módulo de gestión de la carga de las placas solares y pilas para almacenar esa carga, sensor de ultrasonidos, sensor de infrarrojos, sensor de humedad, sensor de temperatura, contrachapado de madera y cables, además de un ordenador para diseñar y programar el código que vayamos a utilizar.

Lo primero que habría que hacer es pensar en qué zonas colocar estas casetas. Lo que he pensado, y lo que más lógica tiene, sería en la entrada de nuestro instituto, ya que colocarlo en parques dificultaría mucho el tema de la alimentación de los componentes, además del montaje de la misma caseta. La idea es montar la caseta con contrachapado de madera utilizando la cortadora láser, y posteriormente las cubiertas para los componentes eletrónicos (principalmente para que los pájaros que se encuentren dentro no puedan romper los componentes) imprimirlas en 3D, de las cuales ya se estudiaría el material con el que se imprimiría. 

Ahora, vamos a explicar un poco lo que va a hacer la placa. La placa ESP32, como pequeño resumen, es una tarjeta de desarrollo de bajo costo y consumo de energía muy utilizada en proyectos de Internet de las Cosas (IoT) y robótica. Es muy versátil y útil, y tiene el rol de ser el cerebro del proyecto. Tiene mucha potencia, consume muy poco, se le pueden conectar todo tipo de componentes electrónicos (a través de sus pines GPIO) y tiene conectividad Wi-Fi y Bluetooth. Esta placa va a controlar todos los componentes electrónicos (sensores, servomotor y bomba de agua), además de convertirse en el mensajero de información a nuestro teléfono utilizando principlamente la conectividad Wi-Fi, la cual tiene más alcance que el Bluetooth.


Ahora pasamos a la parte de explicación de las funciones de los componentes que vamos a utilizar en esta idea, empezando por el servomotor y la bomba de agua. Primero, el servomotor. Este se va a encargar de abrir y cerrar la compuerta del dispensador de comida para los pájaros. Va a estar controlado por la placa, obviamente, además de por los sensores de infrarrojos, para regular cuando colocar comida en la caseta para que el pájaro en cuestión se alimente. Segundo, la bomba de agua. Esta va estar conectada a un contenedor de agua, cuya función principal va a ser verter agua en un recipiente para que los pájaros puedan beber, regulada también por los infrarrojos y la placa. 

Después, tenemos a los sensores de infrarrojos, humedad, temperatura y ultrasonidos. Los sensores infrarrojos, sencillamente, van a enviar la señal a la placa de cuando entra o sale un pájaro. Solo se va a encargar de eso. Despiués, los sensores de teperatura y humedad se van a encargar de comprobar la calidad del interior de la caseta, para conocer si está en unas buenas condiciones para que los pájaros se encuentren dentro. Y, los ultrasonidos, van a detectar la cantidad de comida que tiene el depoósito a través de la distancia. Si detecta que la distancia que hay entre el principio y el fin del contenedor es considerable, entonces se envía una señal para recordar que el contenedor se debe rellenar.  
