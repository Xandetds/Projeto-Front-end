# Plataforma de Streaming de Livros Digitais

## Visão Geral do Projeto

Este projeto apresenta uma aplicação web de front-end construída com **React.js**, simulando uma plataforma de streaming de livros digitais. O objetivo principal é demonstrar proficiência em desenvolvimento de Single Page Applications (SPA), interação com APIs RESTful, gerenciamento de estado e manipulação de dados, além de práticas de desenvolvimento moderno.

## Funcionalidades Chave

A aplicação oferece as seguintes funcionalidades principais:

* **Autenticação de Usuário:** Uma tela de login robusta com validação e feedback de erro, garantindo acesso seguro à plataforma.
* **Interface Responsiva:** Design adaptável para proporcionar uma experiência de usuário consistente e agradável em desktops, tablets e dispositivos móveis.
* **Navegação Intuitiva (SPA):** Utiliza `react-router-dom` para uma navegação fluida entre diferentes seções, como a Home, Explorar Livros e áreas administrativas.
* **Layout Consistente:** Inclui uma barra de navegação (`Navbar`) e rodapé (`Footer`) fixos, garantindo uma estrutura de layout padronizada em toda a aplicação (exceto na tela de login).
* **Gerenciamento de Conteúdo (CRUD de Livros):** Funcionalidades completas de **Criação, Leitura, Atualização e Exclusão** (CRUD) para o catálogo de livros, permitindo a gestão eficiente dos títulos disponíveis na plataforma.
* **Gerenciamento de Usuários (CRUD de Usuários):** Operações CRUD para a administração de contas de usuário, oferecendo controle sobre o acesso e os perfis dentro do sistema.
* **Consumo de API:** Interage com uma API RESTful simulada (JSON Server) para persistência e recuperação de dados, demonstrando habilidades em requisições assíncronas.
* **Tratamento de Erros:** Implementação de `try/catch` para gerenciamento robusto de exceções em todas as requisições HTTP, melhorando a resiliência da aplicação.

## Tecnologias e Ferramentas

* **Front-end Framework:** [React.js](https://react.dev/) - Biblioteca JavaScript para construção de interfaces de usuário reativas e componentizadas.
* **Build Tool:** [Vite](https://vitejs.dev/) - Ferramenta de build de nova geração para um desenvolvimento front-end mais rápido e eficiente.
* **Roteamento:** [React Router DOM](https://reactrouter.com/en/main) - Biblioteca para roteamento declarativo, facilitando a navegação em SPAs.
* **Backend Simulado:** [JSON Server](https://github.com/typicode/json-server) - Ferramenta para criar APIs RESTful mockadas de forma rápida, ideal para desenvolvimento front-end sem um backend real.
* **Linguagens:** HTML5, CSS3, JavaScript (ES6+).
* **Controle de Versão:** [Git](https://git-scm.com/) & [GitHub](https://github.com/) - Para versionamento de código e colaboração.
* **(Opcional: Adicione aqui se usar)** **Frameworks CSS:** Ex: [Tailwind CSS](https://tailwindcss.com/), [Bootstrap](https://getbootstrap.com/), [Material-UI](https://mui.com/), etc.
* **(Opcional: Adicione aqui se usar)** **Bibliotecas de Requisição HTTP:** Ex: [Axios](https://axios-http.com/) (além da Fetch API nativa do JavaScript).

## Estrutura do Repositório

O projeto está organizado na seguinte estrutura de diretórios, promovendo modularidade e clareza:
<pre>
.
Projeto-Front-end/
├── public/
├── src/
│   ├── assets/       # Imagens, ícones, etc.
│   ├── components/   # Componentes reutilizáveis (Navbar, Footer, CardLivro, Formulario)
│   ├── pages/        # Componentes que representam páginas (Login, Home, AdminLivros, DetalhesLivro)
│   ├── services/     # Funções para requisições HTTP (API calls)
│   ├── styles/       # Arquivos CSS ou módulos CSS
│   ├── App.js        # Componente principal e configuração de rotas
│   ├── index.js      # Ponto de entrada da aplicação
│   └── ...
├── db.json           # Banco de dados simulado pelo JSON Server
├── .gitignore        # Arquivos e pastas a serem ignorados pelo Git
├── package.json      # Dependências e scripts do projeto
├── README.md         # Este arquivo
└── ...
</pre>

## Progresso e Próximos Passos

Este `README.md` será atualizado continuamente para refletir o progresso e as próximas etapas de desenvolvimento do projeto.

### Fase 1: Configuração e Estrutura Base (Concluída)

* Repositório GitHub e configurações iniciais (`README.md`, `.gitignore`).
* Configuração do ambiente de desenvolvimento React com Vite e instalação de dependências.
* Definição da estrutura de pastas (`src/components`, `src/pages`, `src/services`, `src/styles`).
* Configuração inicial do `db.json` para o JSON Server.
* Implementação de roteamento (`react-router-dom`) e criação dos componentes `App.jsx`, `Navbar`, `Footer`, `LoginPage`, `HomePage` com estilos iniciais.

### Fase 2: Autenticação de Usuário (Em Andamento)

* Desenvolvimento da lógica de login e validação de credenciais contra o JSON Server.
* Implementação de feedback visual para erros de autenticação.
* Configuração de redirecionamento pós-login.
* Adição de funcionalidade de logout.

### Fase 3: Gerenciamento de Conteúdo (CRUD de Livros)

* Implementação das interfaces e lógica para listar, adicionar, editar e remover livros.
* Desenvolvimento de formulários dedicados para as operações de criação e edição.
* Integração completa com a API do JSON Server para persistência dos dados dos livros.

### Fase 4: Gerenciamento de Usuários (CRUD de Usuários)

* Criação das interfaces e lógica para listar, adicionar, editar e remover usuários.
* Integração com a API do JSON Server para as operações de usuário.

### Fase Final: Polimento e Implantação

* Garantir a responsividade e o refinamento visual em todos os dispositivos.
* Revisão de código e otimização de performance.
* Testes abrangentes de todas as funcionalidades.
* Preparação para a demonstração e possível implantação (ex: Vercel, Netlify).

## Como Rodar o Projeto Localmente

Para configurar e executar o projeto em sua máquina:

### Pré-requisitos

Certifique-se de ter o [Node.js](https://nodejs.org/en/) (versão LTS recomendada) e o [npm](https://www.npmjs.com/get-npm) (gerenciador de pacotes do Node.js) instalados.

### Instalação

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/Xandetds/Projeto-Front-end.git](https://github.com/Xandetds/Projeto-Front-end.git)
    ```

2.  Navegue até o diretório do projeto:
    ```bash
    cd Projeto-Front-end
    ```

3.  Instale as dependências:
    ```bash
    npm install
    ```

### Executando o Backend Simulado (JSON Server)

Em um **novo terminal** na raiz do projeto (`Projeto-Front-end`):

1.  Crie o arquivo `db.json` com os dados iniciais de livros e usuários. Exemplo:
    ```json
    {
      "livros": [
        {
          "id": 1,
          "titulo": "O Senhor dos Anéis",
          "autor": "J.R.R. Tolkien",
          "genero": "Fantasia",
          "sinopse": "Uma aventura épica...",
          "urlCapa": "[https://example.com/capa_sda.jpg](https://example.com/capa_sda.jpg)",
          "conteudoTextoInicial": "Primeiro parágrafo do livro..."
        }
      ],
      "usuarios": [
        {
          "id": 1,
          "nome": "Admin",
          "email": "admin@livros.com",
          "senha": "123",
          "tipoUsuario": "admin"
        }
      ]
    }
    ```
2.  Instale o JSON Server (se ainda não o fez):
    ```bash
    npm install json-server
    ```
3.  Inicie o servidor:
    ```bash
    npx json-server --watch db.json --port 3001
    ```
    O servidor da API estará disponível em `http://localhost:3001`. Mantenha este terminal ativo.

### Executando a Aplicação Front-end (React)

Em **outro terminal** (mantendo o JSON Server rodando) na raiz do projeto (`Projeto-Front-end`):

```bash
npm run dev
```
A aplicação React será iniciada em `http://localhost:5173`. Mantenha este terminal ativo.

##Status do Projeto
Em desenvolvimento. As funcionalidades estão sendo implementadas incrementalmente.

Autores
Alexandre Tibes da Silva
