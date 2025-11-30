---
description: Методы для работы с WebApp каталогом
---

# WebApp каталог



## Добавить товар

#### Метод POST

```
/catalog/item/create
```

#### Параметры запроса

```json
{
    "webappid": num | string - id приложения каталога, обязательный
    "title": string - название товара, необязательный
    "description": string - описание товара, необязательный
    "price": num | string - цена товара, необязательный
    "oldprice": string - старая цена товара, необязательный
    "hide": boolean - временно скрыть товар из каталога, необязательный
    "pieces": string - остатки товара, необязательный
    "code": string - артикул товара, необязательный
    "rubric": string - рубрика/категория в каталоге, необязательный
    "szpieces": string - остатки по размерам, например, S:10, M:15, L:20, необязательный
    "sizes": string - размеры через запятую, необязательный
    "colors": string - цвета через запятую, необязательный
    "order": num | string - порядковый номер в списке, необязательный
}
```



#### Ответ

```json

{
        "id": num - id товара
        "result": 'Item successfully created'
}

```

## Изменить товар

#### Метод POST

```
/catalog/item/edit
```

#### Параметры запроса

```json
{
    "webappid": num | string - id приложения каталога, обязательный
    "itemid": num | string - id товара, обязательный
    "title": string - название товара, необязательный
    "description": string - описание товара, необязательный
    "price": num | string - цена товара, необязательный
    "oldprice": string - старая цена товара, необязательный
    "hide": boolean - временно скрыть товар из каталога, необязательный
    "pieces": string - остатки товара, необязательный
    "code": string - артикул товара, необязательный
    "rubric": string - рубрика/категория в каталоге, необязательный
    "szpieces": string - остатки по размерам, например, S:10, M:15, L:20, необязательный
    "sizes": string - размеры через запятую, необязательный
    "colors": string - цвета через запятую, необязательный
    "order": num | string - порядковый номер в списке, необязательный
}
```

#### Ответ

```json
{
    "result": 'Item successfully changed'
}
```

## Удалить товар

#### Метод POST

```
/catalog/item/delete
```

#### Параметры запроса

```json
{
    "itemid": num | str - id товара, обязательный
}
```

#### Ответ

```json
{
    "result": 'Item successfully deleted'
}
```

## Добавить товары массово

#### Метод POST

```
/catalog/item/bulk/create
```

#### Параметры запроса

```json
{
    "webappid": num | string - id приложения каталога, обязательный
    "items": [ // array of obj - массив товаров 
        {
            "title": string - название товара, необязательный
            "description": string - описание товара, необязательный
            "price": num | string - цена товара, необязательный
            "oldprice": string - старая цена товара, необязательный
            "hide": boolean - временно скрыть товар из каталога, необязательный
            "pieces": string - остатки товара, необязательный
            "code": string - артикул товара, необязательный
            "rubric": string - рубрика/категория в каталоге, необязательный
            "szpieces": string - остатки по размерам, например, S:10, M:15, L:20, необязательный
            "sizes": string - размеры через запятую, необязательный
            "colors": string - цвета через запятую, необязательный
            "order": num | string - порядковый номер в списке, необязательный
        },...
    ]
}
```

#### Ответ

```json
{
    "id": array of num - массив id товаров
    "result": 'Items successfully created'
}
```

## Изменить товары массово

#### Метод POST

```
/catalog/item/bulk/edit
```

#### Параметры запроса

```json
{
    "webappid": num | string - id приложения каталога, обязательный
    "items": [ // array of obj - массив товаров 
        {
            "itemid": num | string - id товара, обязательный
            "title": string - название товара, необязательный
            "description": string - описание товара, необязательный
            "price": num | string - цена товара, необязательный
            "oldprice": string - старая цена товара, необязательный
            "hide": boolean - временно скрыть товар из каталога, необязательный
            "pieces": string - остатки товара, необязательный
            "code": string - артикул товара, необязательный
            "rubric": string - рубрика/категория в каталоге, необязательный
            "szpieces": string - остатки по размерам, например, S:10, M:15, L:20, необязательный
            "sizes": string - размеры через запятую, необязательный
            "colors": string - цвета через запятую, необязательный
            "order": num | string - порядковый номер в списке, необязательный
        },...
    ]
}
```

#### Ответ

```json
{
    "result": 'Items successfully changed'
}
```

## Удалить товары массово

#### Метод POST

```
/catalog/item/bulk/delete
```

#### Параметры запроса

```json
{
    "items": [ // array of obj - массив товаров 
        {
            "itemid": num | string - id товара, обязательный
        },...
    ]
}
```

#### Ответ

```json
{
    "result": 'Items successfully deleted'
}
```

## Удалить все товары

#### Метод POST

```
/catalog/items/delete
```

#### Параметры запроса

```json
{
    "webappid": num | string - id приложения каталога, обязательный
}
```

#### Ответ

```json
{
    "result": 'Items successfully deleted'
}
```

## Получить ссылку для скачивания каталога

#### Метод POST или GET

```
/catalog/get
```

#### Параметры запроса

```json
{
    "webappid": num | string - id приложения каталога, обязательный
}
```

#### Ответ

<pre class="language-json"><code class="lang-json">{
    "link": str - ссылка на файл каталога
<strong>    "notice": 'link is valid for 2 minutes'
</strong>}
</code></pre>

## Удаление WebApp приложения

#### Методы GET, POST

```
/webapp/delete
```

#### Параметры запроса

{% code overflow="wrap" %}
```json
{
    "id": num | string - id приложения, обязательный
}
```
{% endcode %}



#### Ответ

```json

{
        "result": "deleted"
}

```
