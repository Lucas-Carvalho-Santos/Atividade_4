📝 API de Gerenciamento de Tarefas – Spring Boot + MongoDB
Este projeto é uma API REST simples para gerenciamento de tarefas, construída com Spring Boot e MongoDB. A aplicação permite criar, listar, atualizar e excluir tarefas por meio de requisições HTTP.

📂 Estrutura do Projeto
bash
Copiar
Editar
src/
└── main/
    ├── java/
    │   └── com/example/tarefas/
    │       ├── controller/         # Camada de controle (endpoints)
    │       ├── model/              # Modelos de dados
    │       ├── repository/         # Interfaces de acesso ao banco
    │       ├── service/            # Regras de negócio
    │       └── TarefasApplication.java  # Classe principal
    └── resources/
        └── application.properties  # Configurações da aplicação
⚙️ Tecnologias Utilizadas
Java 21

Spring Boot 3.4.4

Spring Web

Spring Data MongoDB

Spring Validation

MongoDB

Maven

🛠️ Pré-requisitos
Antes de rodar o projeto, certifique-se de ter:

Java 21+ instalado

Maven instalado

MongoDB Community Edition instalado e em execução localmente

🚀 Como Executar o Projeto
bash
Copiar
Editar
# Clone o repositório
git clone https://github.com/seu-usuario/tarefas-api.git

# Acesse a pasta do projeto
cd tarefas-api

# Execute a aplicação
./mvnw spring-boot:run
A aplicação será iniciada na porta padrão http://localhost:8080.

📥 Endpoints Disponíveis
Método	Endpoint	Descrição
GET	/tarefas	Lista todas as tarefas
POST	/tarefas	Cria uma nova tarefa
PUT	/tarefas/{id}	Atualiza uma tarefa existente
DELETE	/tarefas/{id}	Remove uma tarefa pelo ID

📌 Exemplo de Requisição – Criar Tarefa
URL: http://localhost:8080/tarefas

Método: POST

Body (JSON):

json
Copiar
Editar
{
  "titulo": "Estudar Spring Boot",
  "descricao": "Aprender sobre Controllers e Services",
  "status": "Em andamento"
}
