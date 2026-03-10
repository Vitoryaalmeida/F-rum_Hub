# Fórum Hub 💬

## Descrição

O **Fórum Hub** é uma aplicação back-end desenvolvida em **Java** que simula o funcionamento de um fórum de discussão, semelhante ao Fórum da Alura.

A aplicação permite que pessoas usuárias autenticadas criem, visualizem, atualizem e excluam tópicos relacionados a cursos, possibilitando a troca de conhecimentos e a resolução de dúvidas.

Este projeto foi desenvolvido como parte do **Challenge Back-End do programa Oracle Next Education (ONE) em parceria com a Alura**.

---

## Funcionalidades

A API do Fórum Hub possui as seguintes funcionalidades principais:

* **Listar todos os tópicos**
* **Listar um tópico específico**
* **Criar um novo tópico**
* **Atualizar um tópico**
* **Deletar um tópico**

Além disso, a aplicação conta com **sistema de autenticação**, garantindo que apenas pessoas usuárias autenticadas possam criar, editar ou excluir tópicos.

---

## Regras de Negócio

Algumas regras importantes da aplicação:

* Cada tópico deve possuir:

  * **Título**
  * **Mensagem**
  * **Nome do curso**
  * **Data de criação**
  * **Autor**

* Apenas **usuários autenticados** podem:

  * Criar tópicos
  * Atualizar tópicos
  * Deletar tópicos

* A **data de criação** é gerada automaticamente pelo sistema.

---

## Tecnologias Utilizadas

* Java
* Spring Boot
* Spring Data JPA
* Spring Security
* JWT (JSON Web Token)
* Banco de dados relacional
* Insomnia (para testes de API)

---

## Estrutura da API

### Listar todos os tópicos

GET

```id="api1"
GET /topicos
```

---

### Buscar tópico por ID

```id="api2"
GET /topicos/{id}
```

---

### Criar novo tópico

```id="api3"
POST /topicos
```

Exemplo de JSON:

```json
{
 "titulo": "Dúvida sobre Java",
 "mensagem": "Estou com dificuldade em entender orientação a objetos",
 "curso": "Java"
}
```

---

### Atualizar tópico

```id="api4"
PUT /topicos/{id}
```

---

### Deletar tópico

```id="api5"
DELETE /topicos/{id}
```

---

## Autenticação

A aplicação utiliza **JWT (JSON Web Token)** para autenticação.

Para acessar endpoints protegidos é necessário enviar o token no header da requisição:

```
Authorization: Bearer TOKEN
```

---

## Testes da API

Os testes das requisições podem ser realizados utilizando ferramentas como:

* **Insomnia**
* **Postman**

---

## Objetivo do Projeto

Este projeto tem como objetivo praticar:

* Desenvolvimento de APIs REST
* Segurança com autenticação
* Modelagem de banco de dados
* Boas práticas de back-end com Java
* Versionamento de código com Git e GitHub

---

## Autor

Projeto desenvolvido por

**Vitórya de Almeida Vieira**
Participante do **Oracle Next Education (ONE)**.
