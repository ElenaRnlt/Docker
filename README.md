# Explicaciones de las configuraciones de Docker Compose

## Archivo docker-compose.yml para Drupal y MySQL

### Servicio de Drupal

- Utiliza la imagen Docker drupal.
- Mapea el puerto 81 del host local al puerto 80 del contenedor Drupal.
- Utiliza un volumen llamado drupal_data para persistir los datos.
- Define las variables de entorno para la conexión a la base de datos MySQL.

### Servicio de MySQL

- Utiliza la imagen Docker mysql:5.7.
- Utiliza un volumen llamado mysql_data para persistir los datos.
- Define las variables de entorno para configurar la base de datos MySQL.

## Archivo docker-compose.yml para WordPress y MariaDB

### Servicio de WordPress

- Utiliza la imagen Docker wordpress.
- Mapea el puerto 82 del host local al puerto 80 del contenedor WordPress.
- Utiliza la red Docker redDocker.
- Utiliza un volumen llamado wordpress_data para persistir los datos.
- Define las variables de entorno para la conexión a la base de datos MariaDB.

### Servicio de MariaDB

- Utiliza la imagen Docker mariadb.
- Utiliza la red Docker redDocker.
- Utiliza un volumen llamado mariadb_data para persistir los datos.
- Define las variables de entorno para configurar la base de datos MariaDB.

