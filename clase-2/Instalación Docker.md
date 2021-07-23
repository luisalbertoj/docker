Instalación Docker
===
En esta sesión se realizó la instalacion de Docker y Docker Compose:

>1. Instalación Docker Para la instalación de docker se necesita una variante de Linux, y entrar a su terminal, luego se siguieron los pasos del siguiente link. [instalacion de docker](https://docs.docker.com/engine/install/ubuntu/)
---
>2. En caso de que se tenga el sistema operativo seleccionado en una maquina virtual y esta no te dé la posibilidad de copiar, la mejor recomendación es descargar un programa que te permita esa función. Para esta clase se descargó Mobaxterm. [link de descarga](https://mobaxterm.mobatek.net/)
---
>3. Para poder ejecutar mobaxterm tenemos que actualizar la maquina virtual con el comando:

> > > **sudo apt-get update**
---
>4. luego instalamos el cliente ssh con el comando 

> > > **sudo apt-get install openssh-server**
---
>5. Luego buscamos la ip con el comando:

> > > **ip a s**
---
>6. Vamos al mobaxterm y ponemos nuestra ip con el siguiente comando:

> > > **ssh 192.168.1.104 -l "usuario"**
---
>7. Cuando ya se conecte con la terminar de nuestro sistema Linux ya procedemos con los pasos del link [instalacion de docker](https://docs.docker.com/engine/install/ubuntu/)
---
>8. Instalación Docker Compose Para la instalación de Dcoker compose nos encontramos en la terminar de linux nuevamente y seguimos los pasos que se encuentran en el siguiente link. [instalacion de docker compose](https://docs.docker.com/engine/install/ubuntu/)