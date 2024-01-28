##  Chapter 4 - Clase 1
- Instalar serverless a nivel de proyecto
- Ejecutar `npm run sls -- create -t aws-nodejs`
- Instalar plugin para appsync `npm i -D serverless-appsync-plugin`
- En `serverless.yml` añado
```
plugins:
  - serverless-appsync-plugin
```
- Para tener mas limpio el codigo serverless defino `serverless.appsync-api.yml`
```
custom:
  appSync:
    -${file(serverless.appsync-api.yml)}
```
