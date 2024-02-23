---
sidebar_position: 4
---
1. Después de instalar el facturador, puede necesitar cambiar algunos parámetros en el archivo `.env`, tales como:
    - La dirección de envío de correos que utiliza el facturador para enviar los archivos PDF, XML y CDR a sus clientes.
    - Cambiar algunas configuraciones de plantillas de los PDF.
    - Entre otros parámetros según sus necesidades.

<!-- 2. Recuerde que siempre que se edita el archivo `.env`, debe utilizar el comando `php artisan config:cache` dentro del contenedor de `fpm1`. Para más detalles, consulte el [manual de actualización aquí](link_to_manual). -->

3. Es importante tener en cuenta que la ruta donde ejecute el script será donde se clone el repositorio. Asegúrese de que los usuarios del servidor tengan permisos para acceder a dicha ruta si desea acceder desde FTP o SCP.
