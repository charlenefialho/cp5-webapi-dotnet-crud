# Customer Management API

WebAPI em .NET, com a finalidade de realizar um CRUD de clientes para gerenciamento.

## Objetivo
Desenvolver uma WebAPI em .NET, com a finalidade de realizar um CRUD de uma entidade qualquer (prova de .NET).

## Requisitos
- (até 1 ponto) - Implementar o endpoint de inclusão dos dados;
- (até 1 ponto) - Implementar o endpoint de alteração dos dados;
- (até 1 ponto) - Implementar o endpoint de exclusão dos dados;
- (até 1 ponto) - Implementar o endpoint de consulta dos dados;
- (até 2 pontos) - Utilizar o MongoDB para armazenamento dos dados;
- (até 2 pontos) - Trabalhar com a chamada assíncrona dos dados;
- (até 2 pontos) - Ter um projeto de testes unitários, integrados ou de sistema, utilizando xUnit.

## Endpoints

### 1. Get All Customers
- **Endpoint:** `GET /api/customer`
- **Description:** Retorna uma lista de todos os clientes cadastrados.
- **Response:**
  - **Status Code:** `200 OK`
  - **Content:** Uma lista de objetos do tipo `Customer`.

### 2. Get Customer by ID
- **Endpoint:** `GET /api/customer/{id}`
- **Description:** Retorna as informações de um cliente específico com base no ID fornecido.
- **Parameters:**
  - `id` (string) - O ID do cliente a ser recuperado.
- **Response:**
  - **Status Code:** `200 OK` - Se o cliente foi encontrado.
  - **Content:** O objeto `Customer`.
  - **Status Code:** `404 Not Found` - Se o cliente com o ID fornecido não for encontrado.

### 3. Create a New Customer
- **Endpoint:** `POST /api/customer`
- **Description:** Cria um novo cliente com as informações fornecidas.
- **Request Body:** 
  - Um objeto JSON representando o `Customer` a ser criado.
- **Response:**
  - **Status Code:** `201 Created`
  - **Content:** O objeto `Customer` criado.
  - **Location Header:** URL para acessar o novo cliente criado (`/api/customer/{id}`).

### 4. Update an Existing Customer
- **Endpoint:** `PUT /api/customer`
- **Description:** Atualiza um cliente existente com as novas informações fornecidas.
- **Request Body:** 
  - Um objeto JSON representando o `Customer` atualizado.
- **Response:**
  - **Status Code:** `200 OK` - Se o cliente foi atualizado com sucesso.

### 5. Delete a Customer by ID
- **Endpoint:** `DELETE /api/customer/{id}`
- **Description:** Exclui um cliente específico com base no ID fornecido.
- **Parameters:**
  - `id` (string) - O ID do cliente a ser excluído.
- **Response:**
  - **Status Code:** `200 OK` - Se o cliente foi excluído com sucesso.


### 🤝 Contribuente do projeto

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/charlenefialho">
        <img src="https://avatars.githubusercontent.com/u/94643076?v=4" width="100px;" border-radius='50%' alt="Charlene Aparecida's photo on GitHub"/><br>
        <sub>
          <b>Charlene Aparecida</b>
        </sub>
      </a>
    </td>
    
  </tr>
</table>
