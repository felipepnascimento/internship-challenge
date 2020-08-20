# A Tarefa - Sistema de Gerencimento de Usuários
- Crie um aplicativo responsivo para gerenciar usuários
- O usuário deve ter:

1. full_name
2. email
3. avatar_image (upload do arquivo)
4. role (admin/student)

##  A Aplicação
### Casos de uso do Admin
- Como `admin`, devo ser capaz de acessar um painel de administração do usuário, o **Dashboard**
- Como `admin`, devo ser capaz de ver no Dashboard:
   - Número total de usuários
   - Número total de usuários agrupados por `role`
- Como `admin`, devo ser redirecionado para o Dashboard após o login
- Como `admin`, devo ser capaz de listar, criar, editar e excluir usuários
- Como `admin`, devo ser capaz de alternar a `role` do usuário
- Como `admin`, devo ser capaz de importar uma planilha para o sistema, a fim de criar novos usuários

### Casos de uso do Student
- Como `student`, devo ser redirecionado para o meu perfil após o login
- Como `student`, devo poder apenas ver minhas informações, editar e deletar meu perfil

## O que vamos usar?
- Ruby on Rails
   - Linguagem para desenvolvimento do frontend com `.erb` e o backend

- Postgres
   - Banco de dados para armazenamento dos dados da aplicaço

- Docker
   - Para subir a aplicação localmente

- Javascript
   - Validação da planilha no frontend com uma função javascript pura
   - Validação do formulário de cadastro de usuário

- Bootstrap
  - Para deixar responsivo

- Devise:
   - Autenticação de usuários
   - sign_up, sign_in, sign_out

- Sidekiq
   - Utilização de jobs para o processamento de arquivos

- Cancancan
   - Autorização de usuários

- RSpec
   - Testes automatizados

## Cereja do bolo

- CI/CD com GitHub Actions
- Deploy no Heroku

## Live Preview
Acessa a [aplicação](https://quero-app.herokuapp.com/) de modelo para ter acesso aos seguintes items:

- Mockup das telas a serem desenvolvidas
- Usabilidade da aplicação
- fluxo de vida da aplicação