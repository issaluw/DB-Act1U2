# Ejercicio 3

<div align="center">

![ejercicio 3](<../assets/imagenesTabla3/ejercicio3.png>)

</div>

## Creacion de tabla

Se define id_producto como clave primaria autoincrementable, junto con los campos nombre (cadena no nula), tipo, precio (de tipo decimal de precisión 6,2) y existencia, que asigna un entero con valor por defecto 0. La transacción se confirma mediante conn.commit(), notificando la creación satisfactoria de la tabla.

<div align="center">

![creacion tabla](<../assets/imagenesTabla3/1_crecionTabla3.png>)

</div>

## INSERT

Se efectúa la carga de datos del inventario ejecutando la sentencia INSERT INTO productos, registrando cuatro artículos con sus respectivos tipos, precios y existencias en stock: coca (bebida), galleta (snack), fanta (bebida) y paleta (dulce). Se ejecuta la consulta SELECT * FROM productos para validar el correcto almacenamiento e indexación de cada fila.

<div align="center">

![insert](<../assets/imagenesTabla3/2_insertTabla3.png>)

</div>

## UPDATE

Se aplica una actualización condicional ejecutando la consulta UPDATE PRODUCTOS SET precio = precio * 1.5 WHERE precio = 20;. Esta instrucción incrementa en un 50% el costo de aquellos productos cuyo precio base sea igual a 20. La verificación con SELECT * muestra que únicamente los productos coca y fanta actualizaron su precio de 20 a 30, mientras que galleta y paleta mantuvieron sus costos originales.

<div align="center">

![update](<../assets/imagenesTabla3/3_updateTabla3.png>)

</div>

## DELETE

Se lleva a cabo la baja de un elemento mediante la sentencia DELETE FROM productos WHERE existencia = 3;. Esta instrucción filtra los artículos y remueve de la base de datos el registro del producto fanta, el cual coincidía con el nivel de stock especificado. La consulta final de comprobación confirma que la tabla únicamente conserva los registros de coca, galleta y paleta.

<div align="center">

![delete](<../assets/imagenesTabla3/4_deleteTabla3.png>)

</div>

[⬅️ Regresar al ejercicio 2](03_tabla2.md) | [Siguiente: conclusion y referencias ➡️](05_referencias.md)



