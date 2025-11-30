# Отправка писем

С помощью действия Обмен данными мы может выполнять обращения к любым внешним API. Например, мы можем отправить запрос к Unisender, чтобы отправить письмо.

Сам URL GET запроса может выглядеть так:

https://api.unisender.com/ru/api/sendEmail?**format**=json&**api\_key**=6garzmos2g8u7td7ikjra8fxze1n1gud7i8xemxso\&list\_id=1&**email**=#{email}&**sender\_name**=Имя&**sender\_email**=info@mail.ru&**subject**=Уведомление о новой заявке&**body**=У вас новая Заявка.\
Перейдите по ссылке в чат-бот, чтобы ее увидеть. Ссылка на бот в Телеграм: https://t.me/testbot\_bot?start=#{code}\
Код: #{code}

```
https://api.unisender.com/ru/api/sendEmail?format=json&api_key=6garzmos2g8u7td7ikjra8fxze1n1gud7i8xemxso&list_id=1&email=#{email}&sender_name=Имя&sender_email=info@mail.ru&subject=Уведомление о новой заявке&body=У вас новая Заявка.<br>Перейдите по ссылке в чат-бот, чтобы ее увидеть. Ссылка на бот в Телеграм: https://t.me/testbot_bot?start=#{code}<br>Код: #{code}
```

**format** - формат передаваемых данных

**api\_key** - ключ аккаунта Unisender для доступа к API

**email** - эл.почта для отправки

**sender\_name** - имя отправителя

**sender\_email** - адрес эл.почты отправителя

**subject** - тема письма

**body** - письмо с html тегами

<figure><img src="../.gitbook/assets/Сценарии-действий (9).png" alt=""><figcaption></figcaption></figure>
