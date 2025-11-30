# Отправка сообщения в канал Телеграм из бота

Отправлять сообщение в канал Телеграм мы будем используя API Телеграм напрямую. Сделаем это при помощи действия Обмен данными.

Наш бот будет запрашивать пароль для возможности отправить сообщение в наш канал.

Первое, что нужно сделать, это добавить вашего бота в качестве администратора на ваш канал. Делается это так же как добавляется подписчик в настройках вашего канала.

Создадим сценарий, где будем запрашивать пароль, проверять его и просить ввести сообщение. Далее отправляем сообщение на канал с помощью сценария действий. Всего 3 блока сообщений и 1 сценарий действий.

<figure><img src="../.gitbook/assets/Цепочка-сообщений (5).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (12) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (13).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (14) (1).png" alt=""><figcaption></figcaption></figure>

Мы будем использовать документацию Телеграм для отправки сообщения в Телеграм-канал. Она расположена по ссылке [https://core.telegram.org/bots/api#sendmessage](https://core.telegram.org/bots/api#sendmessage)

В сценарии действий используем [https://api.telegram.org/bot\<token>/sendMessage](https://api.telegram.org/bot%3Ctoken%3E/sendMessage)

где вместо \<token> вставляете токен своего бота

<figure><img src="../.gitbook/assets/Сценарии-действий (10) (1).png" alt=""><figcaption></figcaption></figure>

В конце отправляем сообщение об успешной отправке.

Сценарий готов.

{% embed url="https://drive.google.com/file/d/1o4Q2kUbn1xma-LikgSVi3W9UF-N1uXNu/view?usp=share_link" %}

