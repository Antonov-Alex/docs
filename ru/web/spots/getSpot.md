## spots.getSpot: Свойства заведения

> Пример запроса:

```php
<?php
$url = 'https://joinposter.com/api/spots.getSpot'
 . '?token=687409:4164553abf6a031302898da7800b59fb'
 . '&spot_id=1';

$data = sendRequest($url);
```

> Пример ответа:

```json
{  
   "response":{  
      "spot_id":1,
      "name":"Кафе на Полянке",
      "address":"Москва, ул. Б.Полянка 44"
   }
}
```

Метод возвращает свойства заведения

### HTTP запрос

`GET https://joinposter.com/api/spots.getSpot`

### GET-параметры запроса spots.getSpot

Параметр | Описание
-------- | --------
spot_id | Обязательный параметр, обозначает id заведения

### Параметры ответа spots.getSpot

Параметр | Описание
-------- | --------
response | Объект ответа

Внутри параметра `response` лежит объект, в каждом элементе которого есть следующие параметры:

Параметр | Описание
-------- | --------
spot_id | Id заведения
name | Название заведения
address | Адрес заведения
