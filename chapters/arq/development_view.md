# Vista de desarrollo
La vista de desarrollo muestra la estructura de archivos para el proyecto. Inicialmente vemos la aplicación distribuida en 3 proyectos:

![](img/dev_all.png)

- `AppMarketPlace`: Proyecto Maven que agrupa los otros dos proyectos. Esto con fines de poder compilar y ejecutar pruebas para ambos proyectos más fácilmente.
- `AppMarketPlace.logic`: Proyecto con la lógica de negocio de la aplicación en el backend.
- `AppMarketPlace.web`: Proyecto Java Web con los servicios REST y los archivos de FrontEnd

## Proyecto AppMarketPlace.logic
Este proyecto contiene los archivos Java necesarios para cumplir con los requerimientos de la aplicación y comunicarse con la base de datos.

![](img/dev_back.png)

## Proyecto AppMarketPlace.web
Este proyecto se separa en dos grandes grupos de archivos. Aquellos correspondientes al FrontEnd, y aquellos correspondientes a los servicios RESTful.

### Estructura FrontEnd
En la ruta `src/main/webapp` se almacenan todos los archivos relacionados con el front-end. Dentro de esta carpeta encontramos los siguientes elementos:

- `index.html`: Punto de entrada para la aplicación web
- `app.js`: Archivo de configuración de la aplicación.
- Carpeta `src/modules`: Contiene los módulos de la aplicación AngularJS, donde cada puede contener los siguientes tipos de archivo:
  - `*.mod.js`: Archivos de configuración del módulo.
  - `*.svc.js`: Archivos con los servicios del módulo.
  - `*.ctrl.js`: Archivos con los controladores del módulo.
  - `*.tpl.html`: Plantillas propias del módulo.

![](img/dev_front.png)
### Estructura Servicios REST
![](img/dev_rest.png)