---
title: "Conociendo lo que está Detrás de un Desarrollador de Back-End"

subtitle: "Aprenda aquí todo sobre el desarrollo web de Back-End y lo que se necesita para convertirse en Desarrollador de Back-End"

cover: "https://ucarecdn.com/98208ebb-dcb3-4e40-9ae4-4ec886213f97/"

textColor: "white"
date: "2018-05-11"
tags: ["back-end","cliente-servidor"]
---

## El Lado de Back-End de la Web

No hace mucho tiempo, los navegadores eran muy tontos. Todo lo que hicieron fue renderizar documentos HTML en una versión muy temprana de HTML. No había CSS, ni JS. Eso significa que los desarrolladores web front-end no existían!

Todo el trabajo fue realizado por el servidor: como no había JavaScript, el DOM no pudo ~~ser~~ actualizado durante el tiempo de ejecución del sitio web. Eso significa que el código fuente HTML inicial que recibió el navegador al cargar el sitio web también sería la última versión del mismo. **No DOM modifications**.

### La Arquitectura del Cliente-Servidor
***

[Recuerdas como funciona el internet?](https://www.youtube.com/watch?v=UiBT3Kj8KBM) Cada dominio apunta a una única dirección IP / servidor, y ese servidor está listo para devolver una **respuesta de texto** a cualquier solicitud HTTP que provenga de cualquier cliente.

**Piense en el servidor como un "generador de documentos".** Puede ser una imagen, un video, un documento de texto, JSON, HTML, CSS, etc.  La responsabilidad del servidor es responder con el contenido que el cliente le solicite en cada momento.

![backend developer](https://ucarecdn.com/2c0000ef-2907-43cb-80ed-2ba4f194b83e/)

Junto con el contenido del documento generado, el servidor también puede especificar qué tipo de contenido está respondiendo, lo que permite que el navegador lea e interprete la respuesta de manera precisa. Los formatos de respuesta disponibles pueden ser cientos, pero estos son los más comunes:

### Respuestas del Servidor Content-Types

|**Content-type**   |**Descripción**   |
|:------------------|:-----------------|
|text/plain          |Este es el valor predeterminado para los archivos de texto. Incluso si realmente significa un archivo de texto desconocido, los navegadores asumen que pueden mostrarlo    |
|text/css      |Cualquier archivo CSS que deba interpretarse como tal en una página web debe ser un archivo de texto / css. A menudo, los servidores no reconocen archivos con el sufijo .css como archivos CSS y en su lugar los envían como texto / plano.      |
|text/html        |Todo el contenido HTML debe ser creado con este tipo.    |
|image/gif<br>image/jpeg<br>image/png<br>image/svg+xml     |Solo algunos tipos de imágenes son ampliamente reconocidos y se consideran seguros para la web (listos para usar en una página web).  |
|audio/wav<br>audio/mpeg     |Para archivos de auidio .wav .mp3    |
|multipart/form-data     |Los tipo multipart/form-data pueden ser usados cuando se envia el contenido completo de un formulario HTML desde un navegador al servidor.    |
|application/json     |Una respuesta en formato JSON    |

Además del contenido del documento y del content-type, el servidor también agrega un código de respuesta al encabezado. Hay docenas de códigos de respuesta, pero estos son los más populares:

#### Codigos de Respuesta del Servidor

|**Content-type**   |**Descripción**   |
|:------------------|:-----------------|
|2xx Success      |200 OK, 201 Creado, 204 No hay Contenido, 203 Información no autorizada  |
|3xx Redirection    |301 Movido Permanentemente, 307 Redirecionado Temporalmente, 304 No Modificado    |
|4xx Client Error    |404 No Encontrado, 400 Mala Solicitud, 403 Prohibido, 401 Sin Autorización    |
|5xx Server Error     |500 Error Interno del Servidor, 503 Servicio No Disponible    |


[[info]]
|:link: Aquí puedes encontrar información más detallada sobre [Codigos de Respuesta del Servidor.](https://www.restapitutorial.com/httpstatuscodes.html)

### El Rol del Lenguaje Back-End
***

Lo bueno de un lenguaje de back-end es que se ejecuta en una máquina real (no en un navegador como el lenguaje de front-end). Con un lenguaje de fondo puedes hacer cosas como:

+ Generar Documentos PDF’s, Word or Excel.
+ Conectate a una o varias bases de datos al mismo tiempo y recupera / procesa los datos.
+ Transmitir video y archivos de audio.
+ Abre / Crea / elimina archivos locales de la máquina y actualizalos con contenido nuevo.
+ Comprimir imágenes, videos o cualquier tipo de archivo.
+ Accede a cualquier programa instalado en la máquina local y utilizalo para un sitio web (por ejemplo, puede abrir el programa zip y extraer un archivo zip).
+ Puedes interactuar con cualquier hardware conectado al servidor principal (como una máquina expendedora, un lector de huellas digitales, googles de realidad virtual, un lector de tarjetas de crédito, etc.).
+ Puedes combinar cualquiera de las operaciones ya mencionadas en tu propio flujo de aplicaciones de back-end.
  
###  Entonces.. qué hace un desarrollador Web de Back-End?
***

Como desarrollador de Back-End, deberá escribir todo el código para generar y / o responder a esos documentos estáticos y dinámicos según lo soliciten los clientes.

El código de un desarrollador web de back-end debe cumplir con 4 requisitos principales:

+ **Recibir y procesar las solicitudes de los clientes:** Entender lo que el cliente está solicitando, validar los datos ingresados (parámetros), rechazar posibles violaciones de seguridad.
+ **Trabaja con la data:** Obten lo que necesites de la base de datos, actualiza lo que necesitas de la base de datos.
+ **Desarrolla y ejecuta la parte lógica de las necesidades comerciales:** Conectate con aplicaciones de terceros, hardware externo y cualquier otra necesidad comercial.
+ **Responde al cliente:** Prepara la respuesta en el formato adecuado y envíala al cliente.




