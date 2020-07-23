## Informe

### 1. PLANTEAMIENTO DEL PROBLEMA

En la rama de los circuitos digitales se emplean operaciones aritméticas binarias en el diseño de diversos circuitos, entre estas operaciones se encuentra la suma. Si bien se conoce que existen compuertas lógicas que permiten realizar este proceso como es el caso del circuito integrado 74LS32 que posee cuatro compuertas en su estructura, existen otros integrados que realizan la misma operación y se denominan sumadores.

Cuando se utilizan compuertas lógicas OR (suma) se tiene un número limitado de variables de entrada puesto que si se desea trabajar con un número elevado de estas variables, el proceso de obtención de las funciones lógicas resultantes y la implementación del diseño van a complicarse debido al elevado número de circuitos integrados que se utilizarán y por consecuencia no habrá una optimización de diseño y su construcción será más costosa.

Para esta limitante se emplean los circuitos integrados sumadores; un solo integrado de este tipo realiza la suma de hasta 8 variables de entrada (dos números 4 bits) lo cual facilita el diseño, interpretación, optimización e implementación.

En base los puntos planteados se pretende implementar un circuito sumador de dos números de 8 bits (16 variables de entrada) utilizando un circuito integrado sumador: LS74283 y visualizar su resultado en displays de 7 segmentos.

### 2. OBJETIVOS

**General**

* Diseñar simular e implementar un circuito que permita la suma de dos números, cada uno con 8 bits el resultado debe mostrarse en displays de 7 segmentos,en Thinkercad  con la utilización de los integrados 74283 y 4511.

**Específicos**

* Analizar el circuito a diseñar para obtener un resuel funcionamiento de cada integrado para el diseño del circuito sumador de dos números de  
Utilizar la plataforma Thinkercad para la implementación del circuito


### 3. ESTADO DEL ARTE

**Diseño e implementación de sumadores de 32 bits utilizando varios sumadores completos**

En este articulo se diseñan sumadores de 32 bits, Ripple Carry Adder (RCA), Carry Increment adder (CINA) y Carry bypass adder (CBYA) para realizar un sumador completo utilizando Verilog HDL. Los resultados se obtienen ejecutando el código Verilog en Xilinx 14.5 ISE para el dispositivo de la familia Spartan 3E con velocidad de grado -5.

**Autores:**

•	K. Anirudh Kumar Maurya
ECE Department, SRKR Enigineering College, Bhimavaram, India
•	Y. Rama Lakshmanna
ECE Department, SRKR Enigineering College, Bhimavaram, India
•	K. Bala Sindhuri
ECE Department, SRKR Engineering College, Bhimavaram, India
•	N. Udaya Kumar
ECE Department, SRKR Enigineering College, Bhimavaram, India

**Fecha y lugar de publicación:**
Fecha: 21-22 April 2017 en la conferencia Innovaciones 2017 en energía y tecnologías de computación avanzadas (i-PACT)
Este artículo guarda relación con el trabajo de investigación, ya que realiza la suma de 32 bits que es la misma cantidad de bits con los que estamos trabajando sin embargo son diferentes ya que utilizan otro tipo de sumadores y los resultados mostrados también son mostrados de diferente forma.


### 4. MARCO TEÓRICO

**Circuitos Aritméticos**

Dentro de la variada gama de circuitos digitales, tenemos los denominados circuitos aritméticos que son dispositivos que pueden realizar operaciones aritméticas (suma, 
resta, multiplicación y división) en formato binario o BCD, punto fijo o punto flotante. 

Dependiendo de la función a realizar, tenemos sumadores, restadores, multiplicadores, divisores y funciones combinadas de los mismos para realizar operaciones complejas como por 
ejemplo el cálculo de raíz cuadrada, exponenciales, etc.

Si bien es posible generar funciones complejas en base al uso de un microprocesador, a través de algoritmos que se corren en un programa, la posibilidad de generar dichas 
funciones en hardware, en muchos casos, presentan ventajas en cuanto a velocidad y/o el empleo de menores recursos lógicos, como es el caso de la ausencia de un micro para realizarlas (Hoyos Padilla, 2010).

**Sumadores**

La suma o adición binaria es análoga a la de los números decimales. La diferencia radica en que en los números binarios se produce un acarreo (carry) cuando la suma excede de uno mientras en decimal se produce un acarreo cuando la suma excede de nueve (Hoyos Padilla, 2010).

![jf1](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf1.jpg)

la figura muestra las reglas que debemos seguir cuando realizamos las operaciones de suma binaria.

**Semisumador**

Se denomina semisumador a un circuito que admite dos bits como entrada y genera  como salida  un bit que representa la suma de los dos bits de entrada y otro bit que representa 
el acarreo generado por la suma.

La tabla de verdad de este circuito puede deducirse a partir de las La tabla de verdad de este circuito puede deducirse a partir de las reglas de la suma binaria (Véase Fig. ).

![jf2](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf2.png)

A partir de esta tabla de verdad se puede observar que la suma puede implementarse con una operación XOR y el acarreo de salida con una operación AND(Canaria, 2012).

![jf3](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf3.png)

**Sumador Completo**

La principal diferencia diferencia entre un sumador completo y un semisumador es que el sumador completo admite un valor que representa un acarreo de entrada.

![jf4](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf4.png)

Dado que la suma de dos bits está dada la operación XOR, también podemos expresar dicha suma  con un acarreo de la siguiente forma:

![jf5](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf5.png)

El acarreo de salida sera 1 entonces cuando A y B sean 1 o cuando A+B sea 1 al igual que el acarreo de entrada.

![jf6](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf6.png)

De esta forma se puede implementar el circuito sumador completo usando dos compuertas XOR, dos compuestas AND y una compuerta OR.

![jf7](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf7.png)

También es posible implementar el sumador completo utilizando dos circuitos semisumadores, el primer semisumador suma los dos bits, el segundo suma el resultado con el acarreo 
de entrada y habrá acarreo de salida si cualquiera  de los dos semisumadores genera un acarreo.

![jf8](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf8.png)

**Sumadores con Acarreo en Cascada**

El circuito sumador completo permite sumar dos números de un bit con un acarreo de entrada y generar un acarreo de salida. Como regla general, un sumador binario de cualquier número de bits puede realizarse conectando en cascada varios sumadores completos de un bit.

El proceso puede extenderse usando cuaquier sumador como elemento básico: por ejemplo puede hacerse un suamdor de 4 bits a partir de dos sumadores de 2 bits.

![jf9](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf9.png)

El principal problema de esta conexión en serie de sumadores es que el retardo del circuito depende de la propagación del acarreo a lo largo de todo el sumador.

![jf10](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf10.png)

Para la implementación del sumador de 8 bits se dio uso al integrado 74283

![jf11](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf11.jpg)


5. DIAGRAMAS

5.1. Diagrama de Bloques

5.2. Diagramas electrónicos 

6. LISTA DE COMPONENTES

7. MAPA DE VARIABLES

8. EXPLICACIÓN DEL CÓDIGO FUENTE
* Para realizar el circuito sumador de dos números de 8 bits primero se definen las variables de entrada y salida que tendrá el circuito, todas se encuentran en lógica positiva y se presentan de la siguiente forma:

![Diagrama de bloques: Sumador 8 Bits](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/ENTRADAS.png)

**Entradas**

**Número A**: A7, A6, A5, A4, A3, A2, A1, A0
Donde: A0 es el bit menos significativo y A7 es el más significativo

**Número B**: B7, B6, B5, B4, B3, B2, B1, B0
Donde: B0 es el bit menos significativo y B7 es el más significativo

![Entradas en DIPSW](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DIPSENTRADAS.PNG)

**Salidas**
S8, S7, S6, S5, S4, S3, S2, S1, S0
Donde: S0 es el bit menos significativo y S8 (acarreo) es el más significativo.

![Salidas del Sumador](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SALIDAS1.PNG)

* Para realizar el proceso de la suma binaria se utiliza el circuito integrado 74LS283 que cumple la función de sumador.

![Sumador LS74283](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SUM.png)

Donde A0 - A3 representan los cuatro primeros bits del número A y B0 - B3 del número B, sin embargo, los números de las entradas son de 8 Bits de magnitud entonces para realizar la suma se necesita realizar una conexión en cascada entre dos sumadores.

Para que se cumpla el proceso se debe conocer las reglas de la suma binaria:
![Reglas de la suma binaria](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/REGLASUMA.PNG)

El integrado 74LS283 tiene dos pines que representan el acarreo de entrada y salida, entonces para realizar la conexión en cascada: el acarreo de salida del primer sumador es el acarreo de entrada del segundo, por lo tanto, ambos se encuentran conectados y en las entradas del integrado se colocan las cuatro variables restantes de los números A y B, las cuales son: A4 - A7 y B4 - B7 identificando la conexión de los bits más y menos significativos.

![Conexión en cascada](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SUMCASCADA.png)

 * Las salidas de los sumadores representan el resultado de la suma realizada por el circuito integrado y se encuentran conectadas a unos LEDS, de tal forma que cuando el LED se enciende, representa un 1 y cuando se apaga representa un 0.
Donde:
S0=A0+B0
S1=A1+B1
S2=A2+B2
S3=A3+B3
S4=A4+B4
S5=A5+B5
S6=A6+B6
S7=A7+BB7
S8=Acarreo de salida del segundo sumador

![Resultado de la suma binaria representado con LEDS](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SALIDAS.PNG)

* Para visualizar este resultado en un display de 7 segmentos se utiliza el decodificador 4511 conectado a las salidas de cada sumador y a su vez a las entradas del display junto con resistencias para evitar que el dispositivo sufra daños.

![Decodificador 4511](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DECODIFICADOR.PNG)

* Para conectar el display se debe tomar en cuenta la estructura que posee, para este circuito se usa un display 7 segmentos cátodo común. Esto quiere decir que el pin común del display debe ir conectado a tierra:

![Display 7 seg catodo común](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DISPLAY.PNG)

* Hay que tomar en cuenta que para los displays de 7 segmentos el número más alto que se puede visualizar es el nueve, por lo tanto cuando el resultado de la suma implique un número mayor al indicado, no se va a encender el display:

![Display encendido](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DISPLAYENCENDIDO.png)
![Display apagado](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DISPLAYAPAGADO.png)

* El resultado se todos estos procesos da un circuito sumador de dos números de 8 bits como se muestra a continuación en el software de simulación Proteus:

![Simulación Proteus](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SimulacionProteus.png)

* La implementación del circuito en el laboratorio virtual Tinkercad se presenta de la siguiente forma:

![Simulación Tinkercad](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SimulacionTinkercad.png)

9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

10. APORTACIONES

11. CONCLUSIONES

12. RECOMENDACIONES

13. CRONOGRAMA

14. BIBLIOGRAFÍA

https://wilaebaelectronica.blogspot.com/2017/01/sumador-binario.html

https://iesbernatguinovart.com/04v_tecnologia/carpeta_arxius/elec%20dig%20basica.pdf

https://www.studocu.com/pe/document/universidad-nacional-del-callao/circuitos-digitales-turno-01t-ciclo-5/informe/circuitos-aritmeticos/5637738/view

http://homepage.cem.itesm.mx/garcia.andres/PDF201411/Aritmetica(Basis).pdf

http://circuitos-aritmeticos.blogspot.com/

http://serdis.dis.ulpgc.es/~gii-fc/material_clases_teoria/Tema3/Tema3_1_Componentes_combinacionales_FC_GII.pdf

15. ANEXOS

15.1.  MANUAL DE USUARIO

15.2.  HOJAS TÉCNICAS



