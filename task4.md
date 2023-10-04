## Создана виртуалка, установлен докер.
## Создаем сеть docker network create my-app
## Поднят контейнер постгрес docker run -d --name postgres --network my-app  -p 5432:5432 -e POSTGRES_PASSWORD=1234 -v postgres:/var/lib/postgresql/data postgres:14
## Контейнер запущен, база работает.
## Контейнер с клиентом docker run -it --rm jbergknoff/postgresql-client postgresql://postgres:1234@51.250.102.19:5432/
## Создана таблица с парой строк.
## Подключиться к базе с внешнего клиента psql -h 51.250.102.19 -U postgres
## docker rm --force postgres
## Контейнер создан снова
## Табличка доступна. 
