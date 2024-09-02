# pymongo-api

## Как запустить

Запускаем mongodb и приложение

```shell
docker compose up -d
```

Инициализируем шарды mongodb и заполняем тестовыми данными:

```shell
./scripts/mongo-init-configSrv.sh
```

```shell
./scripts/mongo-init-shards.sh
```

```shell
./scripts/mongo-init-router.sh
```

```shell
./scripts/mongo-init-fixtures.sh
```

## Как проверить

### Если вы запускаете проект на локальной машине

Откройте в браузере http://localhost:8080

### Если вы запускаете проект на предоставленной виртуальной машине

Узнать белый ip виртуальной машины

```shell
curl --silent http://ifconfig.me
```

Откройте в браузере http://<ip виртуальной машины>:8080

## Доступные эндпоинты

Список доступных эндпоинтов, swagger http://<ip виртуальной машины>:8080/docs