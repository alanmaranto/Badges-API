# CURSO DE REACT JS

## INTRODUCCIÓN A REACT JS

### ¿QUÉ ES REACT?

React cumple su función como biblioteca ya que para utilizar su código se debe importar. También es un Framework aunque las convenciones de cómo debe ser organizado todo no son estrictas.

En este curso aprenderás las prácticas que la comunidad ha decidido que son buenas.

> React es declarativo, lo que quiere decir que se le indica qué debe hacer pero no cómo debe hacerse, ahorrando de esta manera muchos pasos.

JSX es HTML dentro de Javascript, esto se verá más adelante en detalle.

React está estructurado por componentes que son como pequeños bloques de lego que al ser unidos forman aplicaciones de React. Estos componentes pueden tener estilos, ser enlazados a eventos y sus estados pueden ser modificados.

Con React también se tiene la ventaja de que será escrito una sola vez y podrá ser utilizado en aplicaciones web, móviles, entre otras.

### HERRAMIENTAS QUE USAREMOS

Estas son las herramientas que usaremos en el curso:

- Navegador: Especialmente Chrome ya que cuenta con óptimas herramientas de desarrollo.
- React Developer Tools: Es una herramienta Open Source creada por Facebook y tiene instalación para Chrome o Firefox. Nos dejará ver el código de React inspeccionando elementos.
- Editor de texto: Puedes usar cualquiera, en este curso sugerimos Visual Studio Code. Tiene muchos plugins útiles para el desarrollo.
- Prettier: Es un plugin que hace que el código se vea bien sin importar cómo esta escrito.

### CREATE REACT APP

**create-react-app** es una aplicación moderna que se usa desde una línea de comando. Antes de ella se configuraba todo el entorno manualmente lo cual tomaba mucho tiempo.

Pasos para obtenerlo:

- Se debe instalar desde la línea de comando usando `npm install -g create-react-app`

- Una vez instalado se crea la carpeta del proyecto con `create-react-app -nombre del proyecto-`

En este punto se estará instalando React y otras herramientas, también se configurará el entorno usando Webpack.

Una vez se instala todo entra a la carpeta src donde estará todo el código fuente de la aplicación, siendo el más importante index.js que es el punto de entrada a la aplicación.

- Finalmente para correr la aplicación se usa el comando `npm run start`

Otras herramientas:

- Babel: Traduce Javascript moderno (JSX) a un Javascript que todos los navegadores puedan interpretar.
- Eslint: Lee el código y avisa de errores.

### FUNDAMENTOS

### ReactDOM.render

React y ReactDOM trabajarán en conjunto.

- React como análogo a createElement.
- ReactDOM a appendChild-

`ReactDOM.render()` toma dos argumentos: Qué queremos renderizar y dónde lo queremos renderizar.

Siempre que escribas JSX es requisito importar **React**.

### JSX

JSX es una extensión de JavaScript creada por Facebook para el uso con la biblioteca React; sirve de preprocesador (como Sass o Stylus a CSS) y transforma el código generado con React a JavaScript.

JSX tiene su alternativa que es React.createElement pero es preferible JSX porque es mucho más legible y expresivo. Ambos tienen el mismo poder y la misma capacidad.

React.createElement recibe 3 argumentos:

1. El tipo de elemento que estamos creando
2. Atributos o props
3. El children que es el contenido.

Ejemplo:

```javascript
  React.createElement('a', { href: 'https://platzi.com' }, 'Ir a Platzi')
```

En **JSX** se utilizan las llaves para introducir variables o expresiones de Javascript. Lo que sea que esté adentro se va a evaluar y su resultado se mostrará en pantalla.

Las expresiones pueden ser llamadas a otras funciones, cálculos matemáticos, etc. Si las expresiones son false, 0, null, undefined, entre otros, no se verán.

En **jsx** es posible representar funciones através de `{}`, una **expresión** es algo que en JavaScript se va a interpretar y evaluar, por ejemplo `{2 + 2}`, si la expresión es null, o undefined los datos no se van a ver

```javascript
  import React from 'react'
  import ReactDOM from 'react-dom'

  const jsx = <div>
    <h1>Hi I'm Aaron</h1>
    <p>I'm Web Developer</p>
  </div>

  const container = document.getElementById('app')
  ReactDOM.render(jsx, container)
```
