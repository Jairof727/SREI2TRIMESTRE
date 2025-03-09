Para esta practica hemos usado una nueva maquina ya que la anterior ya tenia configuraciones las cuales podrian interferir con la practica.

Instalamos bind9

![image](https://github.com/user-attachments/assets/5515cb83-da34-4d9f-ae70-eacf2cd62f8f)


Creamos un fichero en /etc/bind llamado marisma.intranet.db y añadimos lo siguiente.


![image](https://github.com/user-attachments/assets/68f4952f-a426-4eb7-ac38-229e1e755b04)


Creamos ahora un archivo de configuracion para la zona inversa en /etc/bind


![image](https://github.com/user-attachments/assets/19a4958c-d8d8-4dcf-818e-40057c8db7db)

![image](https://github.com/user-attachments/assets/1d3a62a6-7c65-4f67-aaf8-545076f99ad3)

![image](https://github.com/user-attachments/assets/2424734a-e5e1-47df-acaa-cc989579bfcd)


Reiniciamos el servicio bind y hacemos varias consultas


![image](https://github.com/user-attachments/assets/98cf1fca-9637-4fae-bf2e-83d81e50114b)

![image](https://github.com/user-attachments/assets/5b540547-6133-4167-9d93-132ba99591a2)

![image](https://github.com/user-attachments/assets/fa3d7de9-e650-4abb-81c2-34fcfa2d1d95)

![image](https://github.com/user-attachments/assets/c4992eb2-d118-4b9f-aa35-f7dd017595b4)

