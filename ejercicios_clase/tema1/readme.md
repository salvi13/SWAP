# Ejercicios Tema 1
**Buscar información sobre las tareas o servicios web para los que se usan más los programas que comentamos al principio de la sesión**
- **Apache**: 
Es el servidor web más usado en el mundo, principalmente para enviar páginas web estáticas y dinámicas en la World Wide Web (WWW). Entre las principales características de Apache, se encuentran las siguientes:
    - Soporte de seguridad SSL y TLS.
	- Puede realizar autentificación de datos utilizando SGDB.
	- Puede dar soporte a diferentes lenguajes, como Perl, PHP, Python y tcl.
	- Modular.
	- Código abierto.
	- Multiplataforma.
	- Extensible.
	- Fácil de conseguir ayuda y soporte.

- **nginx**:
nginx además de ser un servidor web ligero de alto rendimiento, también es un excelente proxy inverso para contenido web o para protocolos de correo electrónico como por ejemplo IMAP o POP3. Una de sus principales ventajas es que consume menos recursos al servir páginas estáticas. Además, su arquitectura, es diferente al modelo tradicional, de crear una instancia por cada petición. NGINX procesa decenas de miles de conexiones simultáneas en un proceso compacto y con varios núcleos de CPU. Más características:
    - SMTP, POP3 e IMAP
    - El proxy inverso ayuda con el balanceo de carga distribuyendo las peticiones y almacenando en caché parte del contenido.
    - Cuenta con caché para solicitudes HTTP
	- Facilita el uso de URL con posibilidad de usar expresiones regulares
	- Función de rastreo y seguimiento de los usuarios
	- Actúa como web server si fuese necesario
	- Soporta TLS/SSL y similares
	- Ofrece cierta tolerancia a fallos

- **thttpd**:
thttpd (tiny/turbo/throttling HTTP server) es un servidor web de código libre disponible para la mayoría de las variantes de Unix. Se caracteriza por ser simple, pequeño, portátil, rápido, y seguro, ya que utiliza los requerimientos mínimos de un servidor HTTP. Esto lo hace ideal para servir grandes volúmenes de información estática. Sus características:
	- Simple.
	- Pequeño.
	- Portátil.
	- Rápido.
	- Seguro.

- **Cherokee**:
Es un servidor web multiplataforma. Su objetivo es ser rápido y completamente funcional, sin dejar de ser liviano comparado con otros servidores web. Sus características:
	- Soporta tecnologías como: FastCGI, SCGI, PHP, CGI, SSI, SSL/TLS.5
	- Soporta la configuración de servidores virtuales.
	- Permite la realización de redirecciones.
	- Permite su utilización como balanceador de carga.
	- Dispone de un panel de autenticación:
		- plain
		- htpasswd
		- htdigest
		- PAM

- **node.js**:
Node.js es un entorno de ejecución para JavaScript construido con el motor de JavaScript V8 de Chrome. Node.js usa un modelo de operaciones E/S sin bloqueo y orientado a eventos, que lo hace liviano y eficiente. El ecosistema de paquetes de Node.js, npm, es el ecosistema mas grande de librerías de código abierto en el mundo. Al contrario que la mayoría del código JavaScript, no se ejecuta en un navegador, sino en el servidor. Fue creado con el enfoque de ser útil en la creación de programas de red altamente escalables, como por ejemplo, servidores web.