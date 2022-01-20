## BOILERPLATE BASIC WEBPACK BABEL FOR VSCODE

Este repositorio contiene una plantilla básica de un proyecto para vscode con webpack y babel

Para usarlo solo descarga este repocitorio con
```git clone https://github.com/programagol/boilerplate.git```

 Luego ejecuta dentro de la carpeta ```npm i``` (esto cargara los modulos), luego inicia vscode dentro de la carpeta con ```code .```, finalmente compila el proyecto con ```npm run build``` e inicia el servidor local con ```npm run serve```


## CREACION DE PLANTILLA PASO A PASO
Si quieres crear tu mismo la plantilla, sigue estos pasos:
1. Abrir un terminal de windows ```cmd```
1. ```mkdir project-name && cd project-name```
1. ```npm init -y```
1. ```code .```
1. en vscode editar dist/index.html
      ```
      <!DOCTYPE html>
      <html lang="es">
      <head>
      <meta charset="UTF-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Titulo</title>
      </head>
      <body>
      <script src="bundle.js"></script>
      </body>
      </html>
      ```
1. en vscode editar src/index.js
      ```document.getElementsByTagName('body')[0].innerHTML = "HOLA";```
1. instalar el plugin de vscode https://marketplace.visualstudio.com/items?itemName=jeremyrajan.webpack
1. en vscode CTRL+SHIFT+P -> ```Webpack Create```
1. ```npm install --save-dev webpack webpack-cli webpack-dev-server```
1. Agregar estos scripts al package.json
      ```
            "build": "webpack",
            "watch": "webpack --watch",
            "serve": "webpack-dev-server --open && npm run watch"
      ```
1. en vscode editar  .gitignore
      ```
      node_modules  
      ```
1. ```npm run build```
1. ```npm run serve```
