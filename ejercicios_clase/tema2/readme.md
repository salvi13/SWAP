# Ejercicios Tema 2
### Ejercicio 1

**Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).**

	Elemento	| Disponibilidad 1 	| Disponibilidad 2 
 ---------------| ------------------| ----------------
 Web        	| 85% 	      		| 97.75% 
 Application	| 90% 	      		| 99% 
 Database     	| 99.9% 	      	| 99.9999% 
 DNS          	| 98% 	      		| 99.96% 
 Firewall     	| 85%           	| 97.75% 
 Switch       	| 99%           	| 99.99% 
 Data Center  	| 99.99%       		| 99.99% 
 ISP          	| 95%          	 	| 99.75% 

Fórmula: As = Ac1 + (1 - Ac1) * Ac2

Web = 97.75% + (1 - 97.75%) * 85% = 99.6625% 

Application = 99% + (1 - 99%) * 90% = 99.9%

Database = 99.9999% + (1-99.9999%) * 99.9% =99.9999999%

DNS = 99.96% + (1 - 99.96%) * 98% = 99.9992%

Firewall = 97.75% + (1 - 97.75%) * 85% = 99.6625%

Data Center = 99.99% + (1 - 99.99%) * 99.99% = 99.999999%

ISP = 99.75% + (1 - 99.75%) * 95% = 99.9875%

Disponibilidad del sistema = 99.6625% * 99.9% * 99.9999999% * 99.9992% * 99.6625% * 99.999999% * 99.9875%

Disponibilidad del sistema = 99.21% 

### Ejercicio 2

**Buscar frameworks y librerías para diferentes lenguajes que permitan hacer aplicaciones altamente disponibles con relativa facilidad. Como ejemplo, examina PM2 https://github.com/Unitech/pm2 que sirve para administrar clústeres de NodeJS.**

- **PHP**: Yii, Symfony, Zend Framework, Laravel, CodeIgniter

- **JavaScript**: jQuery, BackboneJS, AngularJS, KnockoutJS

- **CSS**: Bootstrap, Foundation, Materialize, Semantic IU

- **NodeJS**: Grunt, Gulp, Browserify, Webpack

- **Java**: Spring MVC, Hibernate, JSF, Vaadin

- **Python**: Django, Flask, Pyramid, Bottle

### Ejercicio 3

**¿Cómo analizar el nivel de carga de cada uno de los subsistemas en el servidor? Buscar herramientas y aprender a usarlas.**

En Linux podemos utilizar el comando top para ver como se están consumiendo los recursos de la máquina, al igual que en Windows podemos usar el administrador de tareas, que también incluye dicha funcionalidad.

Para comprobar como tenemos la red, podemos utilizar Nagios por ejemplo.

### Ejercicio 4

**Buscar ejemplos de balanceadores software y hardware (productos comerciales). Buscar productos comerciales para servidores de aplicaciones. Buscar productos comerciales para servidores de almacenamiento.** 

- Balanceadores software:
	- LVS
	- Ultra Monkey
	- Pound
	- Zen Load Balancer
	- Haproxy
	- Nginx

- Balanceadores hardware:
	- Routers cisco
	- F5 BIG-IP LTM
	- ADC Barracuda

- Productos comerciales para servidores de aplicaciones.
	- WebLogic de Oracle.
	- WebSphere de IBM.
	- JBoss AS de JBoss (RedHat).
	- Geronimo y TomEE de Apache.
	- GlassFish de Oracle

- Productos comerciales para servidores de almacenamiento.
	- Seagate Personal Cloud
	- Servidores NAS, como por ejemplo, Synology DS216.