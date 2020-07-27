## Informe

### 1. PLANTEAMIENTO DEL PROBLEMA

En la rama de los circuitos digitales se emplean operaciones aritméticas binarias en el diseño de diversos circuitos, entre estas operaciones se encuentra la suma. Si bien se conoce que existen compuertas lógicas que permiten realizar este proceso como es el caso del circuito integrado 74LS32 que posee cuatro compuertas en su estructura, existen otros integrados que realizan la misma operación y se denominan sumadores.

Cuando se utilizan compuertas lógicas OR (suma) se tiene un número limitado de variables de entrada puesto que si se desea trabajar con un número elevado de estas variables, el proceso de obtención de las funciones lógicas resultantes y la implementación del diseño van a complicarse debido al elevado número de circuitos integrados que se utilizarán y por consecuencia no habrá una optimización de diseño y su construcción será más costosa.

Para esta limitante se emplean los circuitos integrados sumadores; un solo integrado de este tipo realiza la suma de hasta 8 variables de entrada (dos números 4 bits) lo cual facilita el diseño, interpretación, optimización e implementación.

En base los puntos planteados se pretende implementar un circuito sumador de dos números de 8 bits (16 variables de entrada) utilizando un circuito integrado sumador: LS74283 y visualizar su resultado en displays de 7 segmentos.

### 2. OBJETIVOS

**General**

* Diseñar un circuito sumador de dos números de 8 bits cada uno y mostrar su resultado en dos displays de 7 segmentos.

**Específicos**

* Entender el funcionamiento de los sumadores,sus caracteristicas y como se utilizan para armar el circuito Sumador.  
* Utilizar los integrados 74283 para la suma, y el decodificador 4511 de bcd a display de 7 segmentos para mostrar el resultado.
* Simular el circuito diseñado en el software Proteus y comprobar su funcionamiento.
* Implementar el circuito diseñado en la plataforma virtual Tinkercad.


### 3. ESTADO DEL ARTE

**Análisis de diferentes sumadores usando la lógica CMOS, CPL y DPL**

En este artículo se diseña y analizamos diferentes tipos de sumadores usando CMOS, lógica de transistor de paso complementario (CPL), lógica de transistor de doble paso (DPL). Ripple Carry Adder, Carry Look Ahead Adder, Carry Save Adder, Carry Increder Adder, Carry Skip Adder, Carry Select Adder, Conditional Sum Adder están diseñados con CMOS, lógica de transistor de paso complementario (CPL), lógica de transistor de doble paso (DPL) para Se comparan 16 bits, 32 bits y su velocidad, área y potencia.

**Autores**

* S. Nagaraj

Departamento de ECE, JNTUA, Anantapuramu, AP

* GM Sreerama Reddy

Departamento de ECE, CBIT, Kolar, KA

* S. Aruna Mastani

Departamento de ECE, JNTUA, Anantapuramu, AP

**Fecha y lugar de publicación:**

*Fecha:* 15-17 de diciembre de 2017  

*Lugar:* Roorkee, India en 14a Conferencia Internacional del Consejo de la India IEEE 2017 (INDICON)

Se relaciona con el presente trabajo ya que hace un análisis a diferentes sumadores entre ellos se analiza la tegnologia CMOS que es a la cual pertenece el sumador que se utiliza en el diseño del Circuito Sumador, por lo que permite entender de mejor manera con que se esta trabajando.


**Un estudio comparativo sobre sumadores**

En el articulo se realiza un comparación entres los sumadores, todos de 4 bits y se han sintetizado con la herramienta de síntesis Xilinx y se han simulado con la herramienta de simulación Xilinx. Los resultados de los informes de síntesis y la simulación del circuito ayudan a descubrir las diferentes propiedades de los sumadores,que son las que marcan la diferencia en la operación y el rendimiento de los mismos.

**Fecha y lugar de publicación:**

*Fecha:*  22-24 de marzo de 2017

*lugar:*  Chennai, India en 2017 Conferencia internacional sobre comunicaciones inalámbricas, procesamiento de señales y redes (WiSPNET)

**Autores**

- Bhavani Koyada

MGIT, JNTUH, Hyderabad

- N. Meghana

MGIT, JNTUH, Hyderabad

- MD Omair Jaleel

MGIT, JNTUH, Hyderabad

- Praneet Raj Jeripotula

MGIT, JNTUH, Hyderabad

El Artículo de un estudio comparativo sobre sumadores, se relaciona con nuestro trabajo debido a que analiza los sumadores  de 4 bit que es la herramienta con la cual se diseña el circuito, en el artículo utilizan herramientas más avanzadas analizan las propiedades de cda sumador y hallan el mejor de acuerdo a eso, en el presente trabajo se ha utilizado directamente un tipo de sumador sin embargo al leer el articulo, se entiende que existes otros tipos de sumadores que podían utilizarse de mejor forma.

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

*Fecha:* 21-22 April 2017 en la conferencia Innovaciones 2017 en energía y tecnologías de computación avanzadas (i-PACT)

Este artículo guarda relación con el trabajo de investigación, porque utiliza sumadores completos al igual que nuestro trabajo sin embargo los bits a sumarse y los tipos de sumadores cambian y para mostrar el resultado no usan displays como en el presente trabajo sino  también son mostrados de diferente forma sin embargo se semejan porque el objetivo es sumar dos números pero en el diseño se utiliza otro tipo de circuito.

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

**Figura 1:** Reglas de la Suma Binaria

**Semisumador**

Se denomina semisumador a un circuito que admite dos bits como entrada y genera  como salida  un bit que representa la suma de los dos bits de entrada y otro bit que representa 
el acarreo generado por la suma.

La tabla de verdad de este circuito puede deducirse a partir de las La tabla de verdad de este circuito puede deducirse a partir de las reglas de la suma binaria (Véase Fig.2).

![jf2](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf2.png)

**Figura 2:** Tabla de verdad del Semisumador.

A partir de esta tabla de verdad se puede observar que la suma puede implementarse con una operación XOR y el acarreo de salida con una operación AND(Canaria, 2012).

![jf3](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf3.png)

**Figura 3:** Esquema del Semisumador

**Sumador Completo**

La principal diferencia diferencia entre un sumador completo y un semisumador es que el sumador completo admite un valor que representa un acarreo de entrada.

 ![jf4](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf4.png)
 
 **Figura 4:** Tabla de verdad del Sumador Completo

Dado que la suma de dos bits está dada la operación XOR, también podemos expresar dicha suma  con un acarreo de la siguiente forma:

![jf5](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf5.png)

**Figura 5:** Expresión lógica del Sumador Completo

El acarreo de salida sera 1 entonces cuando A y B sean 1 o cuando A+B sea 1 al igual que el acarreo de entrada.

![jf6](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf6.png)

**Figura 6:** Expresión Lógica

De esta forma se puede implementar el circuito sumador completo usando dos compuertas XOR, dos compuestas AND y una compuerta OR.

![jf7](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf7.png)

**Figura 7:** Esquema del Sumador Completo

También es posible implementar el sumador completo utilizando dos circuitos semisumadores, el primer semisumador suma los dos bits, el segundo suma el resultado con el acarreo 
de entrada y habrá acarreo de salida si cualquiera  de los dos semisumadores genera un acarreo.

![jf8](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf8.png)

**Figura 8:** Sumador COmpleto a Partir de Semisumadores en Cascada

**Sumadores con Acarreo en Cascada**

El circuito sumador completo permite sumar dos números de un bit con un acarreo de entrada y generar un acarreo de salida. Como regla general, un sumador binario de cualquier número de bits puede realizarse conectando en cascada varios sumadores completos de un bit.

El proceso puede extenderse usando cuaquier sumador como elemento básico: por ejemplo puede hacerse un suamdor de 4 bits a partir de dos sumadores de 2 bits.

![jf9](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf9.png)

**Figura 9:** Sumadore de 4 bits

El principal problema de esta conexión en serie de sumadores es que el retardo del circuito depende de la propagación del acarreo a lo largo de todo el sumador.

![jf10](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf10.png)

**Figura 10:** Sumador de 8 bits 

Para la implementación del sumador de 8 bits se dio uso al integrado 74283

![jf11](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jf11.jpg)

**Figura 11:** Integrado 74283

### 5. DIAGRAMAS

**5.1. Diagrama de Entradas y Salidas del Circuito.**

![ent_sal.png](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/ent_sal.png)

**Figura 12:** Entradas y salidas del Circuito.

**5.2. Diagrama de Bloques del Circuito Sumador de 8 bits**

![Diagrama_bloques.JPG](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/Diagrama_bloques.JPG)

**Figura 13:** Circuito Sumador de 8 bits utilizando 2 sumadores de 4 bits conectados en cascada.

**5.3. Diagrama de Bloques del funcionamiento del circuito Sumador de 8 bits.**

![Funcionamiento.png](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/Funcionamiento.png)

**Figura 14:** En el Diagrama explica el funcionamiento del circuito Sumador de 8 bits.

**5.4. Diagramas electrónicos** 

A continuación se muestra el diagramas Electrónico, simulacion del diseños en Proteus.

![Simulación Proteus](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SimulacionProteus.png)

**Figura 15:** Diseño de circuito Sumador de 8 bits.

A continuación se muestra el diagrama Electrónico en THINKERCAD.

![Simulación Tinkercad](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SimulacionTinkercad.png)

**Figura 16:** Implementación del circuito Sumador de 8 bits.

### 6. LISTA DE COMPONENTES

En la Tabla 1 se muestra las herramientas  de software usadas para la simulacion del circuito se utilizó un simulador y la plataforma para la implementación.

**Tabla 1: Herramientas de Software usadas para el diseño de los 3 circuitos.**

   |     **Herramientas de Software**      |                 
   |---------------------------------------|
   |            Proteus                    | 
   |           Tinkercad                  |
  
   
**Tabla 2: Datos de los integrados usados para el diseño de Circuito Sumador de 8 bits**

   | **N°**  |   **Integrados** |   **Códigos**    |     
   |-------|--------------|----------------|
   |      1|   Sumador	  |     74283      |
   |      1| Decodificador|     4511       |
  
**Tabla 3: Componentes electronicos del Circuito Sumador de 8 bits**

  | **N°** |**Componentes Electronicos**	|    
   |-------|------------------------------|
   |     30|   Resistencias de 330        |    
   |      2|   Dip Switch 8 entradas      |     
   |      1|   Fuente de 5 V              |   
   |      8|   Led Green                  | 
   |      2|   Display 7 segmentos        | 

### 7. MAPA DE VARIABLES

 |**Variable** | 	**Tipo**   | **Descripción**|
 |-------------|----------------|-------------------|
 |A0,A1,A2,A3,A4,A5,A6,A7|  Entrada|Son los bits de Entrada del numero A donde A7 es el bit mas significativo y A0 es el bit menos significativo|
 |B0,B1,B2,B3,B4,B5,B6,B7| Entrada|	Son los bits de Entrada del numero B donde B7 es el bit mas significativo y B0 es el bit menos significativo|
 |S0,S1,S2,S3,S4,S5,S6,S7	| Salida|Son los bits de Salida del resultado de la suma donde S7 es el bit mas significativo y S0 es el bit menos significativo|
 |Ci	  | Entrada	|Acarreo de entrada|
 |CO	  |Salida	  |Acarreo de SalidaSalida|

### 8. EXPLICACIÓN DEL CÓDIGO FUENTE

* Para realizar el circuito sumador de dos números de 8 bits primero se definen las variables de entrada y salida que tendrá el circuito, todas se encuentran en lógica positiva y se presentan de la siguiente forma:

![Diagrama de bloques: Sumador 8 Bits](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/ENTRADAS.png)

**Figura 17:** Diagrama de bloques: Sumador 8 Bits

**Entradas**

**Número A**: A7, A6, A5, A4, A3, A2, A1, A0
Donde: A0 es el bit menos significativo y A7 es el más significativo

**Número B**: B7, B6, B5, B4, B3, B2, B1, B0
Donde: B0 es el bit menos significativo y B7 es el más significativo

![Entradas en DIPSW](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DIPSENTRADAS.PNG)

**Figura 18:** Entradas en DIPSW

**Salidas**

S8, S7, S6, S5, S4, S3, S2, S1, S0
Donde: S0 es el bit menos significativo y S8 (acarreo) es el más significativo.

![Salidas del Sumador](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SALIDAS1.PNG)

**Figura 19:** Salidas del Sumador

* Para realizar el proceso de la suma binaria se utiliza el circuito integrado 74LS283 que cumple la función de sumador.

![Sumador LS74283](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SUM.png)

**Figura 20:** Sumador LS74283

Donde A0 - A3 representan los cuatro primeros bits del número A y B0 - B3 del número B, sin embargo, los números de las entradas son de 8 Bits de magnitud entonces para realizar la suma se necesita realizar una conexión en cascada entre dos sumadores.

Para que se cumpla el proceso se debe conocer las reglas de la suma binaria:

![Reglas de la suma binaria](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/REGLASUMA.PNG)

**Figura 21:** Reglas de la suma binaria

El integrado 74LS283 tiene dos pines que representan el acarreo de entrada y salida, entonces para realizar la conexión en cascada: el acarreo de salida del primer sumador es el acarreo de entrada del segundo, por lo tanto, ambos se encuentran conectados y en las entradas del integrado se colocan las cuatro variables restantes de los números A y B, las cuales son: A4 - A7 y B4 - B7 identificando la conexión de los bits más y menos significativos.

![Conexión en cascada](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SUMCASCADA.png)

**Figura 22:** Conexión en cascada

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

**Figura 23:** Resultado de la suma binaria representado con LEDS

* Para visualizar este resultado en un display de 7 segmentos se utiliza el decodificador 4511 conectado a las salidas de cada sumador y a su vez a las entradas del display junto con resistencias para evitar que el dispositivo sufra daños.

![Decodificador 4511](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DECODIFICADOR.PNG)

**Figura 24:** Decodificador 4511

* Para conectar el display se debe tomar en cuenta la estructura que posee, para este circuito se usa un display 7 segmentos cátodo común. Esto quiere decir que el pin común del display debe ir conectado a tierra:

![Display 7 seg catodo común](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DISPLAY.PNG)

**Figura 25:** Display 7 seg catodo común

* Hay que tomar en cuenta que para los displays de 7 segmentos el número más alto que se puede visualizar es el nueve, por lo tanto cuando el resultado de la suma implique un número mayor al indicado, no se va a encender el display:

![Display encendido](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DISPLAYENCENDIDO.png)

**Figura 26:** Display encendido

![Display apagado](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DISPLAYAPAGADO.png)

**Figura 27:** Display apagado

* El resultado se todos estos procesos da un circuito sumador de dos números de 8 bits como se muestra a continuación en el software de simulación Proteus:

![Simulación Proteus](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SimulacionProteus.png)

**Figura 28:** Simulación Proteus

* La implementación del circuito en el laboratorio virtual Tinkercad se presenta de la siguiente forma:

![Simulación Tinkercad](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SimulacionTinkercad.png)

**Figura 29:** Simulación Tinkercad

Para ver el circuito completo ingresar en: https://www.tinkercad.com/things/cYY3aJ8o0qT-sumador-de-8-bits/editel?sharecode=WZe_mOvoBysl6DT_NBUMBbBigi_x7lmxiFtQwO06Kec

### 9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

En el circuito para realizar la conexión entre las salidas de los circuitos y el display de 7 segmentos hicimos uso de un Decodificador 4511 BCD de 7 segmentos cuyas características se muestran en la tabla 9.

| **Código**|**Características**	|    
|---------- |--------------------|
|   4511    | El CD4511 es un decodificador bcd de 4 bits para display cátodo común, que utiliza tecnología cmos.                                                                             Recibe en los Pines de entrada a ABCD los datos en código binario y los decodifica a código decimal,                                                                             siendo posible su exhibición en los display de 7 segmentos.|  
                                              
![4511.gif](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/4511.gif)

**Figura 30:** Integrado 4511

El circuito fue implementado en la plataforma Thinkercad como se muestra que ha acontinuación

![Thinkercad.png](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/Thinkercad.png)

**Figura 31:** Circuito Implementado

|                 **Herramientas de Software**       |                  **Descripción**                      |
|----------------------------------------------------|-------------------------------------------------------|
|              Tinkercad                            | Tinkercad es una sencilla aplicación en línea de diseño e impresión en 3D para todos, creado por la empresa Autodesk. Sus ventajas son claras: es sencillo de usar, su aspecto es atractivo y con unas pocas horas de entrenamiento podemos                                                           adquirir mucha destreza en su uso. Como desventaja podríamos señalar que es necesario tener una cuenta de correo para darse de alta como usuario y que sólo                                                         posee una versión online, por lo que hace falta conexión a internet.|

### 10. APORTACIONES

**Constructor virtual de circuitos**

Esta útil herramienta la usamos para poder comprobar si la implementación hecha en Tinkercad era correcta, ya que también nos permite simular circuitos digitales para corroborar el correcto funcionamiento de nuestro circuito debido a que durante la realización del mismo se presentaron una serie de complicaciones que posterior mente fueron solucionadas con ayuda de este Simulador virtual.
Sencillo, intuitivo, pero poderoso simulador de circuitos digitales, cuenta con todas las compuertas lógicas y una interfaz fácil y rápida de aprender y dominar.

![jAportaciones](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jAportaciones.jpeg)

**Figura 32:** Circuito Implementado en El constructor Virtual de Circuitos

Por su diseño en forma de protoboard asemeja el circuito real sirviendo ademas como guía para ensamblar el circuito de forma física.

Se incluye ademas el manual TTL con los datasheet de cada compuerta y circuito integrado de la familia de los TTL, donde se puede consultar el diagrama interno de cada uno y su funcionamiento.

Constructor Virtual de Circuitos Electrónicos y Manual TTL, ideal para quienes inician en el mundo de la electrónica digital, practicar el uso de la Protoboard etc.

![jAporte2](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jAporte2.png)

**Figura 33:** Circuito Implementado Físicamente

### 11. CONCLUSIONES

•	Para realizar la suma de dos números de 8 bits se debe realizar una conexión en cascada de dos sumadores para que se refleje el resultado completo.

•	Para el resultado de cualquier operación suma se debe considerar cuales son los números más grandes que se pueden sumar y por lo tanto siempre aumenta un bit a la salida, por lo tanto, si se operan dos números de 8 bits cada uno, el resultado será un binario de 9 bits.

•	Hay que tomar en cuenta que para los displays de 7 segmentos el número más alto que se puede visualizar es el nueve, por lo tanto, cuando el resultado de la suma implique un número mayor al indicado, no se va a encender el display

•	La manera idónea para conectar sumadores es atar el acarreo de salida del sumador de menor peso, con el acarreo de entrada del integrado de mayor peso, y de esta manera el residuo de la suma es transferido para tomar en cuenta cualquier valor que venga acumulado. 


### 12. RECOMENDACIONES

•	Se debe tomar en cuenta el valor del acarreo de entrada y salida para cada sumador ya que puede aleterar el resultado.

•	Debemos establecer adecuadamente los bits mas significativos y menos significativos que van a ingresar a cada sumador. 

•	Para las conexion adecuada del display se debe conciderar si será de ánodo o cátodo común para asegurar un correcto funcionamiento del mismo en el circuito diseñado.

•	Verificar que no se encuentren conectadas entradas y/o salidas en un mismo punto para que no se generen errores de operación y así evitar que nuestro integrado daños en el integrado.

### 13. CRONOGRAMA

![jcronograma](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/jcronograma.png)

### 14. BIBLIOGRAFÍA

https://wilaebaelectronica.blogspot.com/2017/01/sumador-binario.html

https://iesbernatguinovart.com/04v_tecnologia/carpeta_arxius/elec%20dig%20basica.pdf

https://www.studocu.com/pe/document/universidad-nacional-del-callao/circuitos-digitales-turno-01t-ciclo-5/informe/circuitos-aritmeticos/5637738/view

http://homepage.cem.itesm.mx/garcia.andres/PDF201411/Aritmetica(Basis).pdf

http://circuitos-aritmeticos.blogspot.com/

http://serdis.dis.ulpgc.es/~gii-fc/material_clases_teoria/Tema3/Tema3_1_Componentes_combinacionales_FC_GII.pdf

### 15. ANEXOS

**15.1.  MANUAL DE USUARIO**

* Primero se debe encender el suministro de energía para alimentar al circuito:

![Energia](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/ENERGIA.PNG)

**Figura 34:** Energia

Para realizar la operación suma entre dos números de 8 bits se debe ingresar los números deseados por los dip switchs del circuito: 
A7-B7: Bit más significativo
A0-B0: Bit menos significativo

![Entradas del circuito en dip switch](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/INGRESO.PNG)

**Figura 35:** Entradas del circuito en dip switch

* Los números ingresados pasan a los sumadores que realizan la operación bit a bit:

![Sumadores](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SUMADORES.PNG)

**Figura 36:** Sumadores

* El resultado se muestra en la salida de los LEDS de forma binaria:
Encendido: 1 
Apagado: 0

![Salida en LEDS](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/SALIDABIN.PNG)

**Figura 37:** Salida en LEDS

* Los números resultantes en forma decimal se muestran en los display de 7 segmentos con ayuda de un decodificador:

![Display de 7SEG](https://github.com/JorgeGallegos99/Trabajo-de-investigacion-2/blob/master/Img/DECDISPLAY.PNG)

**Figura 38:** Display de 7SEG

