# Practica 6

## two services `accounts (2222)` and `web` are running and registered

Se han modificado los archivos:
 - accounts-service.yml
 - web-service.yml

Lanzamos el discovery, config, accounts y servidor.

Si realizamos una peticion del web al accounts podemos ver como no salta
una extepcion, por lo tanto ambos estan corriendo.

![Peticion del web al account](./img/peticion1.png)

## The service registration service has these two services registered

![Eureka](./img/eureka.png)

## Update the configuration repository so that the `accounts` service uses now the port 3333

**link**

## Run a second instance of the `accounts` service using the new configuration. What happens?

Se ve como sin parar la ejecucion hemos sido capaces de que se configure un
accounts al puerto 3333.

![](./img/account3333.png)

## What happens when you kill the service `accounts (2222)` and do requests to `web`?

Que se desconecta y aparece como DOWN.

![](./img/accountDOWN.png)

## Can the web service provide information about the accounts again?. Why?