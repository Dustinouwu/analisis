# ARCHIVO ESTÁTICO A MYSQL
Extraeremos el archivo estático desde la página del gobierno “DATOS ABIERTOS”, específicamente el tema de “personas perdidas”. 
![image](https://user-images.githubusercontent.com/74982150/155870656-476c702c-dd07-4462-831d-73d24416778a.png)

Importaremos algunas librerías para poder realizar tanto la conexión para la base de datos MYSQL y poder leer el archivo que vamos a extraer de las páginas de archivos estáticos.

![image](https://user-images.githubusercontent.com/74982150/155870803-3a06500d-80eb-473e-8a4d-771b67e7005f.png)

Establecemos el nombre del host, el usuario y la contraseña de nuestro servidor de MYSQL, y posteriormente realizaremos esta conexión mediante un if, identificaremos si dicha conexión es exitosa o no, además de crear una variable para poder realizar las operaciones en lenguaje SQL en Python.

![image](https://user-images.githubusercontent.com/74982150/155870812-fe451dad-a513-48b6-8027-a5c47cf63b17.png)

Con la variable antes mencionada, crearemos mediante lenguaje SQL, una nueva base de datos dentro de MYSQL con la siguiente línea:

![image](https://user-images.githubusercontent.com/74982150/155870831-988230ee-25b7-4cdf-bd85-1cbbc101194f.png)

Crearemos una consulta para poder demostrar que la base de datos “PersonasPerdidas” se haya creado dentro de la base de datos de MYSQL.

![image](https://user-images.githubusercontent.com/74982150/155870850-009492a7-bdff-4794-98ed-45015d05a775.png)


Estableceremos la conexión hacia MYSQL desde Python, añadiendo el usuario, contraseña y por ultimo la base de datos que vamos a utilizar en este caso “PersonasPerdidas”

![image](https://user-images.githubusercontent.com/74982150/155870863-21fb7f74-4766-43d7-a881-2dea556a978f.png)

Cargaremos a la variable “df” gracias a la librería de pandas, el documento que extrajimos de la página de archivos estáticos mediante la extensión csv, también para poder leer este archivo hemos necesitado declarar el tipo de separador que utiliza nuestro archivo, caso contrario las columnas al momento de extraer se unen, adicionalmente utilizaremos ecoding para poder leer este archivo y para que no existan errores dentro de la lectura del archivo.

![image](https://user-images.githubusercontent.com/74982150/155870890-46184922-37c6-4075-9cf5-da59afb7f08d.png)

Como último paso, añadiremos la variable que ya contiene el archivo, crearemos la tabla que va ir en la base de datos, en este caso con el nombre de “información”, añadiremos la conexión previamente creada y pasaremos toda la información del archivo CSV  a la base de datos de MYSQL.

![image](https://user-images.githubusercontent.com/74982150/155870902-eb4a143b-34e1-410d-90ad-288a90fb65c4.png)

![image](https://user-images.githubusercontent.com/74982150/155870977-b0c469a5-9d8e-4f3b-a454-8634b177adf5.png)

![image](https://user-images.githubusercontent.com/74982150/155870981-8567f4e5-61fe-419d-ba3b-c550f0a16c32.png)


# MYSQL A MONGODB-ATLAS

Utilizaremos las siguientes librerías para poder realizar esta transición entre base de datos.

![image](https://user-images.githubusercontent.com/74982150/155871017-8fab0e62-2997-4702-b178-5fa982c9a985.png)

Crearemos la conexión hacia MONGODB ya establecido como conectador de datos, añadiendo que en este caso se va a tratar de MONGODB -ATLAS, para esto utilizaremos el clouster en el MONGODB en la nube, comprobaremos el éxito de esta conexión, y adicionalmente crearemos el nombre de la base de datos y colección para MONGODB y guardándolos en distintas variables.

![image](https://user-images.githubusercontent.com/74982150/155871035-3d39b878-58dc-4cd0-955e-6f1f8e2632ff.png)

Volveremos a establecer la conexión hacia MYSQL. 

![image](https://user-images.githubusercontent.com/74982150/155871040-0af9649a-22f8-4fe1-b7d3-89ec70c6707b.png)

![image](https://user-images.githubusercontent.com/74982150/155871051-8e354728-bd29-41d6-86dc-ed0bb5968079.png)

Crearemos el dataframe para poder pasar hacer la trasición de MYSQL hacia MONGODB, almacenaremos todo esto en una lista, para posteriormente mediante append para ir almacenando los múltiples datos y pasarlos hacia MONGODB-ATLAS.

![image](https://user-images.githubusercontent.com/74982150/155871070-71e74e74-3d9f-4af7-afc0-660b01f5e428.png)

![image](https://user-images.githubusercontent.com/74982150/155871091-5f2b8907-6938-4e61-a47e-3f5e9b910040.png)






