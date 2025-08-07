# Formulario-para-subir-archivos
Este proyecto está  destinado para que los usuarios suban archivos a un servidor local por medio de MySQL y PHP. El formulario cuenta con la opción de colocarle un nombre al archivo que se está subiendo, en la parte de subir los archivos podemos optar por dos variables arrastras los archivos o usar el buscador para llegar al archivo que se desea subir. En la base de datos se configuró como extra la columna de fecha y hora para saber cuando se subió el archivo. El estilo es simple, siguiendo el modelo asignado.

# Tecnología usada en el proyecto
## HTML:
Se usaron etiquetas <div>, <form>, <label>, <input> y <button> para dar forma a la estructura del formulario. A cada una se le asignó una clase para poder vincularlas a la hoja de estilo en CSS, además de eso a <label> e <input> se les asignó el mismo nombre en los atributos for e id  para su correcto funcionamiento. En cuanto a la etiqueta <form> se configuró con acction y method para que los datos (en este caso archivos)  sean enviados de forma correcta al archivo PHP, además se configuró enctype para el envío de los archivos a la base de datos.

## CSS:
Se aplicaron estilos básicos al formulario. Para ello se usaron selectores de tipo generales y de clase, a los cuales se les dieron diferentes propiedades y valores para llegar al resultado esperado, por mencionar algunas de las propiedades usadas en el proyecto son: background, background-color, text-aling, aling-item, color, margin, padding, transition, box-shadow, box-sizing.

## PHP:
Antes de empezar con la redacción del código, se utilizaron dos funciones para mostrar errores en el navegador cuando el código fue puesto a prueba. Después de esto se realizó la conexión con la base de datos local por medio del planteamiento de variables una estructura condicional para notificar si hay algún error al realizar la conexión. Seguido se realizó una comprobación de cómo se envió el formulario, esto por medio de condicionales. Nos aseguramos que le de un título y que exista la carpeta donde se subirán los archivos. Luego configuramos para que se le asigne un nombre combinando el nombre del título que se le asignó y el nombre de origen del archivo. Para finalizar se declara una variable para insertar el archivo, después se declara una variable para la preparación de la carga del archivo y una para los parámetros que se utilizaran, por medio de condicionales se le informa al usuario si el archivo se cargó con éxito o hubo algún error.

## MySQL:
La base de datos fue creada usando "phpMyAdmin" desde el panel de Xampp. No se utilizó código SQL, pero si se utilizó el motor de MySQL, todo se realizó por medio de la interfaz gráfica de "phpMyAdmin".
Para crearla se procedió usando una base de base de datos ya existente (registro_usuarios, ver proyecto de registro de usuario) y dentro de esta se creó una nueva tabla (documentos). De la última se completaron los campos solicitados para cada columna, teniendo en cuenta los nombres dados en el formulario HTML para cada columna. Los datos llegan a la base de datos desde el formulario antes mencionado y su conexión con PHP.

# Descargar el archivo

- Busca el botón verde que dice <>Code
- Hace click en la fecha que tiene el botón
- Selecciona "Download ZIP"
- Descomprime el archivo ZIP
  Como tiene archivos PHP y está vinculado a MySQL vamos a:
- Moverlo a la carpeta "htdocs" (se ubica en el sistema, la ruta es /opt/lampp/htdocs, puede variar según sea tu sistema operativo)
- Dentro de esta carpeta crear una neva carpeta con el nombre "uploads", en ella se almacenaran los archivos que suba el usuario

# Creando la base de datos
- Abre XAMPP, activa los servidores.
- Ve al navegador, en la barra de URL coloca "http://localhost" (te lleva a la página principal de tu servidor local)
- Busca "phpmyadmin"
- Busca la base de datos "registro_usuarios"
- Una vez lista, selecciona "Importar"
- Donde dice "Examinar", busca la ruta del archivo SQL que viene en la carpeta del proyecto
- Baja hasta el final y click al botón "Importar"

# Ejecutar en el navegador
- En la barra de URL coloca "http://localhost/nombre_de_la_carpeta/index.html"
- Enter y eso abrirá el formulario

# Agradecimientos
A los profesores Gustavo Rojas y Carolina Riveros por su arduo trabajo al enseñarnos, y a Punto Digital San Martín Mza. por la oportunidad de este cursado.
