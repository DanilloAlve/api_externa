# api_externa
# API com Flask e Swagger

Este projeto consta como requisito para Pós-graduação em Desenvolvimento FullStack PUC-RIO. é uma API REST desenvolvida em **Flask**, com integração à API externa **JSONPlaceholder**, que serve para simular interações com recursos como posts. O projeto também utiliza o **Swagger** para documentar a API.

API externa pode ser acessada pelo link: https://jsonplaceholder.typicode.com/

## Funcionalidades da API

A API oferece as seguintes operações (rotas):

- **GET /api/posts**: Obtém uma lista de posts.
- **POST /api/posts**: Cria um novo post.
- **PUT /api/posts/{post_id}**: Atualiza um post existente pelo ID.
- **DELETE /api/posts/{post_id}**: Remove um post pelo ID.

## Tecnologias Utilizadas

- **Flask**: Framework de desenvolvimento web.
- **Flask-Swagger-UI**: Para gerar a documentação Swagger da API.
- **JSONPlaceholder**: API externa usada para simular dados.
- **Docker**: Para containerizar a aplicação.

## Instalação e Execução

### 1. Clone o repositório

git clone https://github.com/seu-usuario/seu-repositorio.git

### 2. Crie e ative um ambiente virtual (opcional, mas recomendado)

python3 -m venv venv
venv\Scripts\activate  

### 3. Instale as dependências

pip install -r requirements.txt

### 4. Execute a aplicação
Para iniciar o servidor Flask, execute:

python app.py
A API estará disponível em http://localhost:5000.

### Uso da API

GET /api/posts
Obtém uma lista de posts fictícios.

POST /api/posts
Cria um novo post na JSONPlaceholder.

### Rodando com Docker


### 1. Construir a imagem Docker

docker build -t api-externa-flask .

### 2. Executar o contêiner

docker run -p 5000:5000 api-externa-flask
A API estará disponível em http://localhost:5000.
