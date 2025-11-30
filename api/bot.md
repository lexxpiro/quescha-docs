---
description: Работа с ботом
---

# Бот



## Количество подписчиков

#### Метод GET, POST

```
/bot/count
```

#### Параметры запроса

```json
{
    "botid": string - BotID подписчика, обязательный
}
```



#### Ответ

```json

{
        "count": num
}

```

## Остановка отложенного запуска следующего сообщения у подписчика

#### Метод GET, POST

```
/message/next/clear
```

#### Параметры запроса

```json
{
    "clientid": string - ClientID подписчика, обязательный
    "botid": string - BotID подписчика, обязательный
}
```



#### Ответ

```json

{
        "result": "cleared"
}
```
