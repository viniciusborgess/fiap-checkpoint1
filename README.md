Aqui está o seu texto formatado corretamente para um README do GitHub em Markdown:


# API de Pedidos

Esta API permite o gerenciamento de pedidos de clientes. Desenvolvida com **Spring Boot**, a API oferece operações de CRUD (Criar, Ler, Atualizar, Deletar) para gerenciar os pedidos em um banco de dados.

## Endpoints

A seguir estão os endpoints disponíveis para interagir com a API de pedidos:

### 1. Criar um novo pedido

- **Método:** `POST`
- **Endpoint:** `/pedidos`
- **Descrição:** Cria um novo pedido com o nome do cliente e o valor total.
  
**Exemplo de requisição:**
```json
{
  "clienteNome": "João Silva",
  "valorTotal": 150.50
}
```

**Exemplo de resposta:**
```json
{
  "id": 1,
  "clienteNome": "João Silva",
  "dataPedido": "2025-03-24",
  "valorTotal": 150.50
}
```

### 2. Buscar todos os pedidos

- **Método:** `GET`
- **Endpoint:** `/pedidos`
- **Descrição:** Retorna todos os pedidos registrados.

**Exemplo de resposta:**
```json
[
  {
    "id": 1,
    "clienteNome": "João Silva",
    "dataPedido": "2025-03-24",
    "valorTotal": 150.50
  },
  {
    "id": 2,
    "clienteNome": "Maria Oliveira",
    "dataPedido": "2025-03-25",
    "valorTotal": 200.00
  }
]
```

### 3. Buscar um pedido pelo ID

- **Método:** `GET`
- **Endpoint:** `/pedidos/{id}`
- **Descrição:** Retorna os detalhes de um pedido específico, identificando-o pelo ID.

**Exemplo de requisição:**
`GET /pedidos/1`

**Exemplo de resposta:**
```json
{
  "id": 1,
  "clienteNome": "João Silva",
  "dataPedido": "2025-03-24",
  "valorTotal": 150.50
}
```

### 4. Atualizar um pedido

- **Método:** `PUT`
- **Endpoint:** `/pedidos/{id}`
- **Descrição:** Atualiza um pedido existente, permitindo modificar o nome do cliente e o valor total do pedido.
  
---

## Prints dos Testes
**(Somente o exemplo 1 tem o print de ambos os ambientes, pois é um exemplo onde os dados mudaram. Se mudar no Postman, irá mudar no Banco de Dados e na API)**

### 1. Criando um Novo Pedido
- Postman

![Postman](https://github.com/user-attachments/assets/0f9650a3-9cd7-4c0d-9c0a-a704fb21d6c7)

- Banco de dados H2

![image](https://github.com/user-attachments/assets/5830d4bb-c61a-4119-857b-6ffc64837a5c)

- Postman 

![API](https://github.com/user-attachments/assets/da179637-0f82-4f35-880e-41019daaf2b4)


### 2. Buscar Todos os Pedidos
- Postman 

![image](https://github.com/user-attachments/assets/f07e3cfc-d97a-49e8-aa49-48c09b9ace91)


### 3. Buscar um Pedido pelo ID
- Postman 

![Postman](https://github.com/user-attachments/assets/be71d685-3bcd-489f-a1d3-786d800613b7)


### 4. Atualizar um Pedido
- Postman 

![Postman](https://github.com/user-attachments/assets/63ae95f7-d0b4-45da-9dae-da952c497c73)


### 5. Deletar um Pedido
- Postman 

![Postman](https://github.com/user-attachments/assets/c0f20f09-349b-4263-bacb-ce6297312361)
![image](https://github.com/user-attachments/assets/7affa843-d06f-496f-8057-65d90d08df54)


