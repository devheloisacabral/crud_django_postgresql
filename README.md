**README.md**

# 🚀 Django CRUD-PostgreSQL 

**Nota: Este projeto está em andamento e sofrerá melhorias.**

Este repositório contém um projeto Django que implementa operações CRUD (Create, Read, Update, Delete) utilizando um banco de dados PostgreSQL. O objetivo principal é fornecer uma estrutura inicial para um aplicativo web Django que realiza operações básicas de manipulação de dados.

## Configuração do Ambiente

Certifique-se de ter Python e Django instalados em sua máquina. Você pode instalar as dependências do projeto executando:

```bash
pip install -r requirements.txt
```

Além disso, é necessário ter um servidor PostgreSQL em execução. Você pode configurar as configurações do banco de dados no arquivo `settings.py` do projeto.

## Configuração do Banco de Dados

1. Crie um banco de dados PostgreSQL para o projeto.
2. Atualize as configurações do banco de dados no arquivo `settings.py` com as credenciais apropriadas.

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'seu_banco_de_dados',
        'USER': 'seu_usuario',
        'PASSWORD': 'sua_senha',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

3. Execute as migrações para criar as tabelas no banco de dados:

```bash
python manage.py migrate
```

## Executando o Servidor de Desenvolvimento

Inicie o servidor de desenvolvimento Django com o seguinte comando:

```bash
python manage.py runserver
```

O aplicativo estará acessível em [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Funcionalidades

O projeto fornece endpoints para realizar operações CRUD em um modelo específico. Você pode acessar a interface administrativa padrão do Django em [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/) para gerenciar os dados.

### Endpoints API

- **Listar Todos os Itens:** `GET /api/items/`
- **Detalhes do Item:** `GET /api/items/{id}/`
- **Criar um Novo Item:** `POST /api/items/`
- **Atualizar um Item Existente:** `PUT /api/items/{id}/`
- **Excluir um Item:** `DELETE /api/items/{id}/`

Certifique-se de ajustar o modelo e as rotas de acordo com as necessidades específicas do seu projeto.

by devheloisacabral
