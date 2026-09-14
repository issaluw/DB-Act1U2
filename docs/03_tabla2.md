# Ejercicio 2

<div align="center">

![Ejercicio 2](<../assets/imagenesTabla2/ejercicio2.png>)

</div>

## Creación de tabla

La tabla define un identificador único id_alumno como clave primaria autoincrementable, junto con los campos nombre (cadena no nula), grado, edad (entero no nulo) y promedio, el cual utiliza un tipo de dato DECIMAL(4,2) con un valor predeterminado de 0.0. Tras aplicar los cambios con conn.commit(), el sistema confirma la creación de la tabla.

<div align="center">

![creacion tabla](<../assets/imagenesTabla2/1_creacionTabla2.png>)

</div>

## INSERT

Se realiza el registro de información académica mediante la instrucción INSERT INTO alumnos, agregando tres estudiantes con sus respectivas edades, grados y promedios: Juan (3ro A), carlos (5to B) y julian (1ro B). La consulta posterior (SELECT * FROM alumnos) confirma que los datos se almacenaron e indexaron de forma correcta en la base de datos.

<div align="center">

![insert](<../assets/imagenesTabla2/2_insertTabla2.png>)

</div>

## UPDATE

Para realizar una modificación puntual en la base de datos, se ejecuta la consulta UPDATE alumnos SET promedio = 7 WHERE id_alumno = 1;. Esta instrucción busca de manera específica al alumno con el ID 1 (Juan) y actualiza su calificación de 9.5 a 7.0, manteniendo intactos los datos de los demás estudiantes.

<div align="center">

![Update](<../assets/imagenesTabla2/3_updateTabla2.png>)

</div>

## DELETE

Se efectúa una depuración condicional ejecutando la sentencia DELETE FROM alumnos WHERE promedio = 6.1;. La condición evalúa y elimina el registro correspondiente al alumno carlos, cuyo promedio coincidía con el valor especificado. Al consultar nuevamente la tabla, se verifica que solo permanecen los registros de Juan y julian.

<div align="center">

![delete](<../assets/imagenesTabla2/4_deleteTabla2.png>)

</div>



[⬅️ Regresar al ejercicio 1](02_tabla1.md) | [Siguiente: Ejercicio 3➡️](04_tabla3.md)
