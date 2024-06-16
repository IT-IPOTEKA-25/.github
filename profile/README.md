# Documentation

### Управление антропогенной нагрузкой на ООПТ для Камчатского края в рамках ЛЦТ 2024
##### Prerequisites
- GoLang
- ReactJS
  - Yandex Map
  - grpc-web
- PostgresSQL

Also you need install docker

##### Installation

Firstly,
```
mkdir folder-project
cd folder-project
```
clone our repositories for frontend and backend to new folder-project:

```
git clone https://github.com/IT-IPOTEKA-25/kamchatka-backend.git
git clone https://github.com/IT-IPOTEKA-25/frontend.git
git clone https://github.com/IT-IPOTEKA-25/kamchatka-satellite.git
```

You will get structure in Explorer/Finder:
```
- folder-project
-- kamchatka-backend
-- frontend
-- kamchatka-satellite
- docker-compose.yml // You should will create this file some later
```

##### How to run
Create simple docker-compose.yml and put into the root folder.
`docker-compose.yml`:
```
services:
  frontend:
    build:
      context: ./frontend
      args:
        app_env: ${APP_ENV}
    volumes:
      - ./frontend/src:/frontend/src
    ports:
      - "3000:3000"
```

###### FRONTEND
For frontend project use docker-compose.yml. This file should be located in the root project-folder
```
docker compose up --build -d 
```

###### BACKEND
Go to the `main` folder which is located inside `kamchatka-backend` and run command using `go`
```
go run .
```
You will see log:
```
Successfully connected to the database!
2024/06/16 23:04:03 server listening at [::]:50051
```

#### About us

- Tatiana Ian
- Anna Koshkina 
