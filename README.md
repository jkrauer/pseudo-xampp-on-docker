Pasos para hacer funcionar esta cosa

1- Clonar

2- crear una carpeta llamada src, es ahí donde estará el sitio en php

3- configurar en app/db/db.env los valores de usuario y contraseña para mariadb

4- en caso de ser necesario, agregar paquetes de php en app/php/Dockerfile (por defecto se instala mysqli, pero se pueden agregar más paquetes poniendo sus nombres en las filas, hay mucha documentación al respecto buscando "docker-php-ext-install" en Google)

5- docker-compose up (mejor así, para tener reporte visual, se agrega -d si se quiere hacer en segundo plano todo)

La idea es que se trabaje sobre la carpeta src, de modo que cualquier cambio en el código se ve reflejado directamente en el sitio accediendo a localhost
