<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo.

---

1. Clonar el repositorio
2. Ejecutar comando

```
npm i
```

3. Tener Nest CLI instalado

```
npm i -g @nestjs/cli
```

4. tener insataldo Docker

5. Levantar la vase de datos

```
docker-compose up -d
```

6. Clonar el archivo **.env.template** y renombrar la copia a **.env**

7. Llenar las variables de entorno

8. Reconstruir la base de datos

```
http://localhost:3000/api/v2/seed
```

9.  Ejecutar proyecto

```
npm run start:dev
```

## Stack usado

- MongoDB
- Nest
- Docker

## Build

docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build

## Run

docker-compose -f docker-compose.prod.yaml --env-file .env.prod up

## Nota

Por defecto, docker-compose usa el archivo .env, por lo que si tienen el archivo .env y lo configuran con sus variables de entorno de producción, bastaría con

docker-compose -f docker-compose.prod.yaml up --build
