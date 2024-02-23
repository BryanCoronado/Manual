---
sidebar_position: 2
---

# Requisitos previos


Antes de utilizar el script, asegúrese de cumplir con los siguientes requisitos:

1. **Acceso al Servidor:**
   - Debe tener acceso a su servidor, VPS, máquina virtual o local a través de SSH. En las instalaciones realizadas en AWS o Google Cloud, se proporciona un usuario, la IP del servidor y la clave SSH que puede ser un archivo `.ppk` o `.pem`.

2. **Instalación de SSH:**
   - Es necesario tener instalada una versión de SSH en su máquina para conectarse de manera remota al servidor. Puede utilizar herramientas como PuTTY, FileZilla o una consola terminal.

3. **Configuración del Dominio:**
   - Es importante configurar su dominio para que apunte a la IP de su instancia. Durante la ejecución del script, se validará el certificado SSL, y al finalizar la ejecución, no debería haber errores y todo estará listo para realizar pruebas.
   - Edite los registros A y CNAME de su dominio, donde el registro A debe contener su dirección IP y el registro CNAME debe tener el valor `*` (asterisco) para que se tomen los subdominios registrados por la herramienta.

    ![Imagen1](https://i.ibb.co/qMzJWKg/Imagen-de-Whats-App-2024-02-23-a-las-12-04-56-9b67e2cb.jpg)

4. **Almacenamiento de Registros TXT en el Dominio:**

   Durante la ejecución del script, deberá almacenar en su dominio dos registros TXT con unos valores específicos que se mostrarán en pantalla. Estos registros son necesarios para la validación en directo del certificado SSL y no pueden tardar más de 2 minutos en validarse en su dominio. Asegúrese de agregar estos registros correctamente para garantizar una validación exitosa del certificado SSL.

5. **Detener Servicios Instalados en la Instancia:**

   Si cuenta con servicios instalados en su instancia, como MySQL, Apache o Nginx, es importante detenerlos antes de ejecutar el script. Estos servicios ocupan los puertos que serán utilizados por el aplicativo y los contenedores de Docker que se configurarán. Detener estos servicios evitará conflictos de puerto y asegurará un despliegue correcto de la aplicación.

