# Operaciones CRUD en SQL
Las operaciones *CRUD* son un conjunto de cuatro operaciones fundamentales en el manejo de Base de Datos y aplicaciónes web. CRUD es un acronimo que representa las siguientes operaciones.

- **C**reate (crear)
- **R**ead (Leer)
- **U**pdate (Altualizar)
- **D**elete (Eliminar)

**Primero creamos una tabla:**
```SQL
CREATE TABLE Usuario(
    id_usuario INT PRIMARY KEY AUTO_INCREMENT,
    email VARCHAR(100) UNIQUE NOT NULL CHECK(email LIKE "%_@_%.%_%"),
    password CHECK(LENGTH(passwors))>=8

);
```
# CREATE
La operacion crear es responsable de insertar nuevos datos en la base de datos en el lenguaje SQL este se realiza con la sentencia

```Ejemplo de una ensercion valida usando todos los campos.
INSERT INTO usuarios VALUES (1, "ejemplo@gmail.com","123456789"):

#Ejemplo de una sercion valida usando el comando default
INSERT INTO Usuarios VALUES(DEFAULT) "miliorf12@gmail.com", "Demon12345";

#Ejemplo de una insercioón sin incluir el id_usuario.
INSERT usuarios(email,password)VALUES("miliorf12@gmail.com","Demon12345");

### Ejercicos Identifica los tipos de herrores que pueden salir en esta tabla.
#Inserta cuatro registros nuevos en un solo insertar





#READ
La operación **Leer** es utilizada para consultar y recueprar datos de la base de datos. ESto no modifica los datos, solamente los extrae. En MySQL est operación se realiza con la setencia ```SELECT``` 

``Èjemplo de una consulta para para todos los datos rn una tabbla.
SELECT * FROM usuarios;
Ejemplo de una consulta para un registro en especifico en caso de un Identifica
SELECT * FROM usuarios WHERE id_usuario=1;

```Ejemplo de consulta para un regsitro en un email, en especifico
SELECT * FROM usuarios WHERE emai
```Ejemplo de una ensercion valida usando todos los camposl="Eekjempo";

```Ejemplo de consulta con solo los campos de email y los campos
SELECT email,password FROM usuarios:

```Ejemplo de consulta con un condicionalloco
SELECT * FROM usuario WHERE LENGTH /passowrs 7== 9;






##Ejercicio
Realizar una consultar





# UPDATE
La operación Actualuzar se uliza para modificar registros existentes en la base de datos. ESto se hace con la sentencia UPDATE 
```Ejemplo para Actualizar su contraseña con su Identifica
UPDATE usuario SET password = "a12345446" WHERE id_usuario = 1;


```Ejemplo para actualizar el email y el password de un usuario en especifico```
UPDATE usuario SET password="Demon5516" email="emiliorf12@gmail" WHERE id_usuario=1;

Ejercicio Intenta Actualizar Registros con valores que violen las restricciones minimo 3 



#DELETE

La operacion Eliminar se usa para borrar registros de la base de datos. Estos se realiza con la setencia DELETE Debemos ser muy cuidadosos con esta operacion, ya que los datos son eliminados, ya no se podrian recuperar.

``` #Elimnar el usuario con el Delete ```

DELETE FROM usuarios WHERE id_usuaio=4;

# Eliminar los usuarios con el email espesifico 

DELETE FROM usuarios WHERE email = "miliorf12@gmail.com"

#Ejercicios 

Eliminar usuarios cuyo email, contenga uno o mas cincos 
Elimnar usuarios que tengan una contraseña que contenga letras mayusculas usando expresiones Regulares
Eliminar usuarios con contraeñas que contengan solo numeros
Eliminar usuarios con correos que no tengan el dominio gmail

REGEXP
