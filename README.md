# InstalacionConfiguracionNginx
## Instalación de Nginx
La instalación en este caso la hacemos des de un ubuntu, concretamente un desktop 20.04, en este, en su linea de comandos introducimos `sudo apt-get install nginx`<br>
![image](https://user-images.githubusercontent.com/91566044/166509345-9238020d-2169-4a4f-b05c-0d7af84e2235.png)
<br>

## Configuración de Nginx
<br>
Lo siguiente que haremos es copiar el default de `sites-available`de la aplicación, en este caso le cambiamos el nombre a `marc.com`.<br>
![image](https://user-images.githubusercontent.com/91566044/166510123-8d4e4575-436b-40bf-9c74-89e7e0c83a15.png)
<br>

Modificamos el archivo en cuestión, seleccionando donde escucha el servidor. <br>
![image](https://user-images.githubusercontent.com/91566044/166510643-8f08ec82-d9c1-46b2-8a13-eabdab559ab8.png)
<br>

Modificamos también el nombre de la carpeta del servidor y el nombre del servidor en si.<br>
![image](https://user-images.githubusercontent.com/91566044/166510742-f0dd14b2-e957-4e92-ada3-57e7273f0a0a.png)
<br>

Vamos a crear un archivo el cual va a apuntar al default de `sites-enabled`
![image](https://user-images.githubusercontent.com/91566044/166512088-1e1db65f-3f5a-44a7-96f0-1ad8750e1fb4.png)
<br>

Creamos la carpeta definida en `sites-available` en `/var/www`
![image](https://user-images.githubusercontent.com/91566044/166512612-b25c9a5f-24e6-46c3-9537-aacf82688647.png)
<br>

En esta carpeta vamos a crear el archivo html que vamos a usar
![image](https://user-images.githubusercontent.com/91566044/166513189-f7ef8200-baf0-4a13-9d08-66947cbbd042.png)
<br>

Entramos en el `/etc/localhost` y añadimos la direccion a la que apunta la pagina.
![image](https://user-images.githubusercontent.com/91566044/166513884-2d8a7348-d00f-4df4-9831-40d00296db7b.png)
<br>

Reiniciamos Nginx y comprobamos el resultado.
![image](https://user-images.githubusercontent.com/91566044/166514587-f4316071-fcff-4ab5-af03-d6ee3d521a97.png)
<br>

Repitiendo y duplicando los pasos podemos crear varios dominios en el mismo servidor, en este caso hemos creado `marc.com` y `marc2.com`.
![image](https://user-images.githubusercontent.com/91566044/166516701-739304e0-a036-4fd2-b690-a213686c6095.png)
