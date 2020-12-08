# Project_tytus_Group7EDD

Universidad de San Carlos de Guatemala  
Facultad de Ingeniería  
Cursos: 772 Estructuras de Datos | 774 Sistemas de Bases de Datos 1 | 781 Organización de Lenguajes y Compiladores 2  
Diciembre 2020

## Modo árbol B

## Funciones de base de datos

Encargado [Byron Par](https://github.com/ByronPar)  , estructuras de datos para el almacenamiento --> tablas hash

- createDatabase(mode, database): crea una base de datos con cierto número de modo de almacenamiento (mode=1, 2, 3, 4, 5).
- showDatabases(): devuelve una lista de los nombres de las bases de datos, el nombre es único.
- alterDatabase(databaseOld, databaseNew): cambia el nombre de una base de datos.
- dropDatabase(database): elimina por completo la base de datos indicada.

## Funciones de tablas

Encargado [April Vilchez](https://github.com/KeilaVilchez) y [Minerva Vilchez](https://github.com/MinervaVilchez) , estructuras de datos para el almacenamiento ---> avl

- createTable(database, tableName, numberColumns): crea una tabla según el modo de almacenamiento, la base de datos debe de existir, y solo se define el número de columnas.
- showTables(database): devuelve una lista de los nombre de las tablas de una base de datos, los nombre de tablas son únicos.
- alterTable(database, tableOld, tableNew): cambia el nombre de una tabla de una base de datos.
- dropTable(database, tableName): elimina por completo la tabla indicada.
- alterAdd(database, tableName, columnName): agrega una columna a cada registro de la tabla.
- alterDrop(database, tableName, columnNumber): elimina una n-esima columna de cada registro de la tabla.
- extractTable(database, table): extrae y devuelve en una lista de listas el contenido de la tabla.

## Funciones de tuplas

Encargado [Pablo Oliva](https://github.com/27Pablooliva27), estructuras de datos para almacenamiento --> árbol B

- insert(database, table, columns): inserta un registro en la estructura de datos persistente, database es el nombre de la base de datos, table es el nombre de la tabla y columns es una lista de campos a insertar. Devuelve un True si no hubo problema, y un False si no se logró insertar.
- update(database, table, id, columnNumber, value): actualiza el valor de una columna x en un registro id de una tabla de una base de datos. Devuelve True si se actualizó correctamente y False si no se logró actualizar.
- deleteTable(database, tableName, id): elimina un nodo o elemento de página indicado de una tabla y base de datos especificada.
- truncate(database, tableName): vacía la tabla de todos los registros.
- extractRow(database, table, id): extrae y devuelve una tupla especificada 

## Función de carga desde un archivo CSV
Funcion encargada de llamar a las funciones add

- loadCSV(filecsv, database, table, [modo]): carga un archivo csv de un ruta especificada indicando la ruta de la base de datos y en qué tabla será guardada. Si la tabla existe verifica la cantidad de columnas, si no corresponde da error. Si la tabla no existe, la crea. Si la base de datos no existe, la crea con el modo especificado.


## Reportes
Los reportes de las estructuras utilizadas se deben mostrar mediante una aplicación de interfaz gráfica utilizando cualquier herramienta gráfica (que cumpla compatabilidades de licencia). 

La aplicación debe mostrar de manera gráfica y navegable las siguientes estructuras:
- bases de datos
- conjunto de tablas 
- tabla
- tupla

Cada estructura posee una función para mostrar su grafica. realizado por el encargado segun sea el caso de su estructura.

## Manual ténico y de usuario
En la carpeta del equipo se debe crear con Markdown un archivo de manual técnico y otro de manual de usuario. Se puede utilizar cualquier referencia bibliográfica para elaborar los manuales, se sugiere ver este [enlace](https://web.mit.edu/course/21/21.guide/docution.htm) del MIT.

Se estara completando en el transcurso de los días por cada uno de los integrantes.
