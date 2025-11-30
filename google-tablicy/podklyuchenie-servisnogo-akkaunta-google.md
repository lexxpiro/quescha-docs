# Подключение сервисного аккаунта Google

Для работы с Гугл Таблицей вы можете использовать, подключенный на странице интеграций Гугл аккаунт, но вы также можете использовать свой **сервисный гугл аккаунт.**

Давайте создадим его.

Перейдите на страницу [https://console.developers.google.com/iam-admin/serviceaccounts?hl=ru](https://console.developers.google.com/iam-admin/serviceaccounts?hl=ru) и нажмите кнопку Create Project.

<figure><img src="../.gitbook/assets/Service-Accounts-–-IAM-Admin-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/New-Project-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

После этого нажмите кнопку Create Service Account

<figure><img src="../.gitbook/assets/Service-accounts-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

При создании, предоставьте сервисному аккаунту права владельца.



<figure><img src="../.gitbook/assets/spaces_-Mi4gurxGu8W8EBsLl6U_uploads_H6babuplo5AiSv7ddNJS_Create-service-account-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console.webp" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Create-service-account-–-IAM-Admin-–-Google-Sheets-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

После создания нажмите на емэйл сервисного аккаунта, чтобы открыть настройки

<figure><img src="../.gitbook/assets/Service-accounts-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

Перейдите на вкладку KEYS и создайте JSON файл с ключами

<figure><img src="../.gitbook/assets/Quescha-Calendar-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/Quescha-Calendar-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/Quescha-Calendar-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console (2).png" alt=""><figcaption></figcaption></figure>





<figure><img src="../.gitbook/assets/Quescha-Calendar-–-IAM-Admin-–-Quescha-Calendar-–-Google-Cloud-console (4).png" alt=""><figcaption></figcaption></figure>

Теперь необходимо включить доступ к API Гугл Таблицы для этого сервисного аккаунта.

Введите в поле поиска calendar  и найдите Google Sheets API

<figure><img src="../.gitbook/assets/GoogleSheets-–-IAM-Admin-–-Google-Sheets-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Включите доступ, нажав на кнопку Enable

<figure><img src="../.gitbook/assets/Google-Sheets-API-–-Marketplace-–-Google-Sheets-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/API-Service-Details-–-APIs-Services-–-Google-Sheets-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Теперь, чтобы использовать сервисный аккаунт в сценарии действий откройте json файл скопируйте содержимое и вставьте в поле сервисного аккаунта в действии Google Таблицы.

Откройте файл с ключами в текстовом редакторе, скопируйте содержимое и вставьте.

<figure><img src="../.gitbook/assets/gsheetskeys.jpg" alt=""><figcaption></figcaption></figure>

Теперь в сценарии действий вставьте содержимое файла в поле Сервисный аккаунт



<figure><img src="../.gitbook/assets/Сценарии-действий (1) (1).png" alt=""><figcaption></figcaption></figure>

Также необходимо предоставить сервисному аккаунту доступ к редактированию вашей таблицы. Скопируйте почту сервисного аккаунта.



<figure><img src="../.gitbook/assets/GoogleSheets-–-IAM-Admin-–-Google-Sheets-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

Откройте вашу гугл таблицу, нажмите в правом верхнем углу на кнопку Настройки доступа и добавьте этот адрес эл. почты в поле пользователей, которым предоставляются права управления таблицей



<figure><img src="../.gitbook/assets/Моя-таблица-Google-Таблицы.png" alt=""><figcaption></figcaption></figure>



<figure><img src="../.gitbook/assets/Моя-таблица-Google-Таблицы (1).png" alt=""><figcaption></figcaption></figure>

Теперь вы можете настраивать сценарий действий по работе с вашей Гугл таблицей
