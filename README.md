

Запрос на создание задачи: 
```plaintext
POST /tasks/
```
Заголовок: 
Content-Type: application/json

Тело запроса: 

```plaintext
{
  "title": "Тестовая задача"
}
```
Если запрос выполнен успешно, ответ будет таким:

```plaintext
{
  "id": 1,
  "title": "Тестовая задача",
  "is_completed": false
}
```
Если в запросе отсутствует обязательное поле title, будет ошибка: 

```plaintext
{
  "title": [
    "Поле title не заполнено!"
  ]
}
```
