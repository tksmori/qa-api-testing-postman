# API Test Cases - JSONPlaceholder

## TC-01 Obtener lista de posts

Endpoint: /posts  
Método: GET  

Expected Result:
- Status code 200
- Response body es un array
- Cada objeto contiene:
  - userId
  - id
  - title
  - body


## TC-02 Obtener post por ID

Endpoint: /posts/10  
Método: GET  

Expected Result:
- Status code 200
- id = 10
- title no vacío
- body no vacío


## TC-03 Crear post

Endpoint: /posts  
Método: POST  

Body:

{
"userId": 1,
"title": "QA test post",
"body": "testing postman"
}

Expected Result:
- Status 201
- id generado en la respuesta
