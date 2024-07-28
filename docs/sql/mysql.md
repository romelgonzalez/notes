# Comandos Básicos de MySQL

## Conexión al Servidor
- `mysql -u usuario -p` - Conecta al servidor MySQL.
- `USE nombre_base_datos;` - Selecciona la base de datos a utilizar.

## Gestión de Bases de Datos
- `SHOW DATABASES;` - Muestra todas las bases de datos.
- `CREATE DATABASE nombre_base_datos;` - Crea una nueva base de datos.
- `DROP DATABASE nombre_base_datos;` - Elimina una base de datos.

## Gestión de Tablas
- `SHOW TABLES;` - Muestra todas las tablas en la base de datos seleccionada.
- `CREATE TABLE nombre_tabla (columnas);` - Crea una nueva tabla.
- `DROP TABLE nombre_tabla;` - Elimina una tabla.

## Consultas Básicas
- `SELECT * FROM nombre_tabla;` - Selecciona todos los registros de una tabla.
- `INSERT INTO nombre_tabla (columnas) VALUES (valores);` - Inserta un nuevo registro en una tabla.
- `UPDATE nombre_tabla SET columna=valor WHERE condicion;` - Actualiza registros en una tabla.
- `DELETE FROM nombre_tabla WHERE condicion;` - Elimina registros de una tabla.