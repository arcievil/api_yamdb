# Проект YaMDb

### Описание
Проект YaMDb собирает отзывы пользователей на произведения в категориях:
- «Книги»
- «Фильмы»
- «Музыка»

### Алгоритм регистрации пользователей:
1. Пользователь отправляет POST-запрос с параметром *email* на */api/v1/auth/email/.*
2. YaMDB отправляет письмо с кодом подтверждения (*confirmation_code*) на адрес *email* .
3. Пользователь отправляет POST-запрос с параметрами *email* и *confirmation_code* на 
*/api/v1/auth/token/*, в ответе на запрос ему приходит *token* (JWT-токен).
Подробная документация API находится по адресу *redoc/*
Автор
Владимир Наумчук
