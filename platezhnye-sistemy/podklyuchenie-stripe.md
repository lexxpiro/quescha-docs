---
description: https://stripe.com
---

# Подключение Stripe

Для подключения платежной системы вам потребуются Publishable key и Secret key. Они находятся в аккаунте платежной системы.

<figure><img src="../.gitbook/assets/Developers-–-New-Business-–-Stripe-Test- (1).png" alt=""><figcaption></figcaption></figure>

Добавьте интеграцию в аккаунте Квесча.

Скопируйте и вставьте URL для уведомлений и установите их в аккаунте Stripe. Для этого перейдите на страницу для разработчиков (Developers), нажмите на Add an endpoint на вкладке Webhooks.

<figure><img src="../.gitbook/assets/Developers-–-New-Business-–-Stripe-Test- (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Developers-–-New-Business-–-Stripe-Test-.png" alt=""><figcaption></figcaption></figure>

Вставьте URL для уведомлений конструктора.

<figure><img src="../.gitbook/assets/Dashboard-–-New-Business-–-Stripe-Test-.png" alt=""><figcaption></figcaption></figure>

Выберите событие checkout.session.completed и сохраните настройки.

<figure><img src="../.gitbook/assets/Developers-–-New-Business-–-Stripe-Test- (3).png" alt=""><figcaption></figcaption></figure>

Далее вы должны настроить генерацию платежной ссылки в сценарии действий, а также принять платеж.

Для приема платежа установите галочку в отдельном блоке "Ожидание платежа" и, при необходимости, подключите к нему сценарий действий, где настройте действие "Платежи" -> "Принять платеж".
