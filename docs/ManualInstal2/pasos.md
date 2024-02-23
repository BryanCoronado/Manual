# Pasos
## Manual de instalación  Linux | Valet 



Si desea implementar un servidor local Linux "desde cero", debe seguir los siguientes pasos:

1. **Acceso y privilegios:**
   - Acceder como usuario root.

2. **Instalación de PHP y librerías:**
   - Instalar PHP 7.2 y todas las librerías requeridas por el aplicativo y Laravel.

3. **Instalación de MySQL y PhpMyAdmin:**
   - Instalar MySQL y, opcionalmente, PhpMyAdmin para las primeras pruebas de la base de datos.

4. **Instalación de Git, Curl y Composer:**
   - Instalar Git, Curl y Composer.

5. **Configuración de PHP 7.2 en Ubuntu:**
   - Agregar un repositorio y proceder con la instalación de PHP 7.2 en Ubuntu.

6. **Instalación de librerías adicionales:**
   - Instalar librerías y herramientas necesarias como Curl y Git.

7. **Instalación de Composer y configuración:**
   - Instalar Composer y dar permisos de lectura y escritura a la carpeta Composer.

8. **Instalación de Valet y librerías adicionales:**
   - Instalar librerías cpriego de Valet, añadir la ruta a la carpeta Composer en el archivo `~/.profile`, y luego ejecutar `source ~/.profile`.

9. **Instalación de librerías adicionales:**
   - Instalar librerías como network-manager, libnss3-tools, jq, y xsel.

10. **Preparación para la instalación de Valet:**
    - Detener el servicio Apache2 si está instalado y asegurarse de que el puerto :80 esté libre.
    - Instalar el servidor Nginx, necesario para Valet.

11. **Instalación de Valet:**
    - Verificar que Nginx se esté ejecutando correctamente y luego instalar Valet.

12. **Configuración de Valet:**
    - Con Valet, podemos tener nuestro código en cualquier parte del sistema. En este caso, usaremos la carpeta home para instalarlo.

13. **Clonación del repositorio y configuración:**
    - Clonar el repositorio en la carpeta `~/code`, configurar el archivo `.env` y generar la clave de la aplicación.

14. **Migraciones y configuración de base de datos:**
    - Ejecutar migraciones y sembrar la base de datos, luego registrar la base de datos mediante PhpMyAdmin.

15. **Verificación y ajustes finales:**
    - Verificar y ajustar permisos en las carpetas del proyecto, principalmente en storage y cache.
    - Establecer la ruta de los archivos cargados de la empresa.
    
16. **Accesos:**
    - Una vez completados los pasos anteriores, podrá acceder al proyecto mediante la web con los siguientes accesos:
      - Sitio: Facturadorpro3.test
      - Usuario: admin@gmail.com
      - Contraseña: 123456
