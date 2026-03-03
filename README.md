# API Escuela Oficial de Conductores - Gestión de Ubicaciones

Proyecto full stack personal: Backend en Java Spring Boot + Frontend en Angular para simular un sistema de gestión de ubicaciones (Departamento, Provincia, Distrito) como en la Escuela Oficial de Conductores del Perú.

## Tecnologías usadas
- **Backend**: Java 17/21, Spring Boot 3.x, Spring Data JPA, PostgreSQL/MySQL, DTOs, MapStruct (mapper), Validaciones (@Valid), Excepciones globales, Paginación básica.
- **Frontend**: Angular 17+, Reactive Forms, HttpClient, Routing, ngx-toastr (notificaciones), Bootstrap o CSS responsive.
- **Herramientas**: Maven, Git, Postman para testing de API, Angular CLI.

## Estructura del proyecto
- **Backend** (`com.galaxy.api_escuelaConductores`):
  - Controller: EscuelaController (endpoints CRUD)
  - DTOs y Mapper
  - Entity, Repository, Service
  - Config global y excepciones
- **Frontend** (`app-conductores`):
  - Componentes: ubicacion-lista, ubicacion-registro
  - Service: UbicacionService (HTTP requests)
  - Forms reactivos para registro/edición

## Cómo correrlo localmente
1. **Backend**:
   - Clona el repo
   - Configura `application.properties` (DB: url, user, pass)
   - `mvn clean install`
   - `mvn spring-boot:run` → corre en http://localhost:8080 (o el puerto que uses)

2. **Frontend**:
   - `cd frontend/app-conductores`
   - `npm install`
   - `ng serve` → corre en http://localhost:4200

3. Accede a: http://localhost:4200/home/ubicacion para ver el listado y formulario.


Demuestra arquitectura limpia (capas separadas), manejo de DTOs para no exponer entidades, frontend consumiendo API REST, y manejo de estados/forms en Angular.

