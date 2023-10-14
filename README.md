<div align="center">
 <h1>Todolist</h1>

  <img src="https://img.shields.io/badge/JAVA-ED8B00?style=flat&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=flat&logo=spring&logoColor=white">
</div>

## 📘 Sobre
Backend de uma todolist em Java.

Projeto realizado durante o curso de Java oferecido pela [Rocketseat](https://github.com/Rocketseat).

## 💻 Tecnologias
- Java
- Spring Boot
- H2 Database Engine

## ✅ Funcionalidades
- [x] Cadastro de usuários
- [x] Autenticação de usuários
- [x] Verificação de permissões
- [x] Criptografia de senha
- [x] Cadastro de tarefas
- [x] Atualização de tarefas

## ▶️ Como usar
O deploy da aplicação foi realizado na plataforma [Render](render.com).

Use a URL `https://todolist-rocketseat-iq26.onrender.com` em uma aplicação de requisições HTTP como o Postman ou Inmsonia para testar a aplicação.

### Criar usuário
Primeiro você deve criar um usuário:

Defina o método POST e use a seguinte URL:
```
https://todolist-rocketseat-iq26.onrender.com/users/
```

Passe as informações do usuário no Body no formato JSON.

Exemplo:
```json
{
  "name": "Elaine Ferreira",
  "username": "elaine",
  "password": "123456"
}
```

**Após a criação do usuário selecione sempre o método de autenticação Basic Authentication e passe o username e password do usuário criado para ver, criar e atualizar as tarefas.**

### Criar tarefa
Defina o método POST e use a seguinte URL:
```
https://todolist-rocketseat-iq26.onrender.com/tasks/
```

Passe as informações da tarefa no Body no formato JSON.

Exemplo:
```json
{
  "description": "Assistir aula 5 de Java",
  "title": "Assistir aula de Java",
  "priority": "Alta",
  "startAt": "2023-10-14T12:30",
  "endAt": "2023-10-14T15:35"
}
```

### Ver tarefas criadas
Defina o método GET e use a seguinte URL:
```
https://todolist-rocketseat-iq26.onrender.com/tasks/
```

### Atualizar tarefa
Defina o método PUT e use a seguinte URL, substituindo o `id` pelo id da tarefa gerado automaticamente na criação da tarefa.
```
https://todolist-rocketseat-iq26.onrender.com/tasks/id
```

Passe as informações da tarefa que deseja alterar no Body no formato JSON.

Exemplo:
```json
{
  "description": "Assistir aula 6 de Java"
}
```

### Rodar a aplicação localmente
1 - Clonar o repositório `git clone https://github.com/elainefs/todolist_rocketseat.git`

2 - Rodar `mvn clean install` para instalar as dependências

3 - Rodar `mvn spring-boot:run` para subir a aplicação

4 - A aplicação estará disponível na porta `localhost:8080`

5 - Use uma aplicação de requisições HTTP para fazer os testes 

## 📄 Licença
Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](/LICENSE) para obter mais detalhes.

<hr>

Made with ❤️ by [Elaine Ferreira](https://github.com/elainefs)