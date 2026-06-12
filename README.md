# UNIVERISDAD TECNOLOGICA NACIONAL (UTN) --- TPI--- PROGRAMACION I --- 2026

Alumnas: Aquino Chiara Ayelen & Yazmin Dana Rodriguez

Fecha de entrega: 15/06/2026

Titulo del trabajo: Gestion de paises

# DESCRIPCIÓN DEL PROYECTO
Es un programa desarrollado en Python que administra información de paises guardados en un archivo CSV. Presenta un menú interactivo que permite al usuario visualizar, buscar, filtrar y ordenar la información alojada en el. Además, ofrece opciones para añadir más datos y generar estadisticas en base al contenido del archivo.

# ESTRUCTURA DEL ARCHIVO CSV --- ENTRADA
Este dataset denominado "paises.csv" administra las caracteristicas de los paises, tales como: nombre, población, superficie y continente. 
Al abrirlo, su estructura se puede visualizar de la siguiente manera:  

                                          (Fila 1)          # Encabezados                   nombre,poblacion,superficie,continente     
                                          (Fila 2)          # Caracteristicas               Argentina,45376763,2780400,America

Para su interpretación se debe tener en cuenta;
    1. Los encabezados se encuentran separados por comas porque el archivo ".csv" las utiliza para separar por columna.
    2. El archivo .csv se guarda con codificacion UTF-8, lo cual permite la lectura de caracteres como la Ñ y el uso de tildes.
    Para su ejecución;
    1. La función "csv.DictReader" realiza una lectura de las filas. Asigna claves (encabezados) y valores (caracteristicas) para armar diccionarios de datos.
    2. El ciclo for recorre el archivo por filas. Guarda la informacion en la lista "paises". 

# MANEJO DE ERRORES --- SALIDA
El programa valida los datos ingresados por el usuario. Si cumplen con las condiciones establecidas en el código, se ejecutan las funciones correspondientes.

En el caso de ingresar referencias invalidas y/o que no cumplan con las condiciones del programa, este último devuelve mensajes de "ERROR" y especifica por qué:
    1. "ERROR: ningun campo puede estar vacio."
    2. "ERROR: poblacion y superficie deben ser números enteros."

En el caso de los filtros, si no se encuentra coincidencia el programa imprime lo siguiente: 
    3. "No se encontraron paises."
    4. "No se encontraron paises en este continente."
    5. "No se encontraron países en ese rango de superficie."

# RESTRICCIÓN DE GUARDADO
El programa se ejecuta con datos almacenados en la memoria. 

Para que las modificaciones se guarden, se debe modificar el código para reescribir el archivo CSV.
Por lo tanto, los cambios realizados se eliminan al salir del programa.  
