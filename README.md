///Регистрация

//Запрос
{
"user": {
"username": "test24678",
"email": "test24678@yandex.ru",
"password": "testpswd1234"
}
}
//Ответ
{
"user": {
"username": "test24678",
"email": "test24678@yandex.ru",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzYWQ2NDgzMjA3NTk0MWIwMGU0N2U4OCIsInVzZXJuYW1lIjoidGVzdDI0Njc4IiwiZXhwIjoxNjc3NDkxODQ0LCJpYXQiOjE2NzIzMDc4NDR9.dF5AieKjCfuDA9b_seM1DxeKB4cOimeHKhxSM4Yzvc4"
}
}
//===================================================

///Авторизация

//Запрос
{
"user": {
"email": "test24678@yandex.ru",
"password": "testpswd1234"
}
}
//Ответ
{
"user": {
"username": "test24678",
"email": "test24678@yandex.ru",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzYWQ2NDgzMjA3NTk0MWIwMGU0N2U4OCIsInVzZXJuYW1lIjoidGVzdDI0Njc4IiwiZXhwIjoxNjc3NDkyMjkxLCJpYXQiOjE2NzIzMDgyOTF9.Ib1sjI_Q9pDtvWUbR_SVlYbtscyXAKREjEOqjwS0u3E"
}
}
//===================================================

///Получение токена

//Запрос
{
"user": {
"email": "test24678@yandex.ru",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzYWQ2NDgzMjA3NTk0MWIwMGU0N2U4OCIsInVzZXJuYW1lIjoidGVzdDI0Njc4IiwiZXhwIjoxNjc3NDkyMjkxLCJpYXQiOjE2NzIzMDgyOTF9.Ib1sjI_Q9pDtvWUbR_SVlYbtscyXAKREjEOqjwS0u3E",
"username": "test24678"
}
}

//Ответ

{
"errors": {
"message": "No authorization token was found",
"error": {
"name": "UnauthorizedError",
"message": "No authorization token was found",
"code": "credentials_required",
"status": 401,
"inner": {
"message": "No authorization token was found"
}
}
}
}

Токен можем получить при регистрации или логина

// Запрос по header

(Ключ)Authorization: (Значение)Token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzYWQ2NDgzMjA3NTk0MWIwMGU0N2U4OCIsInVzZXJuYW1lIjoidGVzdDI0Njc4IiwiZXhwIjoxNjc3NDkyMjkxLCJpYXQiOjE2NzIzMDgyOTF9.Ib1sjI_Q9pDtvWUbR_SVlYbtscyXAKREjEOqjwS0u3E
