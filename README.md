 Для запуска подключите бд и сделайте миграции 
1.  Создание задачи - POST http://localhost:8001/api/tasks {
    "title": "Первая задача",
    "description": "Описание первой задачи",
    "status": "pending"
}

2.  Получение списка задач - GET  http://localhost:8001/api/tasks

3.  Просмотр одной задачи - GET   http://localhost:8001/api/tasks/1 <- 1 это id задачи

4. Обновление задачи - PUT http://localhost:8001/api/tasks/1 <- 1 это id задачи
{
    "title": "Обновленный заголовок",
    "status": "in_progress"
}

5. Удаление задачи - DELETE http://localhost:8001/api/tasks/1 <- 1 это id задачи
