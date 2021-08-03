DOCKER CLOUD :stars: 
---
1. Repaso 
Durante el repaso se tocaron temas vistos en otras sesiones como:
- Contenedores
- imágenes
Durante la clase también se vio como compartir las imágenes y automatizar el proceso con github 
2. Docker Cloud
Para Docker cloud trabajaremos con archivos de Docker compose  con el cual configuraremos nuestro contenedor o contenedores, en este caso vimos como replicar un contenedor con el siguiente comando 
>docker-compose up --scale web=5

Información importante:
version: '3' -> La versión que se está utilizando, suele ser la última

>services: -> Exísten dos servicios

>web -> servicio #1 (Servicio web) image: dockercloud/hello-world

>lb: -> Servicio #2 (Load balance) image: dockercloud/haproxy

>links: - web

>volumes: -> Docker de comunicación entre los dos servicios - /var/run/docker.sock:/var/run/docker.sock ports: -> Puerto donde estará ubicado el servicio - 80:80

3. Instalación de Jenkis 
Jenkins es una herramienta de automatización, para su instalación primero clonamos el repositorio con el siguiente comando 
>git clone https://github.com/jsgiraldoh/Jenkins.git

Luego ejecutamos los permisos a Jenkins con el siguiente comando 
>	sudo chown "usuario":"usuario" jenkins_home

Luego corremos el contenedor con el siguiente comando 
>	docker-compose -f docker-compose-jenkins.yml up -d

La clave de Jenkins la podemos ver con el siguiente comando 
>	docker logs -f jenkins

con esto se levanta el servidor de Jenkins ahora debemos ir al navegador y seguir el proceso de configuración instalando complementos etc.
