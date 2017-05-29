# Ejercicios Tema 7

### Ejercicio 1
**¿Qué tamaño de unidad de unidad RAID se obtendrá al configurar un RAID 0 a partir de dos discos de 100 GB y 100 GB?**

En este caso tendríamos un RAID con 200GB de capacidad.

**¿Qué tamaño de unidad de unidad RAID se obtendrá al configurar un RAID 0 a partir de tres discos de 200 GB cada uno?**

En este caso tendríamos un RAID con 600GB de capacidad.

### Ejercicio 2
**¿Qué tamaño de unidad de unidad RAID se obtendrá al configurar un RAID 1 a partir de dos discos de 100 GB y 100 GB?**

En este caso tendríamos un RAID con 100GB de capacidad.

**¿Qué tamaño de unidad de unidad RAID se obtendrá al configurar un RAID 1 a partir de tres discos de 200 GB cada uno?**

En este caso tendríamos un RAID con 200GB de capacidad.


### Ejercicio 3
**Buscar información sobre los sistemas de ficheros en red más utilizados en la actualidad y comparar sus características. Hacer una lista de ventajas e inconvenientes de todos ellos, así como grandes sistemas en los que se utilicen.**

- **SMB/CIFS**: Es el sistema nativo de Windows y está orientado al funcionamiento en LAN
- **NFS**: Es el sistema nativo de Unix y funciona en tanto en LAN como en WAN.

**Configurar en una máquina virtual un servidor NFS. Montar desde otra máquina virtual en la misma subred la carpeta exportada y comprobar que ambas pueden acceder a la misma para lectura y escritura.**

Para la configuración del servidor NFS, podemos ver la práctica hecha anteriormente [aquí](https://github.com/salvi13/SWAP/tree/master/practica6 "Enlace a la practica 6")