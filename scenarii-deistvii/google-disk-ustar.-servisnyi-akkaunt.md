---
hidden: true
---

# Google Диск (Устар. сервисный аккаунт)

Конструктор позволяет загружать файлы на Гугл Диск, получить ссылку на файл. Также можно удалять загруженные ранее файлы.

Чтобы иметь возможность работать с Гугл Диском, вам потребуется сервисный аккаунт Гугл. Давайте создадим его.

Перейдите по ссылке [https://console.cloud.google.com/](https://console.cloud.google.com/)



<figure><img src="../.gitbook/assets/Dashboard-–-Google-Sheets-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Создадим новый проект. Если у вас уже есть сервисный аккаунт, то вы можете добавить туда поддержку Google Drive API через поиск вверху и включить его.

<figure><img src="../.gitbook/assets/Dashboard-–-Google-Sheets-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/New-Project-–-Google-Cloud-console (2).png" alt=""><figcaption></figcaption></figure>

Выберем созданный проект.

<figure><img src="../.gitbook/assets/Dashboard-–-Google-Drive-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Dashboard-–-Google-Drive-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

В поле поиска вверху вводим google drive api и выбираем его из списка.

<figure><img src="../.gitbook/assets/Dashboard-–-Google-Drive-–-Google-Cloud-console (2).png" alt=""><figcaption></figcaption></figure>

Включаем Google Drive API, нажав ENABLE.

<figure><img src="../.gitbook/assets/Google-Drive-API-–-Marketplace-–-Google-Drive-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Теперь мы должны создать ключи доступа для сервисного аккаунта. Для этого переходим в меню Service Accounts.

<figure><img src="../.gitbook/assets/Create-credentials-–-APIs-Services-–-Google-Drive-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Нажимаем CREATE SERVICE ACCOUNT.

<figure><img src="../.gitbook/assets/Service-accounts-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Вводим название и нажимаем CREATE AND CONTINUE.

<figure><img src="../.gitbook/assets/Create-service-account-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Выбираем роль сервисного аккаунта Owner. Нажимаем CONTINUE.

<figure><img src="../.gitbook/assets/Create-service-account-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

Нажимаем DONE.

<figure><img src="../.gitbook/assets/Create-service-account-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console (2).png" alt=""><figcaption></figcaption></figure>

Открываем настройки сервисного аккаунта, нажав на емэйл.

<figure><img src="../.gitbook/assets/Service-accounts-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

Переходим на вкладку KEYS и в выпадающем меню ADD KEY нажимаем Create new key.

<figure><img src="../.gitbook/assets/google-drive-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console.png" alt=""><figcaption></figcaption></figure>

Тип создаваемых ключей оставляем JSON.

<figure><img src="../.gitbook/assets/google-drive-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console (1).png" alt=""><figcaption></figcaption></figure>

Нажимаем CREATE.

<figure><img src="../.gitbook/assets/google-drive-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console (2).png" alt=""><figcaption></figcaption></figure>

Json файл сохранится на ваш компьютер.

<figure><img src="../.gitbook/assets/google-drive-–-IAM-Admin-–-Google-Drive-–-Google-Cloud-console (3).png" alt=""><figcaption></figcaption></figure>

Откройте файл с ключами с помощью текстового редактора, выделите все и скопируйте содержимое в буфер обмена.

<figure><img src="../.gitbook/assets/servicekeydrive.jpg" alt=""><figcaption></figcaption></figure>

Теперь вы можете использовать этот сервисный аккаунт в конструкторе. Добавьте действие Google Диск  и вставьте содержимое JSON файла в поле Сервисный аккаунт. Также заполните поля с названием файла и ссылкой на сохраняемый файл. Ссылку на файл можно принимать при пересылке файлов от пользователя в боте. При использовании действия Прием и пересылка файлов, URL файла сохраняется в переменную #{media\_url}.

Также укажите названия для переменных, в которые будет сохранен URL файла Гугл Диска и ID файла.

Дополнительно можете указать переменные об успехе операции и JSON ответа сервера.

<figure><img src="../.gitbook/assets/Доска (9).png" alt=""><figcaption></figcaption></figure>

После создания файла в Гугл Диске вы получаете ссылку на файл, которая доступна для чтения для всех открывших ее. Также вы можете указать емэйл Гугл Аккаунта, для которого будут назначены права редактора и этот файл будет отображен в Гугл Диске этого аккаунта на странице Доступные мне.

<figure><img src="../.gitbook/assets/Доступные-мне-–-Google-Диск.png" alt=""><figcaption></figcaption></figure>
