# 1. Descarga la imagen de Ubuntu
docker pull ubuntu

![image](https://github.com/user-attachments/assets/4edd59ae-6be4-4dba-baac-b5146b59645a)


# 2. Descarga la imagen de hello-world
docker pull hello-world

![image](https://github.com/user-attachments/assets/17ed0bac-63a2-4f0d-9bc1-f4fff9d607c1)


# 3. Descarga la imagen nginx
docker pull nginx

![image](https://github.com/user-attachments/assets/9505cedd-15d8-43f2-93a7-506094206834)


# 4. Muestra un listado de todas las imágenes
docker images

![image](https://github.com/user-attachments/assets/13759df6-c95a-43af-8f34-99389d964ede)


# 5. Ejecuta un contenedor hello-world y dale nombre “myhello1”
docker run --name myhello1 hello-world

![image](https://github.com/user-attachments/assets/d4e48190-d58d-4d93-8a28-b921c725c0e2)

# 6. Ejecuta un contenedor hello-world y dale nombre “myhello2”
docker run --name myhello2 hello-world

![image](https://github.com/user-attachments/assets/f7f07d53-d1e4-41fb-8e42-f171909bdfdb)


# 7. Ejecuta un contenedor hello-world y dale nombre “myhello3”
docker run --name myhello3 hello-world

![image](https://github.com/user-attachments/assets/e245a8a6-087e-4290-ac3a-438fda22c7aa)

# 8. Muestra los contenedores que se están ejecutando
docker ps

![image](https://github.com/user-attachments/assets/05c90ab9-6b40-4db0-9348-7a8f10cdd4d6)

# 9. Para el contenedor "myhello1"
docker stop myhello1

![image](https://github.com/user-attachments/assets/8f29c4d2-5da6-4462-8f15-18503b78b9f6)

# 10. Para el contenedor "myhello2"
docker stop myhello2

![image](https://github.com/user-attachments/assets/aae2d78d-0935-445e-af5a-0221ad2a659f)

# 11. Borra el contenedor “myhello1”
docker rm myhello1

![image](https://github.com/user-attachments/assets/7b54c2d7-4e3a-4852-92ba-da5fd4a5ca9b)

# 12. Muestra los contenedores que se están ejecutando
docker ps

![image](https://github.com/user-attachments/assets/399239e1-4fd4-4746-accf-5fdaf65fc360)

# 13. Borra todos los contenedores
docker rm $(docker ps -a -q), el comando deberia ejecutarse pero da un error el cual no encuentro solucion, por tanto he usado un comando que elimina los contenedores detenidos

![image](https://github.com/user-attachments/assets/8ea72279-8f0b-4b36-b2b1-bd9860c8da85)



