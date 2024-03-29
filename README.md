# Задание
- Сделать REST сервис c основными CRUD операциями
- Использовать сервлеты
- Использовать JDBC
- Нельзя использовать Spring, Hibernate
- Сервлет должен возвращать DTO, не возвращаем Entity, принимать 
также DTO
- Покрыть rest unit тестами (не менее 80 %, использовать Mock, Spy, 
Parameterized Tests)
- Должны быть как минимум слои: service, repository, mapper, dto, entity,
controller или servlet
- Использовать Lombok, кроме случаев переопределения equals и 
hashcode
- Должны быть реализованы связи One-to-Many и Many-to-Many
- Базы данных MySQL или PostgreSQL
- Должны соблюдаться принципы ООП, SOLID
- Для проверки REST API использовать Postman или Insomnia


## Сущности:

- Distillery: Представляет производителя вина содержит название фирмы производителя.
- Vine: Содержит наименование вина и id магазина продажи.
- Shop: Магазинб содержит название магазина. 

Один и тот же вид вин могут производить разные производители, производители могут производить разне виды вин.

## Использование:

### _Производители_

- Получение всех производителей:
>**GET** /distillery/
- Получение производителя по id:
>**GET** /distillery/{id}
- Добавление нового производителя:
>**POST** /distillery
- Изменение производителя по id:
>**PUT** /distillery/{id}
- Удаление производителя по id:
>**DELETE** /distillery/{id}

### _Магазины_

- Получение всех магазинов:
>**GET** /store
- Получение магазина по id:
>**GET** /store/{id}
- Добавление магазина клиента:
>**POST** /store
- Изменение магазина по id:
>**PUT** /store/{id}
- Удаление магазина по id:
>**DELETE** /store/{id}

### _Вина_

- Получение всех вин:
>**GET** /vine
- Получение вина по id:
>**GET** /vine/{id}
- Добавление нового вина:
>**POST** /vine
- Изменение вина по id:
>**PUT** /vine/{id}
- Удаление вина по id:
>**DELETE** /vine/{id}
