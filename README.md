Informe

1. PLANTEAMIENTO DEL PROBLEMA

2. OBJETIVOS

3. ESTADO DEL ARTE

4. MARCO TEÓRICO

**Circuitos Aritméticos**

Dentro de la variada gama de circuitos digitales, tenemos los denominados circuitos aritméticos que son dispositivos que pueden realizar operaciones aritméticas (suma, 
resta, multiplicación y división) en formato binario o BCD, punto fijo o punto flotante. 

Dependiendo de la función a realizar, tenemos sumadores, restadores, multiplicadores, divisores y funciones combinadas de los mismos para realizar operaciones complejas como por 
ejemplo el cálculo de raíz cuadrada, exponenciales, etc.

Si bien es posible generar funciones complejas en base al uso de un microprocesador, a través de algoritmos que se corren en un programa, la posibilidad de generar dichas 
funciones en hardware, en muchos casos, presentan ventajas en cuanto a velocidad y/o el empleo de menores recursos lógicos, como es el caso de la ausencia de un micro para realizarlas (Hoyos Padilla, 2010).

**Sumadores**

La suma o adición binaria es análoga a la de los números decimales. La diferencia radica en que en los números binarios se produce un acarreo (carry) cuando la suma excede de uno mientras en decimal se produce un acarreo cuando la suma excede de nueve (Hoyos Padilla, 2010).

![jf1]()

la figura muestra las reglas que debemos seguir cuando realizamos las operaciones de suma binaria.

**Semisumador**

Se denomina semisumador a un circuito que admite dos bits como entrada y genera  como salida  un bit que representa la suma de los dos bits de entrada y otro bit que representa 
el acarreo generado por la suma.

La tabla de verdad de este circuito puede deducirse a partir de las La tabla de verdad de este circuito puede deducirse a partir de las reglas de la suma binaria (Véase Fig. ).

![jf2]()

A partir de esta tabla de verdad se puede observar que la suma puede implementarse con una operación XOR y el acarreo de salida con una operación AND(Canaria, 2012).

![jf3]()

**Sumador Completo**

La principal diferencia diferencia entre un sumador completo y un semisumador es que el sumador completo admite un valor que representa un acarreo de entrada.

![jf4]()

Dado que la suma de dos bits está dada la operación XOR, también podemos expresar dicha suma  con un acarreo de la siguiente forma:

![jf5]()

El acarreo de salida sera 1 entonces cuando A y B sean 1 o cuando A+B sea 1 al igual que el acarreo de entrada.

![jf6]()

De esta forma se puede implementar el circuito sumador completo usando dos compuertas XOR, dos compuestas AND y una compuerta OR.

![jf7]()

También es posible implementar el sumador completo utilizando dos circuitos semisumadores, el primer semisumador suma los dos bits, el segundo suma el resultado con el acarreo 
de entrada y habrá acarreo de salida si cualquiera  de los dos semisumadores genera un acarreo.

![jf8]()

**Sumadores con Acarreo en Cascada**

El circuito sumador completo permite sumar dos números de un bit con un acarreo de entrada y generar un acarreo de salida. Como regla general, un sumador binario de cualquier número de bits puede realizarse conectando en cascada varios sumadores completos de un bit.

El proceso puede extenderse usando cuaquier sumador como elemento básico: por ejemplo puede hacerse un suamdor de 4 bits a partir de dos sumadores de 2 bits.

![jf9]()

El principal problema de esta conexión en serie de sumadores es que el retardo del circuito depende de la propagación del acarreo a lo largo de todo el sumador.

![jf10]()

Para la implementación del sumador de 8 bits se dio uso al integrado 74283

![jf11]()


5. DIAGRAMAS

5.1. Diagrama de Bloques

5.2. Diagramas electrónicos 

6. LISTA DE COMPONENTES

7. MAPA DE VARIABLES

8. EXPLICACIÓN DEL CÓDIGO FUENTE

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



