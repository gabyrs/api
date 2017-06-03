# api
repositorio para api

Proyecto Pagina web de venta de empanadas 02/06/2017.
=======================================
Es indispensable el tener instalado Apache2 para el correcto funcionamiento del proyecto.
Se requiere hacer un par de configuraciones sobre el archivo “apache2.conf” , el cual se puede encontrar accediendo →  /etc/apache2/apache2.conf

Es necesario editar de la siguiente manera:
"AllowOverride None"  se modifica por  "AllowOverride All" en 
<Directory /usr/share>
	AllowOverride All
	Require all granted
</Directory>

<Directory /var/www/>
	Options Indexes FollowSymLinks
	AllowOverride All
	Require all granted
</Directory>
=========================================
Una vez terminada esta configuracion se puede ejecutar el proyecto. Por lo que se procede a descargar el archivo .zip y se pone sobre la carpeta /var/www/html
El archivo pagina.sql” se encuentra en la carpeta "Base de datos" y debe ser importada en phpMyAdmin, la cual ya contiene algunos registros. 
Para ver las consultas solo es necesario acceder a la ruta “localhost/api”   
