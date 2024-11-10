# FLows de NODE-Red

## Introducción

![Node-RED Logo](https://nodered.org/about/resources/media/node-red-icon-2.png)

Bienvenido a la página de información. Aquí encontrarás detalles importantes sobre nuestro proyecto.

Node-RED es una herramienta de código abierto desarrollada inicialmente por IBM y que, estando orientada a flujos de datos, proporciona mecanismos para asociar dispositivos hardware, APIs y servicios online dentro de un ecosistema IoT. Node-RED es una herramienta gráfica, utilizable desde cualquier navegador web, que permite la cración y edición de flujos de datos que tomen datos de entrada (mediante nodos de entrada), los procesen (mediante nodos de procesamiento) y proporcionen salidas (mediante nodos de salida). Todos los elementos, incluyendo flujos complejos definidos por el usuario, pueden almacenarse en formato JSON para ser importados a continuación en otras instalaciones. Node-RED permite la interconexión de elementos software y hardware mediante virtualmente cualquier protocolo conocido, facilitando el despliegue de infraestructuras IoT, y esta condición permite definir flujos de servicios a través de protocolos como el MQTT.

Node-RED es una herramienta de programación visual que se implementa en dispositivos controladores de hardware. Trabaja mostrando de manera visual las relaciones y funciones de manera que se pueda programar sin escribir. Es un panel de flow al que se pueden incorporar nodos que se comuniquen entre ellos y puede instalarse en equipos como ordenadores Windows, Linux, o en servidores en la nube.

## Contenido

- [Descripción del Proyecto](#descripción-del-proyecto)
- [Instalación](#instalación)
- [Uso](#uso)
- [Licencia](#licencia)

## Descripción del Proyecto

Previamente realizaremos una pequeña investigación:

1. ¿Qué es MQTT?
2. ¿Actualmente, en qué casos se usan sistemas distribuidos?
3. ¿Qué es NODE-RED y para qué sirve?
4. Diferencias entre Software Open Source y Software de Licencia
5. Investigue y analice el patrón productor/consumidor o publicador/subscriptor, explique brevemente cómo se aplica este patrón en los sistemas distribuidos.
6. Enumere y explique brevemente los componentes del protocolo MQTT en el patrón publicador/subscriptor
7. ¿En qué tecnologías se usa actualmente el protocolo MQTT?
8. Realice un cuadro comparativo de las características, ventajas y desventajas de Apache Zookeeper, MQTT y Apache Kafka.

Realizaremos cuatro (4) ejercicios:

1. Transmitiendo mensajes a través de un nodo Injection
2. Tratamiento de información desde fuentes externas
3. Bifurcaciones en flujos de trabajo
4. Función básica

## Instalación

Para hacer uso de la herramienta puedes seguir las instrucciones a conitnuación:

### Para Windows

[Instrucciones de instalación para Windows](https://nodered-org.translate.goog/docs/getting-started/windows?_x_tr_sl=auto&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=wapp)

### Para wsl(linux) en windows

[Cómo instalar Ubuntu con Windows WSL (subsystem) for Linux en Windows 10](https://youtu.be/lt4UtlUzx9w?si=MpnBuwCGLnXHUq5U)

### Para Linux

Las presentes instrucciones son válidas para cualquier distribución basada en Debian (incluida Ubuntu). Para otras distribuciones o sistemas operativos, consultad la documentación oficial de Node-RED.

Para instalar Node-RED en la máquina virtual del curso, es suficiente con seguir los siguientes pasos.

En primer lugar, si no lo están ya, instala los requisitos básicos del paquete:

sudo apt install build-essential git curl
La siguiente línea descarga y ejecuta un script que realizará toda la instalación de dependencias (desinstalando versiones antiguas si es necesario) por ti:

bash <(curl -sL <https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered>)

Para ejecutar Node-RED, una vez instalado, es posible utilizar la orden node-red-start desde cualquier terminal. Para detener el proceso, es suficiente con utilizar Ctrl-C:

$ node-red

![pantalla nodered](https://www.dropbox.com/scl/fi/it1qou8ash5fcsg5la35x/pantallanodered.png?rlkey=ykz5iulvodhq9rryo2cn107hh&st=9fpmj1qg&dl=0)

Tras arrancarlo, observarás cuatro áreas en el editor:

Barra principal, en la parte superior, con los botones Deploy y de Menú principal.

Panel de nodos, en la parte izquierda, que proporciona acceso directo a todos los nodos disponibles en Node-RED. Es posible instalar nuevos nodos a través de la Paleta de Nodos, disponible a través del menú principal (Manage Palette). Estos nodos pueden ser arrastrados al editor para conformar nuevos flujos de datos.

Panel de edición o espacio de trabajo, en la parte central de la pantalla, donde podrás arrastrar y unir nuevos nodos. Es posible crear nuevos flujos en pestañas independientes.

Panel de información, en la parte derecha de la pantalla, donde destaca el botón Debug, mediante el cual veremos la salida de los nodos de tipo Debug en nuestros flujos.

[Cómo instalar y ejecutar Node-RED en linux Ubuntu o Debian](https://nodered-org.translate.goog/docs/getting-started/local?_x_tr_sl=auto&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=wapp)

## Uso

Familiarizarse con la herramienta Node-RED para gestión de flujos, que será utilizada durante el resto de prácticas como herramienta rápida de despliegue de aplicaciones IoT.
Desarrollar esquemas básicos de sistemas cliente/servidor TCP y UDP utilizando Node-RED

1. [Flow 1](https://www.notion.so/First-Flow-137995b1451680d98b4fd7c8ad1d6002?pvs=4)
2. [Flow 2](https://www.notion.so/Second-Flow-137995b14516809a972fc14def3c7c4f?pvs=4)
3. [Flow 3](https://www.notion.so/Third-Flow-137995b14516803aa74ed35a9c653fd8?pvs=4)
4. [Flow 4](https://www.notion.so/Fourth-Flow-137995b145168015ab7ae829382fe7d1?pvs=4)
5. [Flow 5](https://youtu.be/wS0E1j1q7sM?si=EaWZIixL5dx5nszF)

## Información Adicional

[Editor Components](https://youtu.be/veiNb6Y0ERg?si=zLDJaqShsJOOwbci)

[Lista de Reproducción Node-Red Essentials](https://youtube.com/playlist?list=PLyNBB9VCLmo1hyO-4fIZ08gqFcXBkHy-6&si=xOXSCtVVbARfrMG5)

[Free Udemy Course about Node-RED](https://www.udemy.com/course/proyecto-node-red-monitorizacion-de-parametros-del-sistema/?utm_source=adwords&utm_medium=udemyads&utm_campaign=Search_DSA_GammaCatchall_NonP_la.ES_cc.ROW-Spanish&campaigntype=Search&portfolio=ROW-Spanish&language=ES&product=Course&test=&audience=DSA&topic=&priority=Gamma&utm_content=deal4584&utm_term=_._ag_167955697191_._ad_706510832613_._kw__._de_c_._dm__._pl__._ti_dsa-1456167871416_._li_1005493_._pd__._&matchtype=&gad_source=1&gclid=Cj0KCQiA57G5BhDUARIsACgCYnwjjReoqhcOGedAfy6QDDNKh0FMHsByYmsFU24DOsyluC8RW2asunMaAlN6EALw_wcB)

## Licencia

## Licencia



© [2024] [Georgelys Marcano]. Todos los derechos reservados.
