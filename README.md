# Proyecto Final Biofísica II: Analizador de energía eléctrica. 

INTRODUCCIÓN

Según datos reportados por la Compañía Administradora del Mercado Mayorista Eléctrico (CAMMESA), el consumo de electricidad nacional aumentó en marzo del corriente 
año un 28,6 % en relación con el mismo mes del 2022. Más precisamente, el 13 de marzo a las 15:28 hs, se registró la demanda de potencia instantánea más alta de la 
historia, 29.105 MW. A pesar de este particular incremento, la demanda de energía eléctrica está aumentando progresivamente desde 1992. Si a dicha problemática 
adicionamos el hecho de que la energía eléctrica a nivel mundial se genera principalmente a partir de combustibles fósiles, una fuente de energía no renovable en 
tiempos humanos, el asunto se torna de suma relevancia. Por lo tanto, consideramos que conocer el consumo de energía eléctrica de nuestra red domiciliaria así como también de la red universitaria, constituye una herramienta indispensable para hacer un uso responsable del recurso.

En este contexto se enmarca el presente proyecto final, el cual contempla como objetivo principal de trabajo el diseño y construcción de un analizador de energía 
eléctrica, dispositivo que permitirá realizar mediciones de corriente y tensión en una red eléctrica doméstica y/o universitaria. En base a dichos parámetros, se 
estimará la energía demandada en un determinado período de tiempo, la potencia activa, y los grados de desfasaje entre la corriente y el voltaje con el objetivo de 
evaluar la potencia reactiva producida en el circuito en estudio. Para llevar a cabo las mediciones de corriente, se utilizará un sensor no invasivo tipo pinza.
Por otro lado, se propone como objetivo secundario aprender a programar el microcontrolador ESP32 desde la IDE de Arduino para registrar en una planilla o 
aplicación los valores de las mediciones tomadas por el analizador de energía eléctrica a través de una red Wi-Fi. De esta forma, se podrá acceder a los datos 
para su posterior análisis desde cualquier dispositivo conectado a Internet.     

Conceptos de la materia a aplicar en este proyecto: 

En el desarrollo de este trabajo se aplican conceptos de corriente eléctrica y potencial eléctrico, Ley de Ampere, circuitos de corriente alterna e induccón electromagnética. Además, se profundiza en el uso de placas programables para la medición y monitoreo de parámetros eléctricos. 

DIAGRAMA DE TAREAS 


Viernes 9:	Diseño del circuito. Descarga e instalación del soporte de Arduino para programar el microcontrolador ESP32. 

Miércoles 14:	Armado del circuito y carga del código para ESP32.

Viernes 16:	Prueba de medición y procesamiento de los datos.

Miércoles 21:	Demostración.


MATERIALES 


Microcontrolador ESP32

Sensor tipo pinza SCT013 (10 A/1 V)

Tablero breadboard

Resistencias

Adaptador para ESP32


DESARROYO DEL TRABAJO 


En primer lugar, se procede con la instalación del soporte de Arduino-ESP32 con el objetivo de utilizar la IDE de Arduino para programar el microcontrolador. Para
ello, se sugiere el empleo de un instructivo encontrado en el repositorio de GitHub, cuyo link se detalla a continuación: 
https://docs.espressif.com/projects/arduinoesp32/en/latest/installing.html. 

Posteriormente, se cargan a la memoria del microcontrolador ESP32 dos programas informáticos. Uno de ellos permitirá subir los valores de las mediciones 
registradas por el analizador de energía eléctrica directamente a la web, mientras que el otro posibilitará asignarle una fecha y hora a cada dato medido en base 
al registro del tiempo obtenido a partir de Internet. Ambos códigos se detallan en el archivo "ProyectoOliySofi".

Las mediciones obtenidas se registrarán conforme transcurra el tiempo en una planilla creada a partir de un script de Java utilizando la extensión de Googlesheet 
AppScript. A continuación se describe el ID de implementación y una aplicación web asociada al ID.                                                                  
ID de implementación: AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI                                                             
Aplicación Web: https://script.google.com/macros/s/AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI/exec

Para  cargar datos en nuestra planilla utilizamos el siguiente enlace: https://script.google.com/macros/s/AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI/exec?hora=1/1/2023/11:23;07&corriente=5&voltaje=220 

Link para acceso a la planilla: https://docs.google.com/spreadsheets/d/1xOkNwPYBVjeUegbSmnY7YPKFOHt2uWFZYH9q6XaOhpw/edit?usp=sharing

Nota: Los códigos utilizados en el presente proyecto representan versiones modificadas de programas expuestos en el Trabajo Práctico "Parece que va a llover", cuyo 
autor es el profesor Raúl Righini. 




