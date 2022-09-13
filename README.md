# consultas_1.sql

# Ejercicios CONSULTAS SQL

![tabla usuario](img/tablausuario.png"Tabla usuario")


1. Para visualizar toda la informacion que contiene la tabla `usuario` se puede incluir con la instruccion SELECT el caracter '*' o cada uno de lo campos de la tabla

SELECT * FROM `usuario` 
![tabla usuario](img/consultas1.png "consulta1")


2. visualizar solamente la identificacion del usuario.

SELECT identificacion FROM `usuario`
![consulta2](img/tablausuario.png "consulta2")

3. se desea obtener los registros cuya identificacion sean mayoes o iguales a 150, se debe utilizar la claudala WHERE que especifica las condiciones que deben reunir los registro que se debe reunir los registros que se van a seleccionar.

SELECT * FROM `usuario` WHERE identificacion>='150'

![consulta3](img/consulta3.png "consulta3")

4. si se desea obtener los registros cuyo sus apellidos sean vanegas o cetina se debe utilizar el operador IN que especifica los registros que se quieren visualizar de una tabla 

SELECT apellidos FROM `usuario` WHERE apellidos IN ('vanegas','celina');

![consulta4](img/consulta4.png "consulta4")

o se puede utilizar el operador OR.

SELECT apellidos FROM `usuario` WHERE apellidos='vanegas' OR apellidos='cetina';

![consulta4](img/consulta4-2.png "consulta4")

5. si se desea obtener los registros cuya identificacion sea menor de '110' y la ciudad sea 'cali' se debe utlizar el operador AND

SELECT * FROM `usuario` WHERE identificacion<'110' AND ciudad_nac='cali';

![consulta5](img/consulta5.png "consulta5")

6. si se desea obtener los registros cuyos nombres empiecen or la letra 'A', se debe utilizar el operdado LIKE que utiliza los patrones '%' (todos) y '_' (caracter).

SELECT * FROM `usuario` WHERE nombre LIKE 'A%';

![consulta6](img/consulta6.png "consulta6")

7. si desea obtener los registros cuyos nombres cotengan la letra 'a'.

SELECT * FROM `usuario` WHERE nombre LIKE '%a%';

![consulta7](img/consulta7.png "consulta7")

8. si se desea obtener los registros donde la cuarta letra del nombre sea un 'a'

SELECT * FROM `usuario` WHERE nombre LIKE '___a%';

![consulta8](img/consulta.png "consulta8")

9. si se desea obtener los registros cuya identificacion este entre el intervalo 110 y 150, se debe utilizar la clausala BETWENN, que sirve para especificar un intervalo de valores . 

SELECT * FROM `usuario` WHERE identificacion BETWEEN '110' AND '150';

![consulta9](img/consulta.png "consulta9")

## COMANDO DELETE

10. Para eliminar solamente los registros cuya identificacion sea mayor de 130

DELETE FROM `usuario` WHERE identificacion> '130';

![consulta10](img/consulta10.png "consulta10")
![consulta10](img/consulta10-2.png "consulta10")

## COMANDO UPDATE

11. para actualizar la ciudad de nacimiento de cristian vanegas, cuya identificacion es 114 . 

UPDATE usuario SET ciudad_nac='manizales' WHERE identificacion='114';

![consulta11](img/consulta11.png "consulta11")
![consulta11](img/consulta11-2.png "consulta11")

## INNER JOIN 

permite obtener dato de dos o mas tablas. cuando se realiza la concatenacion de las tablas, no necesariamente se deben mostrar todos los datos de las tablas









