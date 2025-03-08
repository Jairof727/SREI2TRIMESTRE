Creamos la VPC
![image](https://github.com/user-attachments/assets/47848a4b-686a-4cad-9494-047aa3bb9008)
![image](https://github.com/user-attachments/assets/4802de53-3127-4622-a009-8837f466de39)
![image](https://github.com/user-attachments/assets/110916b1-2274-49fe-b2ea-d2343c1fd05d)
Ya tenemos la VPC
![image](https://github.com/user-attachments/assets/6dca2002-f055-48f8-b103-cc943c41509e)

Ahora vamos a lanzar una instancia
![image](https://github.com/user-attachments/assets/b4901196-d8ac-4a62-9d52-26311e9ad298)
![image](https://github.com/user-attachments/assets/4c46e9c6-70eb-4c00-8b5f-f2988e338823)
Ahora creamos un nuevo grupo de seguridad
![image](https://github.com/user-attachments/assets/fa0c12e5-dc96-4894-a78e-37d06c3b85b8)
![image](https://github.com/user-attachments/assets/c491e6c0-bd8e-48f3-9229-14c3ab13ef4e)

Ahora nos conectamos con putty y como podemos ver no tenemos problemas
![image](https://github.com/user-attachments/assets/c6899e4b-666b-4b4f-bcba-cc75ab72354e)

Vamos a instalar apache y php usando los siguientes comandos
sudo apt update
sudo apt install apache2
sudo systemctl start apache2 (Para arrancar el servidor.)
sudo systemctl enable apache2 (para que apache inicie cada vez que arranca la instancia.)
Ya vemos apache instalado
![image](https://github.com/user-attachments/assets/ba9a7f93-987c-451a-a120-cb3cc471ae31)

Pasamos a instalar php
Confirmamos que el paquete amazon-linux-extras está instalado en nuestro servidor.
  sudo apt -y update && sudo apt upgrade
Instalamos php como un módulo de Apache:
  sudo apt install php7.4 libapache2-mod-php7.4 php7.4-cli 
También necesitamos instalar mysql como módulo de apache:
  sudo apt install php7.4-mysql
Y reiniciamos apache:
  sudo systemctl restart apache2
Como podemos ver ya tenemos instalado php
![image](https://github.com/user-attachments/assets/9f0ffd14-6c07-46f1-95bb-0d7c014b0cc4)

Creamos la base de datos
![image](https://github.com/user-attachments/assets/2696c458-8fe6-4253-94db-ce1743633a77)
![image](https://github.com/user-attachments/assets/d0a5f860-ad4f-4ce8-8ac8-f2dcc979daf0)
![image](https://github.com/user-attachments/assets/3b262058-c5e2-4c15-9060-db878082db1b)
![image](https://github.com/user-attachments/assets/3c394ff9-3a4b-47d5-a3f5-2c2494280268)
![image](https://github.com/user-attachments/assets/388f09cd-2ca2-4550-bee3-09c845fbdde6)
![image](https://github.com/user-attachments/assets/163d8461-2d95-49d0-8692-3cd24c1d4a66)

Configuramos la configuración EC2 de la base de datos
![image](https://github.com/user-attachments/assets/4cbfca71-bd28-4531-bd8f-5fe623c7bd47)
![image](https://github.com/user-attachments/assets/7927d1af-5d3f-4271-8fad-500211405f7a)
![image](https://github.com/user-attachments/assets/a230ad4d-0748-46ac-957b-d9abd87334ee)

Creamos el sistema de archivos
![image](https://github.com/user-attachments/assets/ff6a8574-384d-4177-8f69-880b5e490df2)

Agregamos una regla en el grupo de seguridad
![image](https://github.com/user-attachments/assets/52845a47-c0d4-4877-9294-a4418f28e3c3)

Asociamos el EFS 
![image](https://github.com/user-attachments/assets/22d2791a-3d91-4cb8-843f-e492b046a743)

Vamos al siguiente directorio
![image](https://github.com/user-attachments/assets/e0fa79b9-6155-438e-9de3-b6eb7e9bf364)

Instalamos cleinte mysql
![image](https://github.com/user-attachments/assets/4898e3af-b951-42a9-aa1d-315d18e3dea8)

Iniciamos sesion en la base de datos
![image](https://github.com/user-attachments/assets/b06b2d6d-015b-41f7-906f-a84207cf2e77)

Creamos una base de datos
mysql -u admin -h nombre-dns-rds-wordpress -p 

Instalamos wordpress en la instancia desde la ruta /var/www/html
![image](https://github.com/user-attachments/assets/de9a94eb-8ae5-4989-b76b-a0beae0ce6de)
![image](https://github.com/user-attachments/assets/5ff43039-bf62-411b-9ce7-84f8b30d156b)
Como podemos ver ya esta instalado
![image](https://github.com/user-attachments/assets/068081a6-a782-466e-af3c-b9877ee8ab8f)


CREATE DATABASE wordpress; 
CREATE USER 'Admin' IDENTIFIED BY '777'; 
GRANT ALL PRIVILEGES ON wordpress.* TO 'Admin'; 
FLUSH PRIVILEGES;
![image](https://github.com/user-attachments/assets/f654dba5-81a1-4972-bb6b-9eeb4f56a3b7)


Ahora accedemos a wordpress desde el navegador para configurarlo
![image](https://github.com/user-attachments/assets/c5ede7bd-e261-4a7d-940b-b2a93bb48bfa)

