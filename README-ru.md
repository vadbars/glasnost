# Простой запуск Glasnost с помощью Docker

```
docker run -it -e "GLASNOST_SOURCE_BLOCKCHAIN=..." -e "GLASNOST_BLOG_AUTHOR=..." --restart always ontofractal/glasnost:0.1
```

## Настройки

Для выбора блокчейна и блога используются переменные пространства докер контейнера.

* `GLASNOST_SOURCE_BLOCKCHAIN`: `steem` или `golos`
* `GLASNOST_BLOG_AUTHOR`: имя аккаунта в `steem` или `golos`

Такие переменные пространства, как `PORT`, `STEEM_URL` и `GOLOS_URL` могут быть изменены в Dockerfile для создания нового докер имиджа.

# Остановка Glasnost с помощью Docker

```
docker ps 
```

и найти имя контейнера `CONTAINER_NAME` (в колонке `NAMES`)

```
docker stop CONTAINER_NAME
```
```
docker rm CONTAINER_NAME
```
