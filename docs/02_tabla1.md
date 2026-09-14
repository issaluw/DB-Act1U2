# Establecer conexión (general)

El primer paso para comenzar con la manipulación de una base de datos, es realizar una correcta conexión, y para este caso será mediante el uso de Python, al mismo tiempo, para poder hacer la manipulación de la información, es necesario hacer uso de una de las librerías llamada "pandas" y se almacenara en una variable "pd" para hacer el manejo de esta misma

<div align="center">

![Conexion](<../assets/1_conexionDB.png>)

</div>

# Ejercicio 1 

<div align="center">

![ejercicio 1](<../assets/ejercicio1.png>)

</div>

## Creación de la tabla

Para definir la estructura de la entidad comida, se ejecuta un script SQL a través del método cur.executescript() en Python. Se establece la columna id_platillo como clave primaria autoincrementable, junto con los atributos nombre, categoria, precio (con formato decimal de precisión 6,2) y el estado disponible con un valor booleano predeterminado en TRUE. Tras confirmar la transacción con conn.commit(), la consola confirma la creación exitosa.

<div align="center">

![crecion de tabla](<../assets/2_creacionTabla1.png>)

</div>

## INSERT

Se realiza el poblamiento inicial de la tabla ejecutando una consulta INSERT INTO con tres registros correspondientes a distintos platillos (Chilaquiles, tacos y torta). Inmediatamente después, se valida la persistencia de los datos mediante una consulta de verificación (SELECT * FROM comida), confirmando que los valores numéricos y booleanos (donde 1 representa true y 0 representa false) se han almacenado correctamente en cada columna.

<div align="center">

![insert](<../assets/3_insertTabla1.png>)

</div>

## UPDATE

Se aplica una sentencia de actualización masiva mediante la instrucción UPDATE comida SET precio = precio * 2;, incrementando al doble el costo de todos los platillos registrados en la tabla. Al ejecutar la consulta de comprobación SELECT *, se observa la modificación reflejada en la columna precio: Chilaquiles pasa de 56.60 a 113.20, tacos de 65.48 a 130.96, y torta de 25.50 a 51.00.

<div align="center">

![update](<../assets/4_updateTabla1.png>)

</div>

## DELETE

Para evaluar la remoción condicional de datos, se ejecuta la sentencia DELETE FROM comida WHERE categoria = 'desayuno';. Esta instrucción filtra y remueve de la base de datos el registro del platillo torta, cuya categoría coincidía con la condición especificada. La consulta de validación posterior demuestra que la tabla conserva únicamente dos registros pertenecientes a la categoría comida.

<div align="center">

![delete](<../assets/5_deleteTabla1.png>)

</div>

[⬅️ Regresar a la introduccion](01_introduccion.md) | [Siguiente: Ejercicio 2 ➡️](02_tabla2.md)
