# Análisis de Nodos 

1. PLANTEAMIENTO DEL PROBLEMA 

En el siguiente informe de laboratorio se va a emplear los conocimientos aprendidos en la teoría de la materia de Fundamentos de Circuitos eléctricos, estudiaremos el análisis de las mallas en los circuitos eléctricos para tener una facilidad en la aplicación y resolución de ejercicios. Así como también podemos comparar los resultados calculados frente a los medidos con el programa TINKERCAD (laboratorio virutal), mediante la resolución del circuito eléctrico planteado en la guía entregada por el docente.

2. OBJETIVOS

* Medir circuitos de c.d. de varias mallas con múltiples fuentes de voltajes y múltiples resistores.

* Entender las conexiones y forma de uso del protoboard, del multímetro y de los demás materiales de laboratorio para hacer un uso correcto de ellos, ya que cada uno tiene una forma específica de uso.

* Resolver un circuito eléctrico generando un sistema de ecuaciones simultáneas que se obtienen aplicando las leyes de Kirchhoff y las relaciones i-v (corriente-voltaje) de los elementos del circuito en la o las mallas del circuito.

* Comparar los cálculos teóricos con los prácticos de medición de intensidad de corriente eléctrica y analizar el posible margen de error.

3. MARCO TEÓRICO 

Un circuito de varias mallas es el que tiene dos o más mallas, esto significa que tiene diferentes trayectorias cerradas de elementos. Los elementos de las mallas están en serie o paralelo y éstos conducen la misma corriente. Para resolver estos circuitos se determina de forma fácil haciendo uso de las Leyes de Kirchhoff mas específicamente la Ley de Voltajes, se calcula la corriente total de la malla y ya con este dato se determinan los voltajes y las potencias de cada resistor. El voltaje de la fuente equivalente se calcula usando la ley de voltaje de Kirchhoff siguiendo la dirección de las manecillas del reloj usando el flujo de corriente convencional.

¿Qué es una malla?

![](https://github.com/PabloGualotuna7/ANALISIS_DE_MALLAS/blob/master/img/1.jpg)

En un circuito eléctrico, una malla es un camino cerrado formado por elementos de circuitos. En este caso hay 4 mallas, formadas por 4 caminos cerrados. Si no hay una fuente de voltaje o de corriente en una malla entonces asumimos que la corriente fluye en un sentido horario. Se podría asumir en el sentido anti horario, lo cual no interesa mucho ya que si se escoge un sentido incorrecto la corriente que nos resultará al hacer nuestros cálculos tendrá signo negativo. Esto lo podremos apreciar al final cuando obtengamos nuestra respuesta.

Las corrientes las debemos representar en nuestro diagrama se la siguiente manera:

![](https://github.com/PabloGualotuna7/ANALISIS_DE_MALLAS/blob/master/img/2.jpg)

Vemos que en la malla 1 se asume que la corriente va en sentido horario ya que sale del positivo de la fuente. En las mallas 2 y 3 no hay fuente, así que se asume libremente (preferiblemente en sentido horario). En la malla 4 la corriente va en sentido anti horario por salir del positivo de la fuente de voltaje.

* Ley de Ohm: sean V el voltaje, R la resistencia e I la corriente del elemento resistivo óhmico, en el cual el voltaje y la corriente son directamente proporcionales, siendo la resistencia la constante de proporcionalidad: V = I.R

* Ley de Kirchhoff del voltaje (LKV): en cualquier trayectoria cerrada recorrida en una sola dirección, la suma algebraica de los voltajes es cero. Esto incluye los voltajes debidos a fuentes, resistores, inductores o capacitores: ∑ E = ∑ Ri. I

* Ley de Kirchhoff de la corriente (LKC): en cualquier nodo, la suma algebraica de las corrientes es cero, teniendo en cuenta que a las corrientes que entran se les asigna un signo y a las que salen otro. De esta forma: ∑ I = 0.

El análisis de mallas es una técnica empleada para resolver circuitos eléctricos planos. Este procedimiento también puede aparecer en la literatura con el nombre de método de las corrientes de malla (o lazo). Además, es un método general que sirve para resolver circuitos cuyos elementos están conectados en serie, en paralelo o de forma mixta, es decir, cuando no se distingue claramente el tipo de conexión. El circuito debe ser plano, o al menos debe ser posible re-dibujarlo como tal.

Pasos a seguir en un análisis por mallas:

* Paso 1. Asignar una corriente de malla a cada malla (sentido cualquiera) y asignar una polarización a cada elemento del circuito.
* Paso 2. Establecemos un sentido de circulación siguiendo el cual aplicamos KVL a cada malla. Tendremos tantas ecuaciones como mallas.
* Paso 3. Usamos las relaciones V/I (Ley de Ohm) para expresar las tensiones en función de las corrientes en las ecuaciones de 2.
* Paso 4. Sustituimos las ecuaciones del paso 3 en 2.
* Paso 5. Obtenemos las corrientes de malla.

4. DIAGRAMAS

Circuito Eléctrico

![](https://github.com/JavoEstevez/An-lisis-de-Nodos-/blob/master/img/%7B82D5275B-6BA9-4C7B-886A-C33CDF6B8261%7D.png.jpg)

Descripción del circuito.

* En el diagrama se observa dos fuentes voltajes independientes, conectadas a los extremos del circuito.
* Además, dentro del circuito se aprecia 5 resistencias medidas en kOhms
* Al momento de unir dos elementos eléctricos, se forman nodos que para el caso del circuito de la práctica reconocemos 3 nodos principales.
* Se tiene que la resistencia de 0.82 KOhm forma nodo con las resistencias de 1,2 KOhm y 1 KOhm. La resistencia de 1.2 KOhm forma un nodo con las resistencias de 0.39 KOhm y 2.2 kohm. Como nodo de referencia o tierra es toda la sección de abajo del circuito eléctrico.
* En el caso de este circuito eléctrico identificamos 3 mallas, colocando una intensidad en cada malla denotándolas como I1, I2, I3 todas en sentido de las manecillas del reloj.

Circuito Eléctrico hecho en Tinkercad

![](https://github.com/PabloGualotuna7/ANALISIS_DE_MALLAS/blob/master/img/Circuito_Armado.png)

Circuito Elécrtico con mediciones realizado en Proteus 

![](https://github.com/PabloGualotuna7/ANALISIS_DE_MALLAS/blob/master/img/Circuito_Proteus.png)

5. LISTAS DE COMPONENTES

![](https://github.com/PabloGualotuna7/ANALISIS_DE_MALLAS/blob/master/img/Componentes.png)

6. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

* Abrimos el sitio web "tinkercad" y creamos una cuenta.

* Hacemos clic izquierdo en "Circuits" y comenzamos con la práctica.

* Seleccionamos una placa de pruebas pequeñas (Protoboard).

* Se selecciona y se conecta al protoboard los suministros de energía asignándole el valor de 5 y 18 V.

* Escogemos cinco resistencias y las conectamos siguiendo el diagrama visto en el archivo de la práctica, que en este caso son 5 de valores de 820 Ohm, 1.2k Ohm, 390 Ohm, 1K Ohm y 2.2k Ohm.

* Haciendo clic izquierdo en los pines del protoboard conectamos con cables las resistencias y pasamos corriente a donde haga falta.

* Colocamos un multímetro y cambiamos la configuración del multímetro en amperaje y conectamos en serie con el circuito, el color negro es el negativo mientras que el color rojo es el positivo. 

* Realizamos las mediciones de corriente pedidas en la guía.

* Anotamos los valores obtenidos en las tablas de la guía de laboratorio.

* Guardamos y salimos.

7. TABLAS DE MEDICIONES Y CÁLCULOS 

| Malla| Resultados Analíticos | Resultados Experimentales| Resultados Simulados|
| --    |                 ---- |-------------             |----------------      |
| 1 |                   11.46mA| 11.5mA                   |11.5mA                |
|2  |                   2.85mA |2.85mA                    |2.85mA                |              
|3  |                   0.49mA | 0.488mA                  |0.49mA                |

8. CONCLUSIONES 

* Este método nos permite hallar las tensiones en cualquier parte del circuito, debido a que encontramos la corriente de la malla, además la ventaja de usar este método es que nos brinda un sistema de ecuaciones para luego hallar lo que deseamos.

* Los errores relativos no pasan del 1% por lo cual nuestros valores son casi perfectos y no hay fallo en la medición que realizamos, esto debido también a que los simuladores que usamos son un software programado con un cierto número de decimales, mientras que nosotros usamos como máximo de dos decimales válidos.

* Y de lo anterior, se concluye que el método de Análisis de Mallas es un método práctico y muy útil para el análisis de circuitos, y que no requiere tanta complejidad, aunque existan variaciones en su forma de aplicarlo.

9. RECOMENDACIONES 

* Al momento de realizar la práctica en el simulador se hizo un mal posicionamiento de ciertos elementos del circuito, esto genera que los valores sean diferentes o que no se pueda hacer una correcta toma de los datos, recomendamos antes de proceder con la parte experimental tener claro el diagrama del circuito a usar.

* Es muy importante entender el porqué la realización de esta práctica puesto que más adelante se verán temas un poco más complejos, donde procedimientos como realizados en este laboratorio no debe contener errores significativos.

10. CRONOGRAMA

Actividades desarrolladas a lo largo de la practica de laboratorio.

![](https://github.com/PabloGualotuna7/ANALISIS_DE_MALLAS/blob/master/img/Cronograma.png)

11. BIBLIOGRAFÍA 

2015 Educatina LLC. (2015). educatina. Recuperado el 11 de Diciembre de 2015. Obtenido de http://www.educatina.com/buscar?q=circuitos+el%C3%A9ctricos+

Alexander, C. 2006. Fundamentos de Circuitos Eléctricos. 3ra. Edición. Mc Graw Hill.

Boylestad, R. 2011. Introducción al Análisis de Circuitos.2da. Edición. Pearson.

Dorf, R., & Svoboda, J. (2011). Circuitos eléctricos. México: Alfaomega.

Matrix calculator. (s.f.). Obtenido de Matrix calculator: https://matrixcalc.org/es/slu.html#solve-using-Gauss-Jordan-elimination%28%7B%7B-%2891/50%29,1,0,-18%7D,%7B1,-%2822/5%29,11/5,0%7D,%7B11/5,-%28259/100%29,0,5%7D%7D%29
