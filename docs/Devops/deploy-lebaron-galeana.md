# Deploy Lebaron Galeana

El deploy de Lebaron Galena es diferente dependiendo de si el deploy lo requieres para el frontend o backend.

## Frontend

Para realizar el deploy se requiere:

- Tener el [repo de Lebaron Galena Frontend](https://github.com/LebaronGaleana/LebaronGaleana) cloneado en tu local.
- Tener instalado Node.js en su versión especificado en el archivo `.nvmrc` que está dentro del repositorio.
- Tener instalado todas las dependencias de NPM (`npm install`).
- Tener acceso a la bucket de S3 de `lebaron-galeana-frontend` en la consola AWS.

El proceso para realizar el deploy es:

- Crear un Pull Request con tus cambios desde tu branch a la branch `Staging` y mergear el Pull Request.
- Hacer checkout a la branch de `Prod`.
- Hacer pull de la branch de `Staging`.
    - Si salen conflictos, toma en cuenta que es necesario utilizar URLs para la API diferentes en producción.
- Corre `npm run build`
- Entrar a la bucket de AWS S3 `lebaron-galena-frontend` y borrar todos los archivos.
- Copiar todos los archivos de tu local dentro del subdirectorio `dist`, dentro del repositorio, a la bucket de S3 de AWS `lebaron-galeana-frontend`.
- Hacer todos los archivos de la AWS S3 bucket, `lebaron-galeana-frontend`, públicos:
    - En la consola de AWS, dentro de la bucket, seleccionas todos los archivos.
    - Abres el menú de acciones.
    - Seleccionas la opción de `Make public via ACL`.
    - Confirmar.

Después de este proceso, es importante probar tus cambios en producción para asegurar que tus cambios funcionan correctamente y no se introdujeron bugs sin querer.

## Backend

Parar realizar el deploy se requiere:

- Tener el [repo de Lebaron Galeana Backend](https://github.com/adrianlebaron/Lebaron-galeana-django-BE) cloneado en tu local.
- Tener instalado [Elastic Beanstalk CLI](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-install.html) en tu local.
- Tener la clave de acceso para el EB CLI. Este no se puede descargar de nuevo, es necesario pedírselo a un compañero que ya ha hecho el deploy previamente.
- Inicializar el EB CLI dentro del repositorio en tu local:
    - Estando dentro del directorio del repositorio, corre `eb init`.
    - Te preguntará si quieres configurar CodeCommit, te puedes saltar esto.
    - Para responder las demás preguntas, puedes utilizar estos valores de ejemplo:
        ```
        Environment details for: Lebaron-Galeana-Production
        Application name: Lebaron-Galeana-Production
        Region: us-west-2
        Deployed Version: app-cad8-230529_084221228661
        Environment ID: e-6rkdvk7dh3
        Platform: arn:aws:elasticbeanstalk:us-west-2::platform/Python 3.8 running on 64bit Amazon Linux 2/3.3.7
        Tier: WebServer-Standard-1.0
        CNAME: Lebaron-Galeana-Production.us-west-2.elasticbeanstalk.com
        Updated: 2023-05-29 14:42:41.411000+00:00
        Status: Ready
        Health: Green
        ```

El proceso para realizar el deploy es:

- Crear un Pull Request con tus cambios desde tu branch a la branch `Staging` y mergear el Pull Request.
- Hacer checkout a la branch de `Prod`.
- Hacer pull de la branch de `Staging`.
    - Si salen conflictos, toma en cuenta que es necesario utilizar URLs diferentes en producción.
- Correr `eb deploy` para mandar los cambios a producción.
