# Introducción
En el ámbito del desarrollo de software contemporáneo y la gestión de la información, las bases de datos relacionales continúan siendo la columna vertebral para el
almacenamiento estructurado, la persistencia y la integridad de los datos. MySQL se posiciona como uno de los sistemas de gestión de bases de datos relacionales
(RDBMS) más populares y eficientes del mercado, gracias a su robustez, escalabilidad y amplio soporte en la industria. Sin embargo, en entornos de producción
modernos, la interacción con las bases de datos raramente se realiza de forma manual mediante interfaces gráficas o consolas de comandos; en su lugar, se automatiza
a través de lenguajes de programación de alto nivel como Python, los cuales permiten integrar la lógica de negocio directamente con la capa de persistencia.

La integración entre Python y MySQL ofrece una combinación poderosa para desarrolladores y analistas. A través de conectores y controladores especializados, es
posible gestionar el ciclo de vida completo de la información de manera programática. Este proceso abarca desde la ejecución de sentencias del Lenguaje de Definición
de Datos (DDL) para la estructuración del esquema y la creación de tablas, hasta la aplicación de sentencias del Lenguaje de Manipulación de Datos (DML) para la
inserción, modificación y depuración de registros. Comprender cómo establecer conexiones dinámicas, controlar errores de ejecución y gestionar transacciones desde
código es una competencia esencial para la construcción de sistemas de información automatizados.

El presente reporte documenta el desarrollo práctico de operaciones sobre bases de datos relacionales mediante scripts de Python. Para cumplir con este propósito,
la práctica se estructura en el diseño y creación de tres tablas dentro de una base de datos MySQL. Sobre este esquema, 
se implementan las operaciones fundamentales de manipulación de datos. Específicamente, se detalla la ejecución de sentencias 
de inserción (INSERT), actualización (UPDATE) y eliminación (DELETE) para cada una de las tres entidades definidas.

A lo largo de este documento, se analizan la estructura del código en Python, el uso de controladores de conexión y el impacto directo de cada instrucción en el 
motor de MySQL. Este ejercicio busca validar la conectividad entre ambas tecnologías y sentar las bases prácticas para el desarrollo de aplicaciones capaces de 
interactuar con bases de datos de forma segura, eficiente y automatizada.

[⬅️ Regresar al Índice principal](../README.md) | [Siguiente: tabla 1 ➡️](02_tabla1.md)
