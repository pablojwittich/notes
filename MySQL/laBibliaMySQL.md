# LA BIBLIA DE MYSQL - IAN GILFILLAN
---
# Parte 1: Uso de MySQL
## Guia rapida MySQL
*MySQL es la base de datos de codigo abierto mas popular del mundo, su fundador es Michael "Monty" Windenius*
### 1.1. Compresión de los fundamentos de MySQL
MySQL es un *sistema de administación de base de datos relacional* (RDBMS). Capaz de almacenar una enorme cantidad de datos de gran variedad y de distribuirlos para cubrir las necesidades de cualquier tipo de organización. MySQL compite con sistemas RDBMS propietarios como Oracle,  SQL Server, DB2.
MySQL incluye todos los elementos necesarios para instalar el programa, preparar diferentes niveles de acceso de usario, administrar el sistema y protegerlo, hacer volcados de datos, etc. MySQL utiliza el lenguaje de consuslta estructurado (SQL) que trata del lenguaje mas utilizado por todas las bases de datos.
### 1.2. Que es una base de datos
Es una calección de archivos relacionados. La mayor parte de las bases de datos actuales son de tipo relacional, se denominan asi porque utilizan tablas de datos relacionadas por un campo en común. Ejemplo:

*Tabla 1.1. Product*

| Stock_code |  Descripción | Prize |
|------------|--------------|-------|
| A416       | Clavos, caja | $0.14 |
| C923       | Chincheta    | $0.08 |


*Tabla 0.2. Invoice*

|Invoice_code | Invoice_line | Stock_code | Quanty |
|-------------|--------------|------------|--------|
| 3804        |     1        |  A416      |  10    |
| 3804        |     2        |  C923      |  15    |

