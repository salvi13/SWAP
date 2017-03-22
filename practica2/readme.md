# Práctica 2. Clonar la información de un sitio web

### Crear un tar con ficheros locales en un equipo remoto

Para crear el paquete usamos el siguiente comando
 
```bash
tar czf - directorio | ssh 10.0.2.4 'cat > ~/tar.tgz'
```
![Captura de la creación del paquete](./images/tar.PNG "Creación del paquete")

Y una vez hecho, podemos ver el resultado:

![Captura del resultado de la creación](./images/tar-resultado.PNG "Realización de la copia")

### Sincronizar máquinas con rsync
Para realizar la sincronización, vamos a utilizar los ficheros que tenemos en nuestro espacio web, por tanto haremos un rsync con el siguiente comando

```bash
rsync -avz -e ssh 10.0.2.4:/var/www/ /var/www/ 
```

![Captura de la sincronización](./images/rsync.PNG "Creación de la sincronización")

### Acceso sin contraseña para ssh
Ahora crearemos un par de claves ssh pública/privada, para ello usamos el comando
```bash
ssh-keygen -b 4096 -t rsa 
```

![Captura de la creación de claves ssh](./images/ssh-keygen.PNG "Creación de las claves ssh")

Una vez que tenemos las claves ssh, pasamos a copiar la clave pública en la otra máquina, para ello usamos el comando
```bash
ssh-copy-id 10.0.2.4
```

![Captura de la creación de claves ssh](./images/ssh-copy-id.PNG "Creación de las claves ssh")

Y con esto, solo nos queda añadir a nuestro crontab el script realizado anteriormente del rsync en el tiempo que queramos realizarlo.

Para ello, desde nuestro propio usuario podemos lanzar el comando
```bash
crontab -e
```

![Captura de la apertura del crontab](./images/crontab.PNG "Apertura del crontab")

Ahora, pondremos que cada hora a en punto se realiza una sincronización, para ello añadimos esto al crontab
```bash
00 *    * * *    /home/salvador/script
```

![Captura del crontab](./images/crontab-script.PNG "Crontab")
