# Test Execution Report

API: JSONPlaceholder  
Herramienta: Postman  
Tipo de pruebas: API Testing Manual

---

## TC-01 Obtener lista de posts

Endpoint: GET /posts

Expected Result:
- Status code 200
- Response body array
- Contiene campos userId, id, title, body

Actual Result:
- Status code: 200
- Response body: array de posts

Status:
PASS

---

## TC-02 Obtener post por ID

Endpoint: GET /posts/10

Expected Result:
- Status code 200
- id = 10
- title y body no vacíos

Actual Result:
- Status code: 200
- id: 10
- title presente
- body presente

Status:
PASS

---

## TC-03 Crear post

Endpoint: POST /posts

Expected Result:
- Status code 201
- id generado

Actual Result:
- Status code: 201
- id generado: 101

Status:
PASS

---

## TC-04 Post inexistente

Endpoint: GET /posts/999999

Expected Result:
- Respuesta controlada

Actual Result:
- Status code: 200
- Response body vacío {}

Status:
PASS
