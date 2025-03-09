Para empezar, vamos a instalar apache en nuestra máquina virtual de ubuntu

![image](https://github.com/user-attachments/assets/55c2e2c5-38a2-42d0-a3e5-fb40734f618a)

Ahora con apache instalado, pasamos a configurar el Archivo /etc/hosts para que este
incluya los dominios locales.

![image](https://github.com/user-attachments/assets/d2f67e73-09fe-4b7d-b818-d2818980b352)

Ahora vamos a activar los módulos necesarios para PHP y MySQL con los siguientes comandos.

![image](https://github.com/user-attachments/assets/1f1cd394-45f9-40a6-ae4d-8255f35fd66c)
![image](https://github.com/user-attachments/assets/344c93f0-0b7b-487f-87f2-08fa81125b5a)

Como podemos ver el módulo wsgi está instalado en el sistema

![image](https://github.com/user-attachments/assets/8457baf4-1550-4a26-9ebf-1f3aca2afee1)

Instalamos las dependencias necesarias para wordpress

![image](https://github.com/user-attachments/assets/2c66366b-940b-4717-942e-e9f23cf825da)
![image](https://github.com/user-attachments/assets/709aa652-2f0b-427c-9eb1-69db82536cc4)

Ahora pasaremos a crear una base de datos y un usuario para WordPress en MySQL

![image](https://github.com/user-attachments/assets/ac901029-1cf0-496c-9a8a-4f1601225387)
![image](https://github.com/user-attachments/assets/59ab978a-e8d3-477f-944f-911d0ce8550f)
![image](https://github.com/user-attachments/assets/3e9cb0a9-62c8-4432-80fb-86217b243180)

A continuación instalamos wordpress en el equipo y lo movemos al directorio de apache

![image](https://github.com/user-attachments/assets/0ca02da0-9882-402e-85bf-81849d48f5e2)
![image](https://github.com/user-attachments/assets/bc11acae-bc09-40cb-83f7-78bc68f27bd2)

Configuramos el archivo para que redireccione al directorio de wordpress

![image](https://github.com/user-attachments/assets/3adf0b3b-809a-496b-9248-601313cc6af7)

Activamos y reiniciamos apache

![image](https://github.com/user-attachments/assets/f7755455-ad0c-4c61-850a-121818dacd70)

Comprobamos que wordpress funciona

![image](https://github.com/user-attachments/assets/98c83d19-9f6a-441e-83f1-f67cccbe13db)


5. Desplegamos una aplicación Python bajo departamentos.centro.intranet

![image](https://github.com/user-attachments/assets/6ac5a0e4-ed32-4755-a3fe-ac948e75c95f)

Creamos el archivo de configuración

![image](https://github.com/user-attachments/assets/b277355b-1ceb-4f71-87d3-fdc0aaa2ece1)

Después creamos el directorio para la aplicación

![image](https://github.com/user-attachments/assets/d1e6d632-7df9-468b-b403-cd063b251eaa)

Dentro de este directorio creamos el archivo app.wsgi y un script de Python

![image](https://github.com/user-attachments/assets/27809c36-61ef-4c1a-b907-fcdc7e4d41e2)

Y otorgamos los permisos adecuados 

![image](https://github.com/user-attachments/assets/47505e81-ba98-4e60-8b64-366a8f0fdffd)

6. Adicionalmente protegeremos el acceso a la aplicación python mediante autenticación

Creamos un archivo para guardar las credenciales

![image](https://github.com/user-attachments/assets/5fe88ff1-b3e7-4152-ba27-75d4ee49a920)

Editamos el archivo de configuración para guardar las credenciales

![image](https://github.com/user-attachments/assets/e939afae-ec53-401b-9115-ebd6bcdc1663)

Por último recargamos Apache para aplicar los cambios

![image](https://github.com/user-attachments/assets/548ac85e-0610-42f1-8f9e-ab893f74b984)

Vemos la aplicación funcionando, le cambiamos el texto al mostrado en la imagen

![image](https://github.com/user-attachments/assets/0b572b99-be79-4258-9f82-9956ffadbcce)


7. Instalación y configuración de awstats:

![image](https://github.com/user-attachments/assets/3e58aeb4-4190-4159-a848-7897ac1f513b)
![image](https://github.com/user-attachments/assets/f30af91a-422e-4867-8ecf-660b45f92330)

Modificamos el archivo de configuración para que tenga el dominio adecuado

![image](https://github.com/user-attachments/assets/9c82c490-f7eb-4501-a223-7b1f0af63055)

Actualizamos manualmente

![image](https://github.com/user-attachments/assets/7973e234-ca7c-47e9-b951-2c718c7400bb)

Para acceder a ellas en el navegador, configuramos un alias en Apache

![image](https://github.com/user-attachments/assets/18608250-d799-4eb7-8311-60d2381ff189)

Por último reiniciamos apache

![image](https://github.com/user-attachments/assets/70133a81-27df-4d6a-b41a-66665c2aee47)

Mostramos awstats

![image](https://github.com/user-attachments/assets/3874b90e-789b-4481-8b0a-afafe5989e4c)


8. Configuramos un servidor Nginx

![image](https://github.com/user-attachments/assets/8b0974e8-816e-4293-944d-40506aad6c0a)

Después de instalarlo añadimos la configuración

![image](https://github.com/user-attachments/assets/ceefa46d-0527-4af0-86ee-fa60e0ed5304)
![image](https://github.com/user-attachments/assets/78de91e7-758c-4cc0-bc4c-7291f2681d75)
![image](https://github.com/user-attachments/assets/7c246c98-3247-4a85-af11-04de021c0b4f)

Por último instalamos phpmyadmin

![image](https://github.com/user-attachments/assets/9f3987d3-05f6-48e4-9733-ee3969ff7bd6)



