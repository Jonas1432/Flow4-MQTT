# -flow3-NodeRed-

Este repositorio contiene el flow 4 del curso de NodeRed, visto en en los contenidos de Internet de las cosas de Codigo IoT en edu.codigoiot.com MQTT

## Introducción 

Este flow consiste en un tablero que presente la información de temperatura y humedad locales. Este flow recibe la información por MQTT con un broker local.

# Referencias 

En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com 

## ||Material Necesario||

- [Ubuntu 20.04](https://releases.ubuntu.com/20.04/)
- [NodeJS](https://nodejs.org/es/)
    - [NPM](https://www.npmjs.com/)
    - [NodeRed](https://nodered.org/docs/getting-started/local)
    - [Nodos Dashboard](https://flows.nodered.org/node/node-red-dashboard)
    - [Mosquito](https://mosquitto.org/)

##  Instrucciones

### Requisitos previos
Para que este flow funcione, debes cumplir con los siguientes requisitos previos

1. Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna versión LTS. Al momento de creación de este documento, se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM
2. Instalación de NodeRed. La instalación se realiza por NPM. Al momento de la creación de este contenido, se usó la versión 3.0.2
3. Instalar los nodos node-red-dashboard. Para ello, dirigete a la opcion "Manage Palet" de NodeRed y en la pestaña Install busca node-red-dashboard. Finalmente haz clic en instalar.
4. Instalación de Broker local Mosquitto MQTT.

### Instrucciones de preparación del entorno
Para ejecutar este flow, es necesario lo siguiente

1. Arrancar NodeRed con el comando node-red
2. Importar el flow del repositorio
3. Hacer clic en el boton Deploy

### Instrucciones de operación

- Para observar el resutlado de este flow, abre un navegador y dirígete a localhost:1880/ui
- Enviar por MQTT un mensaje que contenga un JSON con las variables ID, temp y hum
Notas
* Este Flow se suscribe al tema codigoIoT/Mor/mqtt/flow4
* El mensaje mqtt usado para probar este flow es mosquitto_pub -h localhost -t codigoIoT/Mor/mqtt/flow4 -m '{"ID":"Jonathan Jesus","temp":21,"hum":74}'
* Para que la gráfica historica muestre información, deben enviarse al menos 2 puntos

## [Resultado]

![](https://github.com/Jonas1432/-flow3-NodeRed-/blob/main/Resultado-Flow3.png)

# Créditos

* Desarrollado por Jonathan Araujo
* https://github.com/Jonas1432