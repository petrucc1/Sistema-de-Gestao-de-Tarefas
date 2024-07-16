# Sistema de Gestão de Tarefas

Este é um sistema de gestão de tarefas desenvolvido usando Flask no backend e Angular no frontend. Ele permite adicionar, editar, remover e marcar tarefas como concluídas, proporcionando uma experiência interativa ao usuário com uma comunicação eficiente entre o backend e o frontend.

## Funcionalidades

- Adicionar uma nova tarefa
- Editar detalhes de uma tarefa existente
- Remover uma tarefa
- Marcar uma tarefa como concluída

## Pré-requisitos

- Python 3.x
- Node.js
- Angular CLI
- Virtualenv

## Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/sistema-gestao-tarefas.git
cd sistema-gestao-tarefas
```

### Backend (Flask)
Crie e ative um ambiente virtual:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate  # Windows
```

Instale as dependências do backend:
```bash
pip install -r requirements.txt
```

### Frontend (Angular)
Instale as dependências do frontend:
```bash
cd frontend
npm install
```

## Configuração

### Backend (Flask)
No arquivo `.env`, configure as variáveis de ambiente:

```bash
FLASK_ENV=development
FLASK_APP=app.py
```

### Frontend (Angular)
Não são necessárias configurações adicionais além das dependências instaladas.

## Como Usar

### Backend (Flask)

Inicie o servidor Flask:
```bash
flask run
```

O backend estará disponível em `http://localhost:5000`.

### Frontend (Angular)

Inicie o servidor de desenvolvimento do Angular:
```bash
ng serve
```

O frontend estará disponível em `http://localhost:4200`.

## Estrutura do Projeto

```
sistema-gestao-tarefas/
├── backend/
│ ├── app.py
│ ├── models.py
│ ├── routes.py
│ ├── controllers/
│ └── requirements.txt
└── frontend/
├── src/
│ ├── app/
│ ├── assets/
│ ├── environments/
│ └── ...
├── angular.json
├── package.json
└── ...
```

## Rotas da API
* `POST /api/tasks/new`: Adiciona uma nova tarefa.
* `PUT /api/tasks/:id`: Atualiza os detalhes de uma tarefa existente.
* `DELETE /api/tasks/:id`: Remove uma tarefa.
* `GET /api/tasks`: Retorna a lista de todas as tarefas.
* `PUT /api/tasks/:id/complete`: Marca uma tarefa como concluída.

## Telas e Componentes

O frontend utiliza componentes Angular para exibir e manipular as tarefas, com páginas dedicadas para adição, edição e listagem de tarefas.
