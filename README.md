<h1 align="center">
  Todo List
</h1>

<p align="center">
 <img src="https://img.shields.io/static/v1?label=Social&message=@evandersondev&color=EA2027&labelColor=000000" alt="@evandersondev" />
 <img src="https://img.shields.io/static/v1?label=Tipo&message=Curso&color=EA2027&labelColor=000000" alt="Curso" />
</p>

API de tarefas usando Java e Spring Boot, um todo-list desenvolvido no curso Formação Spring Boot da Build & Run para aprender as principais práticas para criação de backend.

## Tecnologias

- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)

## Práticas adotadas

- API REST
- Consultas com Spring Data JPA
- Injeção de Dependências

## Como Executar

- Clonar repositório git
- Construir o projeto:

```
$ ./mvnw clean package
```

- Executar a aplicação:

```
$ java -jar target/todolist-1.0.0.jar
```

A API poderá ser acessada em [localhost:8080/tasks](http://localhost:8080/tasks).

## API Endpoints

- Criar Tarefa

```http
POST http://localhost:8080/tasks
Content-Type: application/json

{
  "id": 2,
  "description": "Ir dormir"
}
```

<br>

- Listar Tarefas

```http
GET http://localhost:8080/tasks
```

- Atualizar Tarefa
  <br>

```http
PUT http://localhost:8080/tasks/1
Content-Type: application/json

{
  "description": "Study Spring Boot Atualizado"
}
```

- Deletar Tarefa por ID

```http
DELETE http://localhost:8080/tasks/1
```

- Deletar todas as tarefas

```http
DELETE http://localhost:8080/tasks
```
