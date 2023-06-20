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


En primer lugar, se procedió con la instalación del soporte de Arduino-ESP32 con el objetivo de utilizar la IDE de Arduino para programar el microcontrolador. Para
ello, se empleó un instructivo encontrado en el repositorio de GitHub, cuyo link se detalla a continuación: 
https://docs.espressif.com/projects/arduinoesp32/en/latest/installing.html. 

Utilizaremos un programa para obtener la fecha y hora de internet y otro para subir los datos registrados a la web. Se encuentran en el archivo "ProyectoOliySofi".

Para poder subir los datos a la web, preparamos una planilla donde se registrarán los datos obtenidos implementando un script de Java utilizando la extensión de Googlesheet AppScript. Se registran a continuación el ID de implementación y una aplicación web asociada al ID. 
ID de implementación: AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI
Aplicación Web: https://script.google.com/macros/s/AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI/exec

Para  cargar datos en nuestra planilla utilizamos el siguiente enlace: https://script.google.com/macros/s/AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI/exec?hora=1/1/2023/11:23;07&corriente=5&voltaje=220 

Link para acceso a la planilla: https://docs.google.com/spreadsheets/d/1xOkNwPYBVjeUegbSmnY7YPKFOHt2uWFZYH9q6XaOhpw/edit?usp=sharing

Nota: Los códigos utilizados en la sección anterior son versiones modificadas de los presentados en el Trabajo Práctico "Parece que va a llover" del Profesor Raul 
Righini. 




