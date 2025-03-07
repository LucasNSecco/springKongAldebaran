# 🚀 API com Spring Boot

Este repositório contém uma API desenvolvida com **Spring Boot**, utilizando **H2 Database** para armazenamento temporário de dados.

## 🛠️ Tecnologias

A aplicação foi construída utilizando:

- **Java 17+**
- **Spring Boot 3+**
- **Banco de Dados H2 (em memória)**
- **Maven**

## 📌 Como Executar a Aplicação

Siga os passos abaixo para rodar a API localmente:

1️⃣ **Clone este repositório:**
```sh
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```  

2️⃣ **Compile e inicie o servidor:**
```sh
mvn spring-boot:run
```  

A aplicação será iniciada e estará acessível em `http://localhost:8080`.

## 🗄️ Acessando o Console do Banco H2

Esta API utiliza um banco de dados **H2**, que roda em memória e pode ser acessado por um console web.

🔹 **Para acessar:**

1. Certifique-se de que a API está rodando.
2. No navegador, abra:
   ```
   http://localhost:8080/h2-console
   ```
3. Utilize as seguintes credenciais:
    - **JDBC URL**: `jdbc:h2:mem:kongapi`
    - **Usuário**: `admin`
    - **Senha**: `admin`

## 📡 Endpoints da API

A API disponibiliza os seguintes endpoints para manipulação de autores e livros:

| Método  | Endpoint                        | Descrição                         |
|---------|---------------------------------|----------------------------------|
| **POST** | `/api/v1/autor`                 | Cria um novo autor                |
| **POST** | `/api/v1/autor/{numero}/livro`  | Adiciona um livro a um autor      |
| **GET**  | `/api/v1/autor/{numero}`        | Retorna os dados de um autor      |
| **GET**  | `/api/v1/autor/`                | Lista todos os autores cadastrados |
| **GET**  | `/api/v1/autor/{numero}/livro/` | Lista os livros de um autor       |

---

Caso tenha dúvidas ou sugestões, sinta-se à vontade para contribuir! 🚀
