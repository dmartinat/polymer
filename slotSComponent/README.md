# SLOTS

### Polymer slot example
#### Crea un componente que tenga slots dedicados para cada sección.

-   **Header**

-   **Body**

    -   **Slide**

-   **Footer**

El slot **header** podrá recibir una imagen, en caso de recibirla tendrá que mostrarla y podrá recibir un texto, en caso de recibirlo también lo enseñará. En caso de no recibir nada, enseñará un texto predeterminado.

El slot **body** tendrá a su vez otro slot hijo que será un **slide** (carrousel).

- El slot **body** enviará un array de 3 objetos, cada objeto tendrá un ID único y un string que diga "Soy el ID x".

- Cada slide podrá ser clicable. Cuando se clique cualquier slide, se enviará un evento al padre que hará que se pinte en el elemento padre (en este caso, el body) qué ID se ha clicado.

- Ejemplo: clico el slide que dice "Soy el ID 3". Se envía un evento al padre, se añade al final del body "El ID 3 ha sido clicado". Si se clica otro ID, la frase será cambiada.

El slot **footer** actuará normal.
## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create builds of your application in the `build/` directory, optimized to be served in production. You can then serve the built versions by giving `polymer serve` a folder to serve from:

```
$ polymer serve build/default
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.