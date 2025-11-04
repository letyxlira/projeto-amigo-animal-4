# 🐾 Projeto ONG - Amigo Animal (Entrega IV)

<p align="center">
  <img src="https://img.shields.io/badge/status-concluído-green" alt="Status do Projeto: Concluído">
  <img src="https://img.shields.io/badge/licença-MIT-blue" alt="Licença MIT">
</p>

> Este é um projeto acadêmico completo que demonstra a evolução de um site HTML estático para uma aplicação web dinâmica, acessível e otimizada, seguindo práticas profissionais de desenvolvimento front-end, incluindo GitFlow, Acessibilidade (WCAG) e Otimização para produção.

<br>

---

## ✨ Funcionalidades e Conceitos Aplicados

Este projeto cumpre um fluxo de trabalho profissional completo, documentado através de Issues, Milestones e Pull Requests.

### JavaScript 
* **Sistema de SPA Básico:** Navegação que carrega o conteúdo das páginas (`index.html`, `projetos.html`, `cadastro.html`) via `fetch` sem recarregar o site.
* **Templates Dinâmicos:** Os cards da página "Projetos" são gerados 100% via JavaScript a partir de um *array* de dados, permitindo fácil adição de novos projetos.
* **Validação de Formulário:** Verificação de consistência de dados (`checkValidity()`) que impede o envio de formulários inválidos e avisa o usuário.

### Acessibilidade e Otimização 
* **Acessibilidade (WCAG):**
    * O menu hambúrguer foi refatorado de um "checkbox hack" para um `<button>` semântico com atributos **ARIA** (`aria-expanded`, `aria-controls`) para ser 100% acessível por leitores de tela.
    * O formulário utiliza `aria-invalid` para comunicar erros de validação a tecnologias assistivas.
    * Todos os links de navegação possuem estados `:focus` visíveis para navegação por teclado.
* **Modo Escuro (Dark Mode):**
    * Um botão de "toggle" (Sol/Lua) permite ao usuário alternar o tema.
    * A preferência é salva no `localStorage` e persiste entre as sessões.
    * Detecta automaticamente a preferência do sistema operacional (`prefers-color-scheme`).
    * Corrige o "pisque" (FOUC) com um script bloqueador no `<head>`.
* **Otimização para Produção:**
    * Todos os arquivos CSS e JS foram **minificados** (`.min.css`, `.min.js`).
    * As imagens do projeto foram **comprimidas**.
    * O HTML foi atualizado para carregar apenas os arquivos otimizados.

### CSS 
* **Design System:** Um sistema de design consistente foi criado com Variáveis CSS (`:root`).
* **Layouts Modernos:** A estrutura principal usa CSS Grid (`grid-template-areas`) e componentes internos usam Flexbox.
* **Grid de 12 Colunas:** Foi implementado um sistema de grid customizado (`.row` e `.col-X`).

<br>

## 🛠️ Tecnologias Utilizadas

* **HTML5** (Semântico e com atributos ARIA)
* **CSS3** (Variáveis, Grid, Flexbox, Media Queries)
* **JavaScript (ES6+)** (DOM, Eventos, Fetch API, localStorage)
* **Git & GitHub** (GitFlow, Issues, Pull Requests)

<br>

## 🚀 Como Rodar o Projeto

Siga os passos abaixo para conseguir rodar o projeto localmente.

### Pré-requisitos
* Um navegador web moderno (Chrome, Firefox, Opera).
* **Um servidor local (Obrigatório).**

### Instalação e Execução

Este projeto **não funciona** apenas abrindo o `index.html` (protocolo `file://`). Como ele usa a `fetch()` API para o roteamento SPA, ele precisa ser servido por um servidor web (protocolo `http://`) devido à política de segurança (CORS) dos navegadores.

1.  Clone este repositório:
    ```bash
    git clone https://github.com/letyxlira/projeto-amigo-animal-4.git
    ```
    *(**Obs:** Use a URL do seu repositório da Entrega IV)*

2.  Acesse a pasta do projeto:
    ```bash
    cd projeto-amigo-animal-4
    ```

3.  Inicie um servidor local. A forma mais fácil é:
    * **Opção 1 (VS Code):** Instale a extensão "Live Server" e clique em "Go Live" no canto inferior direito.
    * **Opção 2 (Python):** Se você tem Python instalado, rode `python -m http.server` na pasta e acesse `http://localhost:8000` no seu navegador.

<br>

## 👨‍💻 Autor

Desenvolvido por **Letycia L. Barbosa**.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/letycia-lira-barbosa)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/letyxlira)
