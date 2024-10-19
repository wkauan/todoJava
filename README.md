# ToDoList 📝

Um aplicativo de lista de tarefas (ToDo) desenvolvido com **Java Spring Boot**, com funcionalidades de login/cadastro de usuários e gerenciamento de tarefas.

## Funcionalidades 🚀

- **Autenticação de Usuários**: Login e cadastro de novos usuários.
- **Gerenciamento de Tarefas**: Criação, visualização, edição e deleção de tarefas.
- **Segurança**: Utilização de `BCrypt` para criptografia de senhas.

## Tecnologias Utilizadas 🛠️

- **Java 21**: Linguagem principal.
- **Spring Boot**: Framework utilizado para facilitar o desenvolvimento do backend.
- **BCrypt**: Para criptografia de senhas.
- **H2 Database**: Banco de dados em memória para testes rápidos.
- **Maven**: Gerenciamento de dependências e automação de build.
- **Docker**: Para containerização da aplicação.

## Como Rodar o Projeto Localmente 💻

### Pré-requisitos

- **Java 21** instalado
- **Maven** instalado
- **Docker** (opcional, se for rodar via container)

### Passo a Passo

1. Clone o repositório:

   ```bash
   git clone https://github.com/wkauan/todoJava
   cd todoJava

   ```

2. Compile o projeto usando Maven

   ```bash
   mvn clean install

   ```

3. Execute o projeto

   ```bash
   mvn spring-boot:run

   ```

4. Acesse a aplicação
   ```bash
   http://localhost:8080/{rota}
   ```

## Como Usar o projeto via web service 💻

1. Acesse a aplicação
   ```bash
   https://todojava-1mnq.onrender.com/{rota}
   ```

## Rotas Disponíveis 🌐

### Usuários

- **POST** `/users/` - Registro de novos usuários
- **POST** `/users/` - Login de usuários

### Tarefas

- **GET** `/tasks` - Lista todas as tarefas do usuário logado
- **POST** `/tasks` - Cria uma nova tarefa
- **PUT** `/tasks/{id}` - Atualiza uma tarefa existente
- **DELETE** `/tasks/{id}` - Deleta uma tarefa
