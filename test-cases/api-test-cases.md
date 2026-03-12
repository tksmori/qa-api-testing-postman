API Test Cases - JSONPlaceholder

TC-01 Obtener lista de posts
Endpoint: /posts
Método: GET

Expected Result:
Status code 200
Response body es un array
Cada objeto contiene:
userId
id
title
body


TC-02 Obtener post por ID
Endpoint: /posts/10
Método: GET

Expected Result:
Status code 200
id = 10
title no vacío
body no vacío


TC-03 Crear post
Endpoint: /posts
Método: POST

Body:
{ "userId": 1, "title": "QA test post", "body": "testing postman" }

Expected Result:
Status 201
id generado en la respuesta


TC-04 Obtener post inexistente
Endpoint: /posts/999999
Método: GET

Expected Result:
El sistema responde correctamente a la solicitud.
La API devuelve una respuesta controlada cuando el recurso no existe.
El body puede devolver un objeto vacío {} u otro mensaje indicando que no hay datos.
No debe producir error del servidor (500).
