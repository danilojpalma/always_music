# Introducción

Este programa te permite gestionar una base de datos de estudiantes en PostgreSQL. Puedes realizar acciones como agregar, consultar, editar y eliminar estudiantes.

### Requisitos previos

``Tener instalado Node.js y npm``
Tener una base de datos PostgreSQL configurada y funcionando

Instalación

Clona o descarga el repositorio del código.
Ejecuta el siguiente comando en la carpeta del proyecto:
Bash
npm install
Usa el código con precaución.
content_copy
Uso básico

Abre una terminal y navega hasta la carpeta del proyecto.
Ejecuta el siguiente comando, reemplazando <accion> con la acción que deseas realizar y los argumentos correspondientes:
Bash
node index.js <accion> <argumentos>
Usa el código con precaución.
content_copy
Acciones disponibles:

nuevo: Agrega un nuevo estudiante a la base de datos.
Argumentos: nombre, rut, curso, nivel
Ejemplo: node index.js nuevo Juan Pérez 12345678-9 Ingeniería Informática 3
rut: Consulta un estudiante por su RUT.
Argumentos: rut
Ejemplo: node index.js rut 12345678-9
consulta: Muestra todos los estudiantes registrados.
Argumentos: No requiere argumentos.
Ejemplo: node index.js consulta
editar: Edita la información de un estudiante existente.
Argumentos: nombre, rut, curso, nivel (nuevos valores)
Ejemplo: node index.js editar Juan Pérez 12345678-9 Ingeniería Informática 4
eliminar: Elimina un estudiante de la base de datos.
Argumentos: rut
Ejemplo: node index.js eliminar 12345678-9
Mensajes de error

Si se proporciona un número incorrecto de argumentos, se mostrará un mensaje de error indicando la cantidad correcta de argumentos para cada acción.
Si se produce un error al conectar a la base de datos o al ejecutar una consulta, se mostrará un mensaje de error con información sobre el error.