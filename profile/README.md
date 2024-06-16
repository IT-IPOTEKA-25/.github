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
```

You will get structure in Explorer/Finder:
```
- folder-project
-- kamchatka-backend
-- frontent
-- kamchatka-satellite
- docker-compose.yml
```

##### How to run


```
docker compose up --build -d 
```
#### About su
