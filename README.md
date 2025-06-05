# Plataforma de Streaming de Livros Digitais

Este repositório contém o código-fonte de um projeto de front-end desenvolvido em **React.js** para uma avaliação. O objetivo é simular uma plataforma de streaming de livros digitais, onde usuários podem explorar e "ler" livros, e administradores podem gerenciar o catálogo de livros e os usuários do sistema.

## Requisitos Atendidos (Avaliação Front-end)

Este projeto foi desenvolvido para cumprir os seguintes requisitos:

1.  **Aplicação em React.js:** Construída do zero utilizando o framework React.
2.  **Layout Agradável e Responsivo:** A interface se adapta a diferentes tamanhos de tela (desktop, tablet, mobile).
3.  **JSON Server para Persistência de Dados:** Utiliza o JSON Server para simular uma API RESTful para o armazenamento de dados de livros e usuários.
4.  **Requisições HTTP:** Todas as interações com o "backend" (JSON Server) são feitas via requisições HTTP (GET, POST, PUT, DELETE).
5.  **Tratamento de Exceções:** Implementação de `try/catch` para lidar com erros nas requisições HTTP.
6.  **Tela de Login:** Possui uma tela de login com validação e exibição de mensagens de erro.
7.  **CRUD de Livros (Serviços):** Funcionalidades completas de Criar, Ler, Atualizar e Deletar livros, com múltiplos campos.
8.  **CRUD de Usuários:** Funcionalidades completas de Criar, Ler, Atualizar e Deletar usuários do sistema.
9.  **Navbar e Footer Fixos:** Componentes de navegação e rodapé presentes em todas as telas, exceto a de login.
10. **Navegação SPA:** Uso de `react-router-dom` para navegação entre as diferentes rotas da aplicação.

## Tecnologias Utilizadas

* **React.js:** Biblioteca JavaScript para construção de interfaces de usuário.
* **JSON Server:** Ferramenta para criar APIs REST simuladas rapidamente.
* **HTML5 & CSS3:** Para a estruturação e estilização da interface.
* **JavaScript (ES6+):** Linguagem de programação principal.
* **Git & GitHub:** Para controle de versão e hospedagem do código.
* **(Opcional: Adicione aqui se usar) Frameworks CSS:** Ex: Tailwind CSS, Bootstrap, Material-UI, etc.
* **(Opcional: Adicione aqui se usar) Bibliotecas de Requisição:** Ex: Axios (além do Fetch API nativo).

## Como Rodar o Projeto (Para Desenvolvedores)

### Pré-requisitos

Certifique-se de ter o [Node.js](https://nodejs.org/en/) e o [npm](https://www.npmjs.com/get-npm) (ou Yarn) instalados em sua máquina.

### Instalação

1.  Clone este repositório 
    ```bash
    git clone [https://github.com/Xandetds/Projeto-Front-end.git](https://github.com/Xandetds/Projeto-Front-end.git)
    ```

2.  Navegue até a pasta do projeto 
    ```bash
    cd Projeto-Front-end
    ```

3.  Instale as dependências do projeto React:
    ```bash
    npm install
    ```

### Executando o JSON Server

Para simular o backend e ter acesso aos dados, você precisa rodar o JSON Server em um terminal separado.

1.  Crie um arquivo `db.json` na raiz do projeto com seus dados de livros e usuários. 
2.  No terminal, na raiz do projeto, execute:
    ```bash
    npx json-server --watch db.json --port 3001
    ```
    O servidor estará disponível em `http://localhost:3001`.

### Executando a Aplicação React

Com o JSON Server rodando, abra *outro* terminal na raiz do projeto e execute:

```bash
npm run dev
# ou, se você usou create-react-app:
# npm start
A aplicação React será iniciada em http://localhost:5173 (ou http://localhost:3000).

Estrutura do Projeto
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
Status do Projeto
Em desenvolvimento. As funcionalidades estão sendo implementadas incrementalmente.
