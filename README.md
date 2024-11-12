/FleetFlowpass
|-- /apps               # Serviços e aplicações principais
|   |-- /registerEnterprise  # Microsserviço de cadastro de empresa
|   |   |-- /controllers       # Controladores do MVC para o microsserviço
|   |   |-- /models            # Modelos de dados (usando Sequelize ou outro ORM)
|   |   |-- /views             # Representações (se houver; pode ser vazio ou ignorado)
|   |   |-- /routes            # Rotas específicas do microsserviço
|   |   |-- /services          # Lógica de negócio separada
|   |   |-- /middlewares       # Middlewares exclusivos do microsserviço (ex: validações)
|   |   |-- /tests             # Testes para o microsserviço
|   |
|   |-- /api                   # API principal com middleware de API key
|   |   |-- /controllers       # Controladores do MVC para a API
|   |   |-- /models            # Modelos de dados, caso algum seja necessário
|   |   |-- /routes            # Rotas da API, incluindo autenticação
|   |   |-- /middlewares       # Middleware de autenticação com API key
|   |   |-- /tests             # Testes para a API principal
|   |
|   |-- /frontend              # Aplicação frontend
|       |-- /src
|           |-- /components    # Componentes reutilizáveis do frontend
|           |-- /pages         # Páginas do frontend
|           |-- /services      # Conexões de API e lógica de front
|           |-- /styles        # Estilos e CSS
|           |-- /tests         # Testes para o frontend

|-- /libs                      # Bibliotecas e pacotes reutilizáveis (opcional)
|   |-- /common                # Código compartilhado entre microserviços (ex: validações comuns)
|   |-- /utils                 # Funções utilitárias e helpers

|-- /configs                   # Configurações gerais do projeto
|   |-- /eslint                # Configurações de lint
|   |-- /prettier              # Configurações de formatação
|   |-- /ci-cd                 # Configurações de CI/CD
|-- /scripts                   # Scripts auxiliares para o projeto
|-- /docs                      # Documentação do projeto
|-- /.gitignore                # Arquivo .gitignore
|-- /package.json              # Arquivo package.json principal do monorepo (se utilizar npm/yarn workspaces)
