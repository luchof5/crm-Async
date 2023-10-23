# Documentación de la Aplicación

Esta documentación proporciona una descripción detallada de los archivos y funciones principales de la aplicación.

## Descripción General

La aplicación se encarga de gestionar clientes. Permite agregar nuevos clientes, editar la información de los clientes existentes, ver la lista de clientes y eliminar clientes. La comunicación con el servidor backend se realiza a través de la API proporcionada en el archivo `API.js`.

## Archivo `nuevoCliente.js`

- **Descripción**: El archivo `nuevoCliente.js` se encarga de la creación de nuevos clientes en la base de datos. Escucha el evento de envío del formulario y realiza las siguientes acciones:
  1. Valida los datos del cliente.
  2. Muestra una alerta si faltan campos obligatorios.
  3. Envia una solicitud al servidor para crear un nuevo cliente.
  4. Redirige al usuario a la página principal después de agregar el cliente.

## Archivo `editarCliente.js`

- **Descripción**: El archivo `editarCliente.js` permite editar la información de un cliente existente. Al cargar la página, obtiene los datos del cliente a través de una solicitud al servidor y los muestra en el formulario de edición. Cuando se envía el formulario, realiza las siguientes acciones:
  1. Valida los datos del cliente.
  2. Muestra una alerta si faltan campos obligatorios.
  3. Envia una solicitud al servidor para actualizar el cliente.
  4. Redirige al usuario a la página principal después de editar el cliente.

## Archivo `App.js`

- **Descripción**: El archivo `App.js` controla la visualización de la lista de clientes y la eliminación de clientes. Al cargar la página, obtiene la lista de clientes a través de la API y muestra los datos en una tabla. Permite a los usuarios eliminar clientes y muestra una confirmación antes de realizar la acción.

## Archivo `funciones.js`

- **Descripción**: El archivo `funciones.js` contiene funciones de utilidad utilizadas en varios archivos. Incluye dos funciones principales:
  - `mostrarAlerta(mensaje)`: Muestra una alerta en el formulario en caso de error.
  - `validar(obj)`: Valida que todos los campos de un objeto no estén vacíos.

## Archivo `API.js`

- **Descripción**: El archivo `API.js` se encarga de interactuar con el servidor de backend para realizar operaciones relacionadas con clientes. Contiene funciones para comunicarse con la API del servidor, incluyendo:
  1. `nuevoCliente(cliente)`: Crea un nuevo cliente en la base de datos.
  2. `obtenerCliente()`: Obtiene la lista de clientes desde el servidor.
  3. `eliminarCliente(id)`: Elimina un cliente específico.
  4. `editarCliente(id)`: Obtiene los datos de un cliente para editarlos.
  5. `actualizarCliente(cliente)`: Actualiza la información de un cliente existente.

## Requisitos del Proyecto

Asegúrate de tener un servidor JSON-Server en ejecución en `http://localhost:4000` antes de utilizar la aplicación. De lo contrario, las solicitudes a la API no funcionarán correctamente.

## Uso

1. Descarga o clona el repositorio.
2. Asegúrate de tener JSON-Server instalado y configurado con una base de datos en `db.json`.
3. Abre los archivos HTML en tu navegador para interactuar con la aplicación.

## Contribución

Si deseas contribuir a la aplicación, por favor sigue estas pautas:
1. Crea un fork del repositorio.
2. Realiza tus cambios en una rama separada.
3. Asegúrate de realizar pruebas para comprobar que tus cambios funcionan correctamente.
4. Envía una solicitud de extracción.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para obtener más información.

## Contacto

Si tienes preguntas o sugerencias, puedes contactarme a través de [lucho_l.f@hotmail.com].

¡Gracias por utilizar esta aplicación!
