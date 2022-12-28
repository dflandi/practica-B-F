# practica-B-F

Pasos de pratica sobre despliegue_app

![image](https://user-images.githubusercontent.com/91167254/209740558-7285d96b-a9f4-4b95-9699-f78011157d44.png)

Paso 1:

Colocamos el comando vi docker-compose.yml para verificar el codigo que copiamos, para salir ponemos la tecla ESC : y escribimos wq 

![1](https://user-images.githubusercontent.com/91167254/209740654-3812ffae-0bd2-4139-85fc-5a702a46cf97.png)

Paso 2:

Para ver los contenedores que tenemos colocamos el comando docker ps

![image](https://user-images.githubusercontent.com/91167254/209740818-451273ae-14c8-447d-b775-c220981f40ee.png)

Paso 3:

Ponemos el comando cat docker-compose.yml

![image](https://user-images.githubusercontent.com/91167254/209740897-57241ce5-fbd0-4904-9018-bfe9ccaa7628.png)

Paso 4:

Ponemmos el comando docker-compose up -d sirve para descargar las librerias.

![image](https://user-images.githubusercontent.com/91167254/209740958-54f41e4f-5193-41ed-a310-cd417513862b.png)

Paso 5: 

Clonamos el repositorio con (git clone https://github.com/maguaman2/tendencias-mar22-security


![image](https://user-images.githubusercontent.com/91167254/209741117-ad626fad-4cf8-4e1b-8cc4-f92f70a070ac.png)


Paso 6:
 
Ponemos el comando  ls para ver los directorios que tenemos.

![image](https://user-images.githubusercontent.com/91167254/209741197-bfce7858-47fa-4c3b-be93-63927014c6e0.png)

Paso 7:

Creamos un documento llamado Dockerfile con el comando vi Dockerfile

![image](https://user-images.githubusercontent.com/91167254/209741425-ac0a1b72-da89-4892-82fd-1e84c1a593e1.png)


Paso 8:

Ponemos el comando docker build -t myapp 


![image](https://user-images.githubusercontent.com/91167254/209741552-374284b4-599b-4fc7-8ff0-daf4d61b5720.png)

Paso 9 :

Ponemos el comando docker run -d --network db_default -p 8081:8081 myapp

![image](https://user-images.githubusercontent.com/91167254/209741725-856610b9-3d5f-4edd-aa43-90d8c25c9e71.png)



Paso 10:

Verificamos en localhost:/users y nos deberia salir la siguiente tabla:

![image](https://user-images.githubusercontent.com/91167254/209741779-1c083705-6a94-4dc5-a2f3-e74ad732ade4.png)

DESPLIEGUE FRONTEND

Vamos a la carpeta local y colocamos lo siguiente el comando git clone git clone https://github.com/maguaman2/securityfe 

![image](https://user-images.githubusercontent.com/91167254/209742017-a86b145c-cb29-4103-bbcd-2e1670e641e2.png)


Entramos en el nuevo gitclone y creamos un vi Dockerfile

![image](https://user-images.githubusercontent.com/91167254/209742145-d9610d96-0244-4304-939f-bd0f608cecef.png)


Ponemos el comando docker build -t myappfe:latest para crear una imagen

![image](https://user-images.githubusercontent.com/91167254/209742243-9a135213-174f-4ee0-a349-a4e3774ebfd4.png)
