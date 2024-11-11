# Ventas Online WhiteBox

Este repositorio contiene la estructura de base de datos para la plataforma **Ventas Online WhiteBox**, una tienda en línea que permite a los usuarios navegar y comprar productos con características avanzadas de gestión de inventario, carritos, pedidos y envíos.

## Estructura del Proyecto

- **Estructura de la Base de Datos**: El archivo `ventas_online_whitebox.sql` incluye la estructura de la base de datos, que contiene tablas para productos, pedidos, usuarios, notificaciones, y más.
- **Funciones Principales**:
  - Gestión de inventarios y productos.
  - Carritos de compra y pedidos.
  - Notificaciones y promociones para los usuarios.
  - Funcionalidad de "Encargos" para cotizar productos desde China a Colombia.

## Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/tu_usuario/base_de_datos_ventas_online.git

2. Importa la estructura de la base de datos (ventas_online_whitebox.sql) en MySQL.

    En MySQL Workbench, ve a Server > Data Import y selecciona el archivo .sql.

3. Crea un usuario y una contraseña para la base de datos en MySQL:

   CREATE USER 'tu_usuario'@'localhost' IDENTIFIED BY 'tu_contraseña';
   GRANT ALL PRIVILEGES ON ventas_online_whitebox.* TO 'tu_usuario'@'localhost';
   FLUSH PRIVILEGES;

4.Configura tu aplicación Laravel en el archivo .env:

	DB_CONNECTION=mysql
	DB_HOST=127.0.0.1
	DB_PORT=3306
	DB_DATABASE=ventas_online_whitebox
	DB_USERNAME=tu_usuario
	DB_PASSWORD=tu_contraseña

5. php artisan migrate:status


Contribuciones

¡Bienvenidas las contribuciones! Si deseas mejorar esta base de datos, siéntete libre de abrir un pull request o reportar problemas en la sección de issues.

