Запрос на создание задачи:
POST /tasks/

Заголовок:
Content-Type: application/json

Тело запроса:
{
  "title": "Test Task"
}

Если запрос выполнен успешно, ответ будет таким:
{
  "id": 1,
  "title": "Test Task",
  "is_completed": false
}

Если в запросе отсутствует обязательное поле title, будет ошибка:
{
  "title": [
    "This field is required."
  ]
}
