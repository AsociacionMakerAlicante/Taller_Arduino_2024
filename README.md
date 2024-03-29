# Taller Arduino 2024 
<ins><b>Aprende a manejar tu Arduino desde el móvil.</b></ins>

En el curso se explicarán dos códigos de ejemplo. Uno para una placa de Arduino UNO y otro para un ESP32. Aunque en los ejemplos se utilizan estas placas el código es facilmente exportable a cualquier otra placa.

Tambien se explica el código generado para la APP instalada en el móvil. Se ha utilizado "APP inventor" para generar la aplicación. Se dejan tres enlaces para descargar el código de los tres ejemplos.

- Código para un Arduino UNO utilizando un módulo bluetooth. [Descargar código](https://github.com/AsociacionMakerAlicante/Taller_Arduino_2024/raw/main/Ejemplos/Control_Movil.zip)

- Enlace a repositorio GitHub para descargar ejemplo de código para un ESP32. [AQUÍ](https://github.com/Ricardo1366/ESP32_ControlMovil)

- Código para APP inventor. [Descarga del ejemplo](https://github.com/AsociacionMakerAlicante/Taller_Arduino_2024/raw/main/Ejemplos/ControlMovil.aia)
  

### Descripción de los programas
<ins><b>Código para Arduino</b></ins>

El código de Arduino consta de una función encargada de detectar cuando se recibe un envío de datos vía bluetooth y separar la cadena recibida en los distintos comandos.

La cadena utiliza el caracter "," (coma) como separador. La estructura de la misma es "Comando 1","Comando 2", ... , "Comando N".

El programa tiene tres funciones predefinidas y mediante la cadena enviada por bluetooth se esjecutará la función indicada tomando como parámetros los valores enviados. Las tres funciones son:

1. __Blink.__
   
   Hace parpadear el led interno de la placa un número determinado de veces controlando el tiempo que permacece encendido y el que permanece apagado (en milisegundos). Necesita tres parámetros. A) Tiempo encendido. B) Tiempo apagado. C) Número de repeticiones.
3. __Encender.__
   
   Enciende el led de forma fija. No necesita parámetros.
5. __Apagar.__
   
   Apaga el led. No necesita parámetros.

<ins><b>Código para el móvil</b></ins>

La APP del móvil consta de una lista desplegable con las funciones implementadas en Arduino y tres campos para que el usuario informe el valor de los distintos parámetro.

La APP se ha desarrollado con APP inventor. Este software permite correr aplicaciones en móviles Android y IOS. Existen dos formas de hacer funcionar la APP en el móvil. La primera consiste en ejecutar APP inventor en el móvil y mediante un código QR cargar la aplicación. 

La segunda es generando un fichero de instalación ".apk". Aunque al no venir de una tienda de Android necesitarás configurar tu teléfono para que te permita instalar aplicaciones de "Fuentes desconocidas".

Si tu móvil es IOS solo tendrás disponible la primera opción.

![](https://github.com/AsociacionMakerAlicante/Taller_Arduino_2024/blob/main/Imagenes/Logo%20Maker%20redondo%20(Electronica).jfif)
