---
sidebar_position: 3
---

1. **Acceder a su instancia vía SSH:**

   Acceda a su instancia utilizando SSH.

2. **Loguearse como super usuario:**

   Ejecute el siguiente comando para cambiar al superusuario:

   ```bash
   sudo su
   ```

3. **Ubicarse en la carpeta del usuario:**

   Por ejemplo, puede cambiar al directorio del usuario utilizando el comando `cd`:

   ```bash
   cd /home/ubuntu/
   ```

4. **Crear el archivo install.sh:**

   Utilice el comando `touch` para crear un nuevo archivo llamado `install.sh`:

   ```bash
   touch install.sh
   ```

5. **Editar el archivo con su editor preferido:**

   Utilice su editor de texto preferido, como `nano`, para abrir el archivo `install.sh`:


   ```bash
   nano install.sh
   ```
6. **Agregar el contenido del script:**

   Copie el contenido del script disponible en el siguiente enlace: [Script](https://gitlab.com/snippets/1852652). Pegue este contenido en el archivo `install.sh`. Es importante mantener la estructura del script tal como se muestra.

      ![Imagen1](https://i.ibb.co/NT2YPwR/Img.jpg)

7. **Guardar y Salir del Editor:**

   Para salir del editor y guardar los cambios en el archivo `install.sh`, siga estos pasos:

   - Presione `Ctrl + X`.
   - Se le consultará si desea guardar los cambios. Confirme presionando `y`.
   - Luego presione `Enter` para confirmar y salir del editor.

8. **Dar Permisos de Ejecución al Archivo:**

   Para otorgar permisos de ejecución al archivo `install.sh`, ejecute el siguiente comando:

   ```bash
   chmod +x install.sh
   ```

9. **Ejecutar el Script con Parámetros:**

   El comando a utilizar requiere de dos parámetros principalmente:

   ```bash
   ./install.sh [repositorio] [dominio]
   ```

   Por ejemplo:

   ```bash
   ./install.sh https://gitlab.com/rash07/facturadorpro2 elfacturador.com
   ```

10. **Proceso de Aceptación de Preguntas y Adición de Registros TXT:**

      Una vez ejecutado el comando, se iniciará un proceso interactivo donde se le presentarán preguntas y valores que debe añadir a los registros TXT de su dominio. Estos registros se utilizan para la validación del certificado SSL.

         - Durante el proceso, se le mostrarán en pantalla los valores que debe añadir en los registros TXT de su dominio. Por ejemplo, para un dominio `example.com`, los registros pueden ser `_acme-challenge.example.com` o `_acme-challenge` dependiendo del proveedor de dominio (por ejemplo, GoDaddy o Punto.pe).

         - Copie el valor mostrado y añádalo al primer registro TXT correspondiente. Luego, pulse Enter.

         - Se le mostrará en pantalla un segundo valor para el segundo registro TXT. Repita el proceso y añada este valor al segundo registro TXT de su dominio.

         Es importante seguir este proceso con precisión para garantizar una validación exitosa del certificado SSL.

       ![Imagen1](https://i.ibb.co/DkHNTrC/img12.jpg)

11. **Verificación de la Edición de los Registros en su Dominio:**
   Editados los récords en su dominio, deberá aceptar para continuar y que el proceso verifique que sea exitoso, de ser exitoso obtendrá una pantalla similar a la siguiente

      ![Imagen1](https://i.ibb.co/tJjhPVL/img13.jpg)

12. **Actualización del Sistema y Descarga del Proyecto desde GitLab:**
    Continuará el proceso de actualización del sistema, se le solicitará el usuario y contraseña de GitLab, para que se pueda clonar/descargar el proyecto en su instancia, luego culminará y tendrá los accesos listos en su dominio:

      - Correo: admin@gmail.com
      - Contraseña: 123456

      Una vez finalizado, puede proseguir con el manual de pruebas u otra documentación relacionada para cada proyecto:

         - PRO1: [Facturador Pro 1](https://gitlab.com/rash07/facturadorpro1)

         - PRO2: [Facturador Pro 2](https://gitlab.com/rash07/facturadorpro2)
