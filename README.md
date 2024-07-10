<h1>BAOFONGhz (TM)</h1>

Requisitos mínimos
---

-Una radio, para utilizar de estación

-Cables de audio, para conectar los jack

-Un dispositivo que ejecute Java

-Conexión a internet

-Conocimientos mínimos en redes


Instrucciones de Ejecución version 0.3.11072024 Beta
---

Descargar: https://github.com/ourenseko/BAOFONGhz/blob/main/BAOFONGhz/dist/BAOFONGhz.jar
 

Instrucciones de Ejecución version 0.2.10072024 Alpha
---

UPDAPTED.

![image](https://github.com/ourenseko/BAOFONGhz/assets/25538565/db09cb01-b0ea-49e3-95cf-873e0fa551a8)



Instrucciones de Ejecución version 0.1 Alpha
---
Compilar los programas: Abre una terminal (o símbolo del sistema) y compila los archivos .java:

(sh - Copy code)
 javac VoiceChatServer.java VoiceChatClient.java

Ejecutar el servidor: En la computadora que actuará como servidor, ejecuta:

(sh - Copy code)
 java VoiceChatServer

Ejecutar el cliente: En la computadora que actuará como cliente, ejecuta:

(sh - Copy code)
 java VoiceChatClient

Asegúrate de que el cliente tenga la dirección IP correcta del servidor. Puedes cambiar 127.0.0.1 en VoiceChatClient.java por la IP real del servidor. Para probar el sistema con una conexión a internet simplemente usar las IPs locales que asigna el router a cada dispositivo y abrir los puertos en el SO (Windows con seguridad avanzada)



Nota:
Ambos programas usan el puerto 12345. Asegúrate de que este puerto esté abierto en ambas computadoras y no esté bloqueado por ningún firewall.
Este ejemplo es bastante básico y no incluye manejo de errores robusto ni cifrado. Para un entorno de producción, se deben considerar más medidas de seguridad y gestión de errores.
La calidad de la transmisión puede variar dependiendo de la red y las capacidades de hardware de las computadoras involucradas.




GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007

 Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.

(...)



Configuración principal de hardware y software 
---

En ordenadores portatiles y teléfonos (necesitas que pueda ejecutar Java) puede ser necesario un adaptador para bifurcar microfono y altavoz además de un reductor del jack 3.5mm a 2.5mm

Conecta el microfono y parlante en los puertos jack respectivamente, activa el modo VOX 1 de tu emisora y sube el volumen al máximo.

Sintoniza una frecuencia silenciosa (legal) o repetidor dedicado en el que va a operar la estación local

El servidor necesita tener una IP estática o usar un servicio noIP para mantener la conexión

En el firewall del router o teléfono (datos) redirecciona el puerto 1234 local al 8080 exterior (o asigna el que veas conveniente)

Nota: Es necesario que tu IPS te probeéa de una IP unica (variable ó fija) y no formes parte de una red para ahorrar matriculas IP, de lo contrario el servicio de broadcast (Emitir) es probable que no funcione para tí al no poder identificarte y conectarse con tu computadora. Solo podrás escuchar.
