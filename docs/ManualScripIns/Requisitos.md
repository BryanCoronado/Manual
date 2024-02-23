---
sidebar_position: 2
---

# Requisitos previos


1. **Acceso SSH:**
   - Tener acceso a su servidor, VPS, máquina virtual o local via SSH. En las instalaciones que realizamos para AWS o Google Cloud, hacemos entrega del usuario, la IP del servidor y la clave SSH que puede ser un archivo .ppk o .pem. Recuerde almacenarlas en su equipo local.

2. **Instalación de SSH:**
   - Tener instalada una versión de SSH en su máquina para conectarse de manera remota. Puede utilizar Putty, Filezilla o una consola terminal. Para mayor información sobre el acceso SSH, visite los siguientes manuales:
     <!-- - [Guía para acceder con Putty (gestión de servidor)](./putty.md)
     - [Guía para acceder con WinSCP (gestión de archivos con aplicación de escritorio)](link_a_winscp) -->

3. **Configuración del dominio:**
   - Si es posible, configure su dominio apuntando a su instancia para que al finalizar la instalación se encuentre disponible el aplicativo. Edite los registros A y CNAME donde A debe contener su IP y CNAME el valor "*" (asterisco) para que se tomen los subdominios registrados por la herramienta.

   ![Imagen1](https://i.ibb.co/3zsfjb8/imagen1.webp)

4. **Detener servicios existentes:**
   - En caso de contar con servicios instalados en su instancia como MySQL, Apache o Nginx, debe detenerlos, ya que estos ocupan los puertos que pasarán a usar el aplicativo con los contenedores de Docker.
