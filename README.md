# ProyectoPropper

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.0.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.


# Documentación
Para este proyecto es necesario tener instalado los siguientes paquetes: 
* **@fortawesome/free-brands-svg-icons**
* **@fortawesome/free-brands-svg-icons**
* **@fortawesome/angular-fontawesome@0.10.x** (Este ultimo lo necesitamos en esta versión ya que la versión empleada de Angular de este proyecto es de 13.0.2)
* **Bootstrap**
## Iconos
Para usar iconos en alguna parte de la pagina se tendran que agregar al ``` app.module.ts``` y agregar al constructor que se encuentra el icono que se necesite

**Ejemplo:**
``` ts
    import { faShoppingCart } from '@fortawesome/free-solid-svg-icons';

    constructor(library: FaIconLibrary){
        library.addIcons(faShoppingCart);
    }
```
>_Nota_: **La libreria que requiere cada icono puede variar, consultarlo en la documentación de los iconos**

Al momento de querer usar el icono en el html usaremos esta sintaxis
``` html
    <fa-icon [icon]="[prefijo , nombre del icono]">
```
Para saber el nombre del prefijo nos basaremos en esta tabla
| **Estilo** | **Prefijo** |
|------------|-------------|
| _Solido_   | **_fas_**   |
| _Regular_  | **_far_**   |
| _Marcas_   | **_fab_**   |

