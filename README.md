# Olá, eu sou o Willians 👋

<p>
  <img src="https://komarev.com/ghpvc/?username=Willsmt&label=Visitas%20no%20perfil&color=764ABC&style=flat" alt="Visitas no perfil" />
  <img src="https://img.shields.io/badge/Dispon%C3%ADvel%20para%20vagas-Full%20Stack%20Python%20%26%20React-2ea44f?style=flat" alt="Disponível para vagas" />
</p>

### Desenvolvedor Full Stack Python & React

Construo interfaces responsivas e componentizadas com foco em código limpo, escalável e bem estruturado. Atualmente expandindo a stack rumo ao desenvolvimento Full Stack com Python.

---

### 🚀 Projetos em destaque

#### 💈 [trimote](https://github.com/Willsmt/trimote) — Sistema de agendamento full stack (projeto pessoal)
Sistema completo de agendamento online para barbearia: o cliente escolhe serviço, dia e horário livre e agenda sozinho, com a garantia de que nunca há duplo agendamento no mesmo horário.

`Next.js 16` · `TypeScript` · `Prisma` · `PostgreSQL` · `NextAuth` · `Tailwind CSS` · `Vitest`

- Não-sobreposição garantida no **nível de dados** (PostgreSQL *exclusion constraint* com `EXCLUDE USING gist`)
- Fuso horário correto: instantes em **UTC**, lógica em `America/Sao_Paulo` isolada numa camada de domínio
- Autorização **multi-tenant no servidor** (`requireOwner` / `requireAdmin`) com camadas anti-escalação de privilégio
- Núcleo testável separado das **Server Actions**, com testes de **unidade e integração** (Vitest)
- Razão financeira (receitas/despesas) com `Decimal`, *soft delete* e snapshots de preço

🔗 **Acesse:** trimote.com.br

#### 💅 [belle-et-belle](https://github.com/Willsmt/belle-et-belle) — Landing page para estúdio de estética (projeto freelance)
Projeto freelance completo para o estúdio de estética Belle et Belle: estratégia digital, identidade visual e landing page reunidos em um só lugar.

`HTML5` · `CSS3` · `JavaScript`

- Logo oficial inline (nav e rodapé) via `<symbol>`/`<use>`, sem depender de arquivo externo
- Baralho de fotos do studio no hero, com slider antes/depois arrastável (mouse, touch e teclado)
- Galeria de resultados por categoria com lightbox e carrossel de depoimentos
- Apostila de estratégia digital e identidade visual entregues junto com o site
- SEO com meta tags, Open Graph e JSON-LD (BeautySalon)

#### 🎵 [reverb](https://github.com/Willsmt/gerador-playlist-reverb) — Microsite musical para marca de sucos (projeto freelance)
Microsite full stack onde cada ritmo musical tem um QR code fixo e gera uma playlist aleatória com links para as principais plataformas de streaming.

`Next.js 16` · `TypeScript` · `Prisma` · `PostgreSQL` · `NextAuth` · `Tailwind CSS` · `Vitest`

- Sorteio de playlist com Fisher-Yates, mantendo a lógica testável sem banco
- Painel admin com login Google (NextAuth) e autorização por allowlist de e-mails
- Soft delete nos ritmos e músicas, preservando QR codes já impressos
- Rate limiting por IP com janela deslizante em memória
- Segurança de rotas: slug validado por Zod, headers CSP e erros sem stack trace exposto

#### 🎤 [pier7](https://github.com/Willsmt/evento_gravacao_pier7) — Convite para evento de gravação ao vivo (projeto freelance)
Landing page de convite para a gravação ao vivo da Pier7 Music, com confirmação de presença e integração completa via WhatsApp e Google.

`HTML` · `CSS` · `JavaScript`

- Confirmação de presença com formulário validado, salvo automaticamente no Google Sheets
- Geração de mensagem de convite pronta para compartilhar no WhatsApp
- Botão de adicionar evento direto no Google Calendar
- Prévia de compartilhamento com Open Graph e imagem de capa personalizada

#### 🎮 [EPlay](https://github.com/Willsmt/eplay-loja-react) — E-commerce de games
E-commerce de jogos com catálogo, categorias, carrinho e checkout completo, consumindo uma API real com cache.

`React` · `TypeScript` · `Redux Toolkit` · `RTK Query` · `Styled Components` · `React Router` · `Formik` · `Yup` · `Vite`

- Catálogo e categorias consumidos via **RTK Query** (com cache e estados de loading/erro)
- Carrinho lateral gerenciado por **Redux Toolkit**
- Checkout com **formulários validados** (Formik + Yup), **máscaras** de CPF/cartão e parcelamento dinâmico
- Deploy contínuo na **Vercel**

🔗 **Acesse:** https://eplay-loja-react.vercel.app

#### 🐍 [commit-diario](https://github.com/Willsmt/commit-diario) — Blog pessoal com Django
Blog pessoal desenvolvido com Django, com apps organizados em models, views e urls, migrations e testes automatizados.

- Estrutura de app Django com **models, views e urls** separados
- **Testes automatizados** (pytest) com factories para models e views
- Variáveis sensíveis via **.env**, nunca versionadas
- Painel administrativo via Django Admin

#### 🗄️ [estudos-sql-postgresql](https://github.com/Willsmt/estudos-sql-postgresql) — Modelagem relacional com PostgreSQL
Estudos de SQL e modelagem de dados com PostgreSQL, incluindo dois schemas completos (blog e e-commerce) com diagramas ER.

`PostgreSQL` · `SQL` · `Modelagem de Dados`

- Schemas completos com diagramas **ER** (blog e e-commerce)
- Decisões de modelagem documentadas (**CASCADE vs RESTRICT**, soft delete, histórico de preços)
- Convenções de nomenclatura para PKs, FKs, índices e constraints
- Acesso ao banco via **SSH tunnel**, seguindo o princípio do menor privilégio

#### ⚙️ [flask-gunicorn-nginx-deploy](https://github.com/Willsmt/flask-gunicorn-nginx-deploy) — Deploy de app Flask em produção
Stack de deploy de uma aplicação Flask em Linux, do ambiente virtual ao serviço gerenciado por systemd com Nginx como reverse proxy.

`Python` · `Flask` · `Gunicorn` · `Nginx` · `systemd`

- **Gunicorn** como servidor WSGI multi-worker
- **Nginx** como reverse proxy via Unix socket (sem expor o Gunicorn na rede)
- Serviço gerenciado por **systemd**
- Documentação detalhada de arquitetura e decisões de segurança

#### 🔀 [estudos-python-avancado](https://github.com/Willsmt/estudos-python-avancado) — Concorrência, TDD e algoritmos
Estudos de programação assíncrona e concorrência, com projeto prático de web scraping assíncrono.

`Python` · `asyncio` · `aiohttp` · `pytest`

- Scraper assíncrono com **asyncio + aiohttp** e controle de concorrência via **Semaphore**
- Estudo de **threads, multiprocessing e TDD**
- Apostila própria em PDF documentando o aprendizado

---

### 🛠️ Tecnologias & Ferramentas

**💻 Linguagens**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**⚛️ Frameworks & Bibliotecas**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vue.js](https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D)
![Redux](https://img.shields.io/badge/Redux_Toolkit-764ABC?style=for-the-badge&logo=redux&logoColor=white)
![Styled Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

**⚙️ Ferramentas & Automação**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Less](https://img.shields.io/badge/Less-1D365D?style=for-the-badge&logo=less&logoColor=white)
![Gulp](https://img.shields.io/badge/Gulp-CF4647?style=for-the-badge&logo=gulp&logoColor=white)
![Grunt](https://img.shields.io/badge/Grunt-FBA919?style=for-the-badge&logo=grunt&logoColor=white)

**🐍 Back-End & Dados**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge&logo=gunicorn&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

**🧪 Testes**

![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![Testing Library](https://img.shields.io/badge/Testing%20Library-E33332?style=for-the-badge&logo=testing-library&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-69D3A7?style=for-the-badge&logo=cypress&logoColor=white)

---

### 🧠 Conceitos & Metodologias

`Desenvolvimento Front-End` · `Design Responsivo` · `Integração de APIs (AJAX / Fetch)` · `Programação Orientada a Objetos (POO)` · `Atomic Design` · `Arquitetura CSS (BEM e SMACSS)` · `Criação de Landing Pages` · Desenvolvimento Back-End · APIs REST · ORM e Migrations · Modelagem Relacional (SQL) · TDD · Programação Assíncrona · Deploy (Gunicorn / Nginx / systemd)

---

### 💡 Competências em detalhe

- **React + TypeScript** com gerenciamento de estado (props, eventos, estado local/global)
- **Redux Toolkit** e **RTK Query** para fluxo de dados e performance
- **CSS-in-JS** com Styled Components, seguindo **Atomic Design**
- JavaScript moderno **(ES6+)**: arrow functions, spread/rest, map/set, async
- **POO** em JavaScript: herança, encapsulamento, código modular
- Consumo de APIs com **AJAX / Fetch** e tratamento de exceções
- **CSS responsivo**: Flexbox, Grid, breakpoints e viewport
- Pré-processadores **(Sass / Less)** e automação de tarefas com **Gulp / Grunt**
- Organização de CSS com **BEM** e **SMACSS**
- **Testes** com **React Testing Library** (unitários) e **Cypress** (E2E)
- Versionamento com **Git** (branches, merge, resolução de conflitos e **pull requests**) e **GitHub**
- **Python** com **Django** (models, views, urls, migrations) e **Flask**
- **Testes automatizados** com **pytest** e TDD
- **Modelagem de dados** relacional com **PostgreSQL** (schemas, relacionamentos, índices e constraints)
- **Deploy** em Linux com **Gunicorn**, **Nginx** (reverse proxy) e **systemd**
- **Programação assíncrona** com **asyncio / aiohttp** e controle de concorrência
---

### 🚧 Em estudo

APIs REST com **Django REST Framework** · Autenticação **JWT** · **Docker** · Integração dos schemas **PostgreSQL** ao **Django ORM**
---

### 📊 Estatísticas

![Stats](https://github-readme-wills.vercel.app/api?username=Willsmt&show_icons=true&theme=tokyonight)
![Top Langs](https://github-readme-wills.vercel.app/api/top-langs/?username=Willsmt&layout=compact&theme=tokyonight)

---

### 📫 Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/willians-martins-329350329/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:willmarthins@gmail.com)
