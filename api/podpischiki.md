---
description: Работа с базой подписчиков
---

# Подписчики



## Удалить подписчика из базы

#### Метод POST

```
/subscriber/delete
```

#### Параметры запроса

```json
{
    "clientid": num | string - ClientID подписчика, обязательный
    "messenger": string - Messenger подписчика: telegram, wa, viber, vk, обязательный
    "botid": string - BotID подписчика, обязательный
}
```



#### Ответ

```json

{
        "result": "Subscriber successfully deleted"
}

```

