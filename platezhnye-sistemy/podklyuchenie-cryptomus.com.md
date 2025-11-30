# Подключение Cryptomus.com

Для подключения платежной системы вам потребуется ID мерчанта и API  ключ

<figure><img src="../.gitbook/assets/Платежные-системы (6).png" alt=""><figcaption></figcaption></figure>

В своем аккаунте cryptomus.com добавьте мерчант и перейдите на вкладку настроек.

<figure><img src="../.gitbook/assets/Cryptomus.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Cryptomus (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Cryptomus (2).png" alt=""><figcaption></figcaption></figure>

Копируем номер ID мерчанта и API ключ и добавляем интеграцию в аккаунте Квесча.

Если API ключ еще не был создан ранее, включите двухфакторную авторизацию и создайте API ключ.

Далее вы должны настроить генерацию платежной ссылки в сценарии действий, а также принять платеж.

Для приема платежа установите галочку в сообщении "Ожидание платежа" и, при необходимости, подключите к нему сценарий действий, где настройте действие "Платежи" -> "Принять платеж".

{% hint style="info" %}
Если у вас возникнут какие-либо вопросы по платежной системе cryptomus.com, обращайтесь [https://t.me/Aivaras\_Mi](https://t.me/Aivaras_Mi)
{% endhint %}
