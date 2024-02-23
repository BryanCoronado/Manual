# Cat Code 

## Manuales de instalacion 

Instalación combinada de Docker con GitLab, configurado con opciones de SSL y SSH para seguridad, y Valet en entorno Linux. Además, incluye la instalación del facturador con Docker, GitLab y SSL para un sistema de facturación seguro.

![Logo de Markdown](https://i.ibb.co/HzYBNg3/Captura-de-pantalla-2024-02-23-160917.png)

 Demo : https://bryancoronado.github.io/Manual/
 <hr/>
 
## Contenido

- Manual para Script de Instalación
- Docker + GitLab + SSL
- Linux | Valet
- Instalación del Facturador



Si estas colaborando con nosotros usa los siguientes comandos:
### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
