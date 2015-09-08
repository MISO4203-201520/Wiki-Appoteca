# Vista funcional
La vista funcional de Appoteca es la siguiente:

- Los usuarios acceden al aplicativo desde sus plataformas web, utilizando dispositivos móviles como el PC, tablet o smartphone.
- Desde su navegador web pueden ver la interfaz web cargada desde el servidor.
- Al ejecutar acciones haciendo uso del aplicativo, se invocan los servicios web expuestos en internet en un servidor de aplicaciones.
- Una vez se hace el llamado, el servicio invoca el aplicativo JEE que hace el llamado a una BD Postgresql, la cual tiene la información del negocio.
- Una vez se ha procesado la petición del cliente, se devuelve la información, por el flujo anteriormente mencionado hasta que se muestra utilizando el navegador web.

![](https://cacoo.com/diagrams/yTIqH314RhQKEIQP-7C04A.png)

La arquitectura de la aplicación se puede ver en contraste con el siguiente diagrama:

![](https://cacoo.com/diagrams/B1gWEQjbmO8hfyDg-07195.png)