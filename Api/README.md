# Sistema de Reservas - API REST
Proyecto Intermodular - Lenguaje de Marcas - Miguel Ángel Tortosa Mira

##  Descripción
Este repositorio contiene la documentación de la API REST para un sistema de reservas 

---

## Estructura del proyecto

```
docs/
 └── api/
      ├── 1-analisis-dominio.md
      ├── README.md
      ├── 2-ejemplos-json/
      │     ├── post-reserva-request.json
      │     ├── post-reserva-response-201.json
      │     ├── get-reservas-response-200.json
      │     └── error-400.json
      ├── images/
      │     └── swagger-ui.png
      └── 3-openapi/
            ├── openapi.yaml
            └── swagger-ui-dist/
                  ├── index.html
                  ├── openapi.yaml
                  └── swagger-ui-dist/
                        ├── (32 archivos)
```

---

##  1. Análisis de Dominio
Archivo: `docs/api/1-analisis-dominio.md`

Incluye:
- Tablas relevantes para la API
- Campos expuestos y no expuestos
- Reglas de validación
- Ejemplos de JSON
- Justificación del diseño

Entidades expuestas:
- USUARIONORMAL  
- RECURSO  
- RESERVA (principal)

---

## 2. Ejemplos JSON
Carpeta: `docs/api/2-ejemplos-json/`

| Archivo | Descripción |
|--------|-------------|
| post-reserva-request.json | JSON enviado al crear una reserva |
| post-reserva-response-201.json | Respuesta al crear una reserva |
| get-reservas-response-200.json | Ejemplo de listado de reservas |
| error-400.json | Ejemplo de error de validación |

---

##  3. Definición OpenAPI
Archivo: `docs/api/3-openapi.yaml`

Incluye:
- Rutas de la API
- Métodos HTTP
- Códigos de respuesta
- Esquemas de datos
- Validaciones

Rutas principales:
- GET /reservas  
- POST /reservas  
- GET /reservas/{id_recurso}/{id_reserva_local}  
- PUT /reservas/{id_recurso}/{id_reserva_local}  
- DELETE /reservas/{id_recurso}/{id_reserva_local}  

---

##  Objetivo del proyecto
Permitir:
- Crear reservas  
- Consultar reservas  
- Modificar reservas  
- Eliminar reservas  


