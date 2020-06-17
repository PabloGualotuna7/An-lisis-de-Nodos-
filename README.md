# Análisis de Nodos 

1. PLANTEAMIENTO DEL PROBLEMA 

En el siguiente informe de laboratorio se va a emplear los conocimientos aprendidos en la teoría de la materia de Fundamentos de Circuitos eléctricos, estudiaremos el análisis de las mallas en los circuitos eléctricos para tener una facilidad en la aplicación y resolución de ejercicios. Así como también podemos comparar los resultados calculados frente a los medidos con el programa TINKERCAD (laboratorio virutal), mediante la resolución del circuito eléctrico planteado en la guía entregada por el docente.

2. OBJETIVOS

* Realizar el circuito indicado y medir los voltajes en cada uno de los nodos formados.

* Comparar el valor de cada medición de voltaje obtenidos en cada nodo.


3. MARCO TEÓRICO 

El análisis de nodos es posible cuando todos los nodos tienen conductancia. Este método produce un sistema de ecuaciones, que puede resolverse a mano si es pequeño, o tambiénpuede resolverse rápidamente usando álgebra lineal en un computador. Por el hecho de que forme ecuaciones muy sencillas, este método es una base para muchos programas de simulación de circuitos (Por ejemplo, Tinkercad). Cuando los elementos del circuito no tienen conductancia, se puede usar una extensión más general del análisis de nodos, El análisis de nodos modificado.

¿Qué es una nodo?

En ingeniería eléctrica y electrónica, un nodo es un punto donde dos o más componentes tienen una conexión común. Corresponde a una unión de alambres hechos de material conductor que poseen una resistencia eléctrica cercana a 0.

![](https://github.com/JavoEstevez/An-lisis-de-Nodos-/blob/master/img/nodo.png)

¿En qué consiste el método de nodos?

El método de los voltajes de nodos consiste en determinar los voltajes en los nodos (puntos de intercepción de las ramas de un circuito eléctrico), y luego calcular las corrientes en las ramas. Se fundamenta en la Ley de Kirchhoff de corrientes, la cual plantea que las cargas no se pueden acumular en ningún nodo, y en la Ley de Ohm.

Es fácil hallar un nodo usando la ley de Ohm o aplicando la ley de Kirchhoff de corrientes teniendo en cuenta las corrientes que entran a un nodo, teniendo en cuenta variables como las impedancias que comparte el nodo con respecto al voltaje que cae sobre el nodo. Cuando miramos el esquema de un circuito, los cables ideales tienen una resistencia de cero (esto no pasa en la vida real, pero es una buena aproximación). Si se asume que no hay cambio de potencial en cualquier parte del cable, todo el cable entre cualquier componente de un circuito es considerado parte del mismo nodo

Pasos para aplicar el método de nodos

a. Localice los segmentos de cable conectados al circuito. Estos serán los nodos que se usarán para el método.

b. Seleccione un nodo de referencia (polo a tierra). Se puede elegir cualquier nodo ya que esto no afecta para nada los cálculos; pero elegir el nodo con más conexiones podría simplificar el análisis.

c. Identifique los nodos que están conectados a fuentes de voltaje que tengan una terminal en el nodo de referencia. En estos nodos la fuente define la tensión del nodo. Si la fuente es independiente, la tensión del nodo es conocida. En estos nodos no se aplica la LCK.

d. Asigne una variable para los nodos que tengan tensiones desconocidas. Si la tensión del nodo ya se conoce, no es necesario asignarle una variable.

e. Para cada uno de los nodos, se plantean las ecuaciones de acuerdo con las Leyes de Kirchhoff. Básicamente, sume todas las corrientes que pasan por el nodo e igualelas a 0. Por lo general el número de ecuaciones es menor a al número de nodos localizados.

f. Si hay fuentes de tensión entre dos tensiones desconocidas, una esos dos nodos como un supernodo, haciendo el sumatorio de todas las corrientes que entran y salen en ese supernodo. Las tensiones de los dos nodos simples en el supernodo están relacionadas por la fuente de tensión intercalada.

g. Resuelva el sistema de ecuaciones simultáneas para cada tensión desconocida.

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
