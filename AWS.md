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





