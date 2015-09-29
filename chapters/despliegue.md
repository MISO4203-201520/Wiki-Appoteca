# Consideraciones de despliegue

## Variables de entorno
Para el correcto funcionamiento de la aplicación debe definirse las siguientes variables de entorno. Estas variables contienen las credenciales para acceder a la cuenta de correo electrónico desde la cual se enviarán las notificaciones.

- EMAIL_HOST: Dirección del servidor SMTP
- EMAIL_PORT: Puerto de conexión
- EMAIL_HOST_USER Nombre de usuario.
- EMAIL_HOST_PASSWORD: Contraseña
- EMAIL_USE_TLS: Si se usa TLS o no.