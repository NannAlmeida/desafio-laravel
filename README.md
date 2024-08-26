# Desafio: Sistema de Gerenciamento de Tarefas Simples

**Objetivo:** Criar um sistema básico de gerenciamento de tarefas onde os usuários possam criar, visualizar, editar e excluir tarefas. As tarefas devem ser categorizadas, e cada tarefa deve ter uma data de vencimento.

## Instruções

### 1. Autenticação
- Implemente um sistema de login e registro usando o sistema de autenticação padrão do Laravel.
- Somente usuários autenticados podem acessar as funcionalidades do sistema de gerenciamento de tarefas.

### 2. Modelos e Migrações
- Crie dois modelos principais: `Task` e `Category`.
- Um `Task` deve ter os seguintes campos:
  - `title` (string)
  - `description` (text)
  - `due_date` (date)
  - `completed` (boolean)
  - `category_id` (foreign key para a tabela `categories`)
- Uma `Category` deve ter:
  - `name` (string)

### 3. Relações
- Relacione as tarefas (`Task`) a uma categoria (`Category`). Um `Task` pertence a uma `Category`, e uma `Category` pode ter muitas `Tasks`.

### 4. Funcionalidades
- **CRUD de Tarefas:**
  - O usuário pode criar, editar, visualizar e excluir tarefas.
- **Listagem de Tarefas:**
  - O usuário pode visualizar a lista de todas as tarefas, filtrá-las por categoria e também visualizar tarefas já completadas.
- **CRUD de Categorias:**
  - O usuário pode criar, editar e excluir categorias.
- **Conclusão de Tarefas:**
  - O usuário pode marcar uma tarefa como concluída.

### 5. Validações
- Valide os dados de entrada ao criar ou editar tarefas e categorias, garantindo que campos obrigatórios sejam preenchidos corretamente.

### 6. Interface do Usuário
- Crie uma interface simples usando Blade, com uma lista de tarefas na página inicial e links para gerenciar tarefas e categorias.
- As tarefas devem ser listadas com destaque para aquelas que estão vencidas ou próximas do vencimento.
- Use tailwind para estilização.

### 7. Extras (Opcional)
- Implemente uma funcionalidade para enviar um lembrete por e-mail ao usuário quando uma tarefa estiver próxima da data de vencimento.
- Adicione a possibilidade de ordenar as tarefas por data de vencimento ou nome.

## Entrega
O código deve estar hospedado em um repositório Git (como GitHub ou GitLab), com instruções claras sobre como configurar e rodar o projeto.
