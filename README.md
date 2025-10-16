# API de Gerenciamento de Tarefas - UNINTER

## 📝 Sobre o Projeto

Este projeto é uma API RESTful para gerenciamento de tarefas, desenvolvida para a Atividade Prática da disciplina de **Desenvolvimento Web Back-End** da Uninter.

O objetivo foi construir um serviço back-end funcional que permitisse criar, consultar, atualizar e deletar tarefas, seguindo todos os requisitos solicitados.

## 🛠️ Tecnologias Utilizadas

Para a construção da API, utilizei a seguinte stack de tecnologias:

* **Java 17** e **Spring Boot**: Para criar a estrutura da aplicação de forma rápida e robusta.
* **Spring Data JPA**: Para facilitar a comunicação com o banco de dados e a manipulação das tarefas.
* **MySQL**: Como banco de dados relacional para armazenar os dados das tarefas.
* **Maven**: Para o gerenciamento das dependências do projeto.
* **Postman**: Para realizar os testes de todos os endpoints e para a documentação da API.

## 🏗️ Estrutura da Aplicação

A aplicação foi organizada seguindo as melhores práticas do Spring, dividindo as responsabilidades em:

* **Model (`Tarefa.java`)**: A entidade que representa uma tarefa e sua estrutura de dados (id, nome, data de entrega, responsável).
* **Repository (`TarefaRepository.java`)**: A interface que, usando o JpaRepository, lida com todas as operações de banco de dados (CRUD) de forma automática.
* **Controller (`TarefaController.java`)**: A classe que expõe os endpoints REST (`/tarefas`) e lida com as requisições HTTP (GET, POST, PUT, DELETE).

## 🔗 Endpoints da API

A API oferece as seguintes funcionalidades através dos endpoints no recurso `/tarefas`:

| Método | Endpoint         | Descrição                  |
| :----- | :--------------- | :------------------------- |
| `POST` | `/tarefas`       | Cria uma nova tarefa.      |
| `GET`  | `/tarefas`       | Lista todas as tarefas.    |
| `GET`  | `/tarefas/{id}`  | Busca uma tarefa por ID.   |
| `PUT`  | `/tarefas/{id}`  | Atualiza uma tarefa por ID.|
| `DELETE`| `/tarefas/{id}`  | Deleta uma tarefa por ID.  |

## 📦 Coleção do Postman

Todos os endpoints foram testados e documentados no Postman. A coleção contendo as requisições prontas pra uso está disponível neste repositório.

➡️ **[API-Tarefas.postman_collection.json](https://github.com/user-attachments/files/22959274/Gerenciador.de.Tarefas.postman_collection.zip)**

---
