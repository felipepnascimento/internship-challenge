# A Tarefa - Sistema de Gerencimento de Usuários
O objetivo desta tarefa é criar um sitema para gerencimento de usuários. Devemos ter dois perfis de acesso: `admin` e `student` com regras e funcionalidades diferentes dentro da aplicação. O cadastro de cada usuário deverá ter os seguintes atributos:

| Nome      | Tipo    | Descrição
|-----------|---------|-----------
| full_name | String  | Nome completo do usuário.
| email     | String  | email válido do usuário
| role      | Integer | valor do enum da role do usuário

A Aplicação compõe-se por uma página inicial, onde será feito o cadastro e login dos usuários e por duas páginas com o usuário autenticado: perfil do usuário logado e dashboard para o administrador do sistema.

## A Aplicação

### Login com Devise
- Utilizar a biblioteca `Devise` para realizar o login.

### Cadastro de usuário
- O sistema deverá iniciar ao menos com um usuário com a `role` de `admin`.
- Todo usuário cadastrado, deverá ter a `role` como `student`.
- Somente o admin poderá alterar a `role` de novos usuários.

### Criação da tela de dashboard
- Somente será exibido para um usuário autenticado.
- Somente será exibido para usuários com a `role`: `admin`.

### Casos de uso - *Roles*

#### *Role Admin*
- Devo ser capaz de acessar Dashboard.
- Devo ser capaz de ver no Dashboard:
   - Número total de usuários.
   - Número total de usuários agrupados por `role`.
- Devo ser redirecionado para o Dashboard após o login.
- Devo ser capaz de listar, criar, editar e excluir usuários.
- Devo ser capaz de importar uma planilha para o sistema, a fim de criar novos usuários.

#### *Role Student*
- Devo ser redirecionado para o meu perfil após o login.
- Devo poder apenas ver minhas informações, editar e deletar meu perfil.

## Requisitos

- Ruby on Rails
   - Linguagem para desenvolvimento do frontend com `.erb`. (pode utilizar o vue/react/etc para fazer o frontend)
   - Linguagem para desenvolvimento do backend.

- Postgres
   - Banco de dados para armazenamento dos dados da aplicaço.

- Docker
   - Para subir a aplicação localmente.

- Javascript
   - Validação da planilha no frontend com uma função javascript pura.
   - Validação do formulário de cadastro de usuário.

- Bootstrap (não obrigatório)
  - Para deixar responsivo.
  > Pode utilizar outro lib para deixar responsivo 

- Devise:
   - Autenticação de usuários.
   - sign_up, sign_in, sign_out.

- Sidekiq
   - Utilização de jobs para o processamento de arquivos.

- Cancancan
   - Autorização de usuários.

- RSpec
   - Testes automatizados.

- Versionamento do projeto no Github

A partir de agora é mão na massa, [clique aqui](1-development.md) e veja os passos iniciais.
