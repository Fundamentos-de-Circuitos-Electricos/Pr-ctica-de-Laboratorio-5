![image](https://user-images.githubusercontent.com/85137398/126711389-6d9a6260-111b-44c5-b987-e0450280a0ed.png)

# Práctica de Laboratorio 5

1. OBJETIVOS

*General*

- Identificar y aplicar el Teorema de Thevénin para lograr simplificar los cálculos de un circuito eléctrico complejo por un circuito eléctrico equivalente mucho más simple, donde interviene una fuente de tensión y una resistencia como elementos principales. 

*Especificos*

- Conocer los fundamentos básicos de este teorema y su aplicación.

-	Analizar el circuito DC mediante la aplicación de los Teoremas Thévenin.

- Verificar los parámetros Vth, Rth, determinados para el teorema de Thévenin y comprobar experimentalmente que se cumplan los teoremas en estudio.

2. MARCO TEÓRICO 

![image](https://user-images.githubusercontent.com/85137398/126720317-387940b3-100e-438a-910a-55da92db9395.png)

![image](https://user-images.githubusercontent.com/85137398/126720336-0185f413-ef95-4e48-a4da-9dfcb020b064.png)

3. EXPLICACIÓN DEL PROCESO

- Material y equipo requerido

![image](https://user-images.githubusercontent.com/85137398/126711871-887bb994-b9a3-4e91-a0fa-d39b9c8f00fe.png)

- Descripcion de equipo y material

Protoboard: Un protoboard es una placa de pruebas en la que se pueden insertar componentes electrónicos y cables, donde se puede ensamblar un circuito sin la necesidad de soldar ningún componente. El protoboard tiene agujeros conectados entre sí, por medio de pequeñas láminas metálicas.

Resistores: Una resistencia o resistor al componente electrónico diseñado para introducir una resistencia eléctrica determinada entre dos puntos de un circuito eléctrico.

Fuente de voltaje: En electrónica, el elemento activo que puede transferir energía se llama fuente de voltaje.

Multímetro digital: Un multímetro digital es una herramienta que sirve para medir dos o más valores eléctricos, principalmente tensión (voltios), corriente (amperios) y resistencia (ohmios).

- Armado del circuito

I. Escoger las fuentes de energia de 12v y 2v respectivamente.

![image](https://user-images.githubusercontent.com/85137398/126712173-b5eed82b-1ac2-4d58-94ac-165c9d803d35.png)

II. Escoger correctamente los resistores con su codificación de colores.

![image](https://user-images.githubusercontent.com/85137398/126712501-49310d2a-009d-4e41-b20b-c6d3001f56d0.png)

III. Conectar el circuito en base al diagrama de conexión.

- Diagrama esquemático

![image](https://user-images.githubusercontent.com/85137398/126712626-01e3c6fc-7ad0-487c-b38c-2824990f7526.png)

- Conexión del circuito

![image](https://user-images.githubusercontent.com/85137398/126714129-8d71b330-001d-4576-8079-8dc83c71f3c2.png)

4. RESPUESTAS A INTERROGANTES Y CÁLCULO DEL ERROR

* Desconecte el resistor R5 y mida el voltaje en el circuito abierto. Anote el valor
medido en la tabla 5.1.

![image](https://user-images.githubusercontent.com/84390686/126749221-1a78d86b-4da5-41ca-aa25-88393254fa97.png)

CALCULAMOS EL VOLTAJE DE THEVENIN

![image](https://user-images.githubusercontent.com/84390686/126749343-2417222a-d21b-4942-aa94-1d325d22ee24.png)

SACAMOS LAS ECUACIONES DE CADA MALLA

MALLA 1

(560 + 4700) I1 – 4700I2 – 12 = 0

5260 I1 – 4700 I2 - 12 = 0      ECUACIÓN (1)

MALLA 2

(330 + 4700) I2 – 4700I1 – 2 = 0

5030 I2 – 4700 I1 - 2 = 0       ECUACIÓN (2)

IGUALAMOS LA ECUACIÓN (1) CON LA ECUACIÓN (2) Y DESPEJAMOS I1

5260 I1 – 4700 I2 – 12 = 5030 I2 – 4700 I1 – 2

9960 I1 = 9730 I2 + 10

I1 = (9730 I2 + 10) / 9960

REMPLAZO I1 EN LA ECUACIÓN (2)

5030 I2 – 4700 ((9730 I2 + 10) / 9960) - 2 = 0

5030 I2 – ((2286550 I2 + 2350) / 498) = 2

(2504940 I2 – 2286550 I2 – 2350) / 498 = 2

218390 I2 – 2350 = 996

I2 = 3346/218390

I2 = 0.01532 A

REMPLAZAR I2 EN I1

I1 = ((9730 · 0.01532) + 10) / 9960

I1 = (149.0636 + 10) / 9960

I1 = 0.01597 A

CALCULAMOS EL VOLTAJE DE THEVENIN

VTH = 0.01532 · 330

VTH = 5.056 V

VALORES DEL CIRCUITO EQUIVALENTE DE THÉVENIN

![image](https://user-images.githubusercontent.com/84390686/126750528-268898af-f380-4f6e-aa24-1d5fd2d97617.png)

* Anule el efecto de las fuentes de alimentación. Desconecte R5 y desde el circuito
abierto resultante mida la resistencia equivalente. Anote el valor medido en la tabla 5.1.

![image](https://user-images.githubusercontent.com/84390686/126749474-61a7728e-5227-4c00-a986-1c8cbb5efea6.png)

ENCONTRAMOS EL CIRCUITO EQUIVALENTE 1

Req1= (560Ω · 4700Ω) / (560Ω + 4700Ω)
Req1= 500.38Ω

![image](https://user-images.githubusercontent.com/84390686/126749604-59752c17-c2ed-43fb-9d27-32530f988157.png)

ENCONTRAMOS EL CIRCUITO EQUIVALENTE 2

Req2= (500.38Ω · 330Ω) / (500.38Ω + 330Ω)
Req2= 198.85Ω

![image](https://user-images.githubusercontent.com/84390686/126749660-039d976c-8df1-4225-8e66-1fb1f80ceca7.png)

ENCONTRAMOS LA RESISTENCIA EQUIVALENTE DE THEVENIN

RTH= 198.85Ω + 100Ω
RTH= 298.85Ω

![image](https://user-images.githubusercontent.com/84390686/126749702-0c61ab98-f581-46e1-a696-519ea03e5f48.png)

VALORES DEL CIRCUITO EQUIVALENTE DE THÉVENIN

![image](https://user-images.githubusercontent.com/84390686/126750639-f5e03302-4764-44a0-af8f-6223e8f4dee6.png)

* Mida el voltaje y la corriente en el resistor R5, anote los resultados en la tabla 5.2.

A continuacion calculamos los valores teóricos de voltaje y corriente en el circuito para completar las interrogantes.

* Calculamos la Intensidad en R5 y su voltaje para ello, vamos a utilizar la ley de mallas de Kirchhoff: 

![image](https://user-images.githubusercontent.com/84390820/126748399-016c49e7-e2c9-4a74-ba61-8bc6a602c1bf.png)

Planteando y simplificando las ecuaciones obtenemos: 

5260 I1 - 4700 I2 = 12

-4700 I1 + 5030 I2 = 2

-330 I2 + 1430 I3 = 0 

Resolviendo el sistema de ecuaciones tenemos que I3 = 3.89 * 10 ^(-3) A 

Entonces para determinar el voltaje de R5 utilzmos Ley de Ohm: VR5 = 1 kohm * 3.89 mA  = 3.89 V 

![image](https://user-images.githubusercontent.com/84390820/126746116-bd999a22-3aaa-4caf-b5c5-da3dd7a78ee7.png)

![image](https://user-images.githubusercontent.com/84390820/126747596-ce38bcf0-01d1-4d4d-acef-b4e2973595ea.png)

* Implemente el circuito equivalente de Thévenin, agregue el resistor R5 y mida la
corriente y el voltaje en el mismo, anote los resultados en la tabla 5.2.

![image](https://user-images.githubusercontent.com/84390820/126751743-28c3be5c-9fbb-4319-b271-61911422ce7d.png)

Calculamos el voltaje de R5 en el circuito equivalente de Thévenin:

Utilizamos el divisor de corriente: Vx = (VTH/Req) * Rx = ( 5.056/1298.85) * 1000 = 3.88 V 

Calculamos tambien la intensidad: ITH = VTH / RTH = 5.05/ 1298.85 = 3.88 mA 
![image](https://user-images.githubusercontent.com/84390820/126747627-098cbb3e-3ba4-45ab-9245-6e78ff7c432d.png)

![image](https://user-images.githubusercontent.com/84390820/126747676-fd82cd0a-3bc5-497a-8a55-8605dae5255b.png)

5. VIDEO

6. CONCLUSIONES

*	El teorema de Thévenin establece que cualquier circuito complejo de corriente directa pueda ser reemplazada por un circuito equivalente que conste de una fuente de voltaje y un resistor en serie.

* La práctica de laboratorio abarca todos los temas teóricos de capítulos anteriores como ley de nodos, ley de mallas, ley de ohm, por lo que es necesario tener estos conocimientos desarrollados para poder realizar los cálculos del teorema de Thévenin. 

7. BIBLIOGRAFÍA

- Wikipedia. (16 de Enero de 2021). Teorema de Thevenin. Obtenido de https://es.wikipedia.org/wiki/Teorema_de_Th%C3%A9venin

- Xnomind. (7 de Noviembre de 2019). TEOREMA. Obtenido de TEOREMA DE THEVENIN EXPLICADO PARA QUE LO ENTIENDAS: https://www.teorema.top/teorema-de-thevenin/
