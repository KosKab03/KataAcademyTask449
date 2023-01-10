****\_****Task 4.4.9****\_****

========Registration========

POST https://blog.kata.academy/api/users

JSON:
{
"user": {
"username": "KostyaKabanov",
"email": "Parzival.youtube@mail.ru",
"password": "Kos265265"
}
}

========Autorization========

POST https://blog.kata.academy/api/users/login

JSON:
{
"user": {
"email": "parzival.youtube@mail.ru",
"password": "Kos265265"
}
}

answer:
{
"user": {
"username": "kostyakabanov",
"email": "parzival.youtube@mail.ru",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzYmQyMTVkMjA3NTk0MWIwMGU0Zjk4YSIsInVzZXJuYW1lIjoia29zdHlha2FiYW5vdiIsImV4cCI6MTY3ODUyNjk4NywiaWF0IjoxNjczMzQyOTg3fQ.ahvGOsTRAXQYcjDY6HpxPuAGxw2KePqCmtLyBU3ngdo"
}
}

========GetCurrentUser========

GET https://blog.kata.academy/api/profiles/kostyakabanov

answer:
{
"profile": {
"username": "kostyakabanov",
"image": "https://static.productionready.io/images/smiley-cyrus.jpg",
"following": false
}
}
