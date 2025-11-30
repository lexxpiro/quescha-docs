# Доступ в закрытый раздел

Реализовать доступ в закрытый раздел можно несколькими способами. Мы рассмотрим самый простой вариант с доступом по паролю.

Создадим цепочку и сценарий с 4 блоками. Из первого блока мы попадаем в блок с требованием ввести пароль. Если пароль верен, то сценарий переходит в третий блок. Если пароль ошибочен, то сценарий переходит на блок ошибки.

<figure><img src="../.gitbook/assets/Автоворонки (6).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Цепочка-сообщений (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (4).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (5).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (6).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (7).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Доска (8) (1).png" alt=""><figcaption></figcaption></figure>

Готово.

Также можно реализовывать проверку доступа через списки, куда помещается пометка о доступе, например, после оплаты.

Можно организовать доступ без ввода пароля, по ClientID подписчика или по наличию тега.

Еще один способ предоставить доступ с условием подписки на канал для Телеграма.
