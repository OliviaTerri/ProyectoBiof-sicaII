# Trabajo Final Biofísica II: analizador de energía. 

Introducción/Objetivos

El objetivo principal del trabajo es diseñar y construir un dispositivo que permita realizar mediciones de corriente y tensión 
en una red eléctrica doméstica, parámetros mediante los cuales se estimarán la energía demandada en cierto período de tiempo en el 
domicilio, la potencia activa, y los grados de desfasaje entre la corriente y el voltaje para evaluar la potencia reactiva preoducida
en el circuito. Se utilizará un sensor no invasivo tipo pinza.
Como un segundo objetivo, proponemos lograr que la información obtenida por el dispositivo sea registrada on-line de 
manera que nos permita visualizar y trabajar con los datos en una computadora con conexión a internet.
Si bien la idea original del proyecto plantea el uso de Arduino, para llevar a cabo ambos objetivos utilizaremos el microcontrolador ESP32 (programado desde la IDE de Arduino). 

Diagrama de tareas 

Viernes 9:	Diseño del circuito. Diseño de carcasa para el dispositivo. Descarga e instalación del soporte de Arduino
para ESP32. 

Miércoles 14:	Armado del circuito y programación del código para ESP32.

Viernes 16:	Prueba de medición y procesamiento de los datos.

Miércoles 21:	Demostración.

Materiales 

Microcontrolador ESP32

Sensor tipo pinza

Tablero breadboard

Desarrollo del trabajo 

Comenzamos instalando el soporte de Arduino-ESP32 para poder utilizar la IDE de Arduino para programar nuestro microcontrolador. Para
ello seguimos el instructivo encontrado en el repositorio de Github (https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html). 

Utilizaremos un programa para obtener la fecha y hora de internet y otro para subir los datos registrados a la web. Se encuentran en el archivo "ProyectoOliySofi".

Para poder subir los datos a la web, preparamos una planilla donde se registrarán los datos obtenidos implementando un script de Java utilizando la extensión de Googlesheet AppScript. Se registran a continuación el ID de implementación y una aplicación web asociada al ID. 
ID de implementación: AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI
Aplicación Web: https://script.google.com/macros/s/AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI/exec

Para poder acceder a nuestra planilla utilizamos el siguiente enlace: https://script.google.com/macros/s/AKfycbwnw09FeCX5xv4po2xRdoj9u69zH97BtmXUJV-VXfmh9ccMUu0Srlv4gsfdqkxJJMI/exec?hora=1/1/2023/11:23;07&corriente=5&voltaje=220 

Nota: Los códigos utilizados en la sección anterior son versiones modificadas de los presentados en el Trabajo Práctico "Parece que va a llover" del Profesor Raul Righini. 




