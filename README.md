
# Spring Java CRUD API

A simple CRUD REST API that I built when learning the basics of Spring Boot


## Requirements

- Java 11
- PostgreSQL Database
- IntelliJ IDEA or another IDE
- Postman


## Installation

to Install this project just edit application.properties as per your requirement and run the project

```bash
  spring.datasource.url= jdbc:postgresql://localhost:5432/your db name
  spring.datasource.username= your db username
  spring.datasource.password= your db password
```
    
## API Reference

#### Insert Item

```http
  POST http://localhost:8080/api/tutorials
```

| key | value     | Description                |
| :-------- | :------- | :------------------------- |
| `title` | `Spring Boot Tutorial` |  |
| `description` | `Spring Boot Tutorial Description` | |


#### Update Item

```http
  PUT http://localhost:8080/api/tutorials/{id}
```

| key | value     | Description                |
| :-------- | :------- | :------------------------- |
| `title` | `Spring Boot Tutorial` |  |
| `description` | `Spring Boot Tutorial Description` | |
| `published` | `true` | |

#### Get All Item
```http
  GET http://localhost:8080/api/tutorials
```

#### Get Item by Id
```http
  GET http://localhost:8080/api/tutorials/{id}
```
#### Find All Published Items
```http
  GET http://localhost:8080/api/tutorials/published
```

#### Find All Items with title={key}
```http
  GET http://localhost:8080/api/tutorials?title={key}
```


