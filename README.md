# PruebaTecnicaSalcaja

Prueba técnica fullstack desarrollada utilizando:

## Backend
- Java
- Spring Boot
- PostgreSQL

## Frontend
- Angular
- TypeScript
- Bootstrap

## Funcionalidades
- Gestión de grupos del mundial
- Gestión de equipos
- Asignación de equipos a grupos
- Consumo de API REST
- Validaciones frontend y backend

---

# Configuración de Base de Datos

El proyecto utiliza PostgreSQL.

Debe crearse una base de datos y un esquema con el nombre de preferencia del usuario.

Ejemplo:

```sql
CREATE DATABASE mundial_db;
```

Luego configurar las credenciales de PostgreSQL en el archivo:

```text
backend/src/main/resources/application.properties
```

Ejemplo:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/mundial_db?currentSchema=mundial_db
spring.datasource.username=postgres
spring.datasource.password=123456
spring.jpa.hibernate.ddl-auto=update
```

---

# Ejecución del Proyecto

## Backend

Ingresar a la carpeta backend y ejecutar:

```bash
mvn spring-boot:run
```

---

## Frontend

Ingresar a la carpeta frontend y ejecutar:

```bash
npm install
ng serve
```

La aplicación estará disponible en:

```text
http://localhost:4200
```