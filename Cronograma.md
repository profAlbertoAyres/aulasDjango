# Cronograma Semestral – Programação Web (Django)
**Curso:** Técnico em Informática Integrado ao Ensino Médio (3º Ano)  
**Carga horária:** 80 horas (40 aulas de 2h)  
**Professor(a):** [Seu Nome]

---

## 1. Visão Geral do Semestre

**Objetivo Geral:** Capacitar o aluno a desenvolver uma aplicação web full‑stack funcional utilizando Django, aplicando arquitetura MVT, sistema de templates, ORM e CRUD. No 4º bimestre, os alunos aplicarão esses conhecimentos no desenvolvimento de um **projeto integrador em grupo** com tema diverso.

**Competências:**
- Compreender a arquitetura e o fluxo de um framework web.
- Desenvolver o backend com Django.
- Modelar dados e relacionamentos (Models).
- Integrar frontend (HTML5, CSS3, Bootstrap) ao backend.
- Versionar código com Git e GitHub.
- Trabalhar em equipe aplicando metodologias ágeis simplificadas.

**Habilidades:**
- Criar projetos e apps Django.
- Mapear URLs e criar views.
- Construir templates com herança, tags e arquivos estáticos.
- Definir models e relacionamentos (ForeignKey).
- Utilizar o Django Admin e o ORM básico.
- Implementar CRUD completo.
- Versionar e colaborar via GitHub.

---

## 2. Cronograma do 3º Bimestre (Teoria e Fundamentos)

| Aula | Data | Tipo | CH | Conteúdo | Objetivos | Atividade Prática (Laboratório) |
|:---:|:---:|:---:|:---:|---|----|---|
| **0** | 25/07 (Sáb) | Med. Tec. | 2h | **Aula Inaugural** – Vídeos acessíveis: O que é framework? Apresentação do Django. Acessibilidade na web. | Conhecer o conceito de framework e o Django. Sensibilizar para a web acessível. | Questionário online sobre os vídeos (legendados e com intérprete de Libras). |
| **1** | 27/07 (Seg) | Presencial | 2h | **Ambiente e “Olá, Mundo!”** – venv, instalação do Django, criação do primeiro projeto. | Configurar o ambiente e rodar o servidor de desenvolvimento. | Setup guiado: todos criam o projeto `meu_site` e executam o servidor. |
| **2** | 28/07 (Ter) | Presencial | 2h | **Projeto vs Aplicação** – Estrutura de projeto, conceito de app, `manage.py startapp`, `views.py`, `HttpResponse`. | Diferenciar projeto e app; criar e registrar uma app; criar a primeira view. | Criar app `paginas` com view `home` retornando “Bem‑vindo!”. Projeto `controle_treinos` é criado para exemplos. |
| **3** | 03/08 (Seg) | Presencial | 2h | **URLs e Views** – `urls.py`, `path()`, mapeamento URL→View, parâmetros na URL. | Compreender roteamento; criar views com parâmetros. | View `saudacao` que recebe um nome pela URL e retorna um título HTML. |
| **4** | 04/08 (Ter) | Presencial | 2h | **Introdução aos Templates** – Separando lógica e apresentação, `render()`, contexto `{{ variavel }}`. | Renderizar templates e passar dados da view para o HTML. | View `dados_aluno` que exibe informações em tabela HTML usando template. |
| **5** | 10/08 (Seg) | Presencial | 2h | **Template Tags** – `{% if %}`, `{% for %}`, contexto com listas. | Criar templates dinâmicos com condicionais e loops. | Lista de exercícios exibida com `{% for %}` e mensagem condicional. |
| **6** | 11/08 (Ter) | Presencial | 2h | **Herança de Templates** – `{% block %}`, `{% extends %}`, estrutura base. | Reutilizar código HTML; criar layout padrão. | Construir `base.html` com blocos e página `sobre.html` que estende. |
| **7** | 17/08 (Seg) | Presencial | 2h | **Arquivos Estáticos** – `STATIC_URL`, `{% static %}`, CSS customizado. | Servir arquivos estáticos e estilizar páginas. | Criar `styles.css` e vinculá‑lo; exibir imagem estática. |
| **8** | 18/08 (Ter) | Presencial | 2h | **Bootstrap no Django** – Navbar, Grid, tabelas, botões, atributos de acessibilidade. | Criar interfaces profissionais e acessíveis rapidamente. | Converter página de alunos em layout com card e tabela Bootstrap. |
| **9** | 24/08 (Seg) | Presencial | 2h | **Revisão e Fixação** | Consolidar fluxo URL→View→Template; sanar dúvidas. | Exercício integrado: página “Lista de Tarefas” completa. |
| **10**| 25/08 (Ter) | Presencial | 2h | **Git e GitHub com Django** – `.gitignore`, `init`, `commit`, `push`. | Versionar o projeto corretamente. | Criação do `.gitignore` padrão Django; primeiro commit e push do projeto base. |
| **–** | **01/08 (Sáb)** | Sáb. Letivo | 2h | **AMT‑1** – “Configurando meu Ambiente” | Tutorial em PDF/vídeo mostrando setup até o “Hello, World!”. | Entrega via Google Sala de Aula. |
| **11** | 31/08 (Seg) | Presencial | 2h | **Models: a planta da casa** – Models, ORM, tipos de campos, criação do model `Aluno`. | Entender models e criar o primeiro. | Criar model `Aluno` com `nome`, `email`, `data_nascimento`. |
| **12** | 01/09 (Ter) | Presencial | 2h | **Migrations e Django Admin** – `makemigrations`, `migrate`, registro no admin, superusuário. | Sincronizar banco e usar o Admin. | Executar migrations; registrar `Aluno`; cadastrar 3 alunos via Admin. |
| **13** | 08/09 (Ter) | Presencial | 2h | **ORM Básico e ForeignKey** – Shell do Django, CRUD via ORM, relacionamento 1:N. | Manipular dados sem SQL; implementar chave estrangeira. | Criar model `Exercicio` com FK para `Aluno`; testar via Shell. |
| **–** | **12/09 (Sáb)** | Sáb. Letivo | 2h | **1ª AVALIAÇÃO** (prática assíncrona) | Avaliar setup, URLs, views, templates, herança, Bootstrap. | App `biblioteca`: listar livros em tabela Bootstrap herdando de `base.html`. |
| **14** | 14/09 (Seg) | Presencial | 2h | **Listando dados do banco nos templates** – `Model.objects.all()`, QuerySet no contexto, iteração com `{% for %}`. | Unir View, Template e Model; listar dados reais. | View `lista_alunos` que exibe alunos em tabela Bootstrap. |
| **15** | 15/09 (Ter) | Presencial | 2h | **Introdução ao CRUD** – As quatro operações; fluxo completo; planejamento de rotas. | Compreender CRUD e planejar URLs. | Mapa de URLs para CRUD de `Exercicio` desenhado no quadro. |
| **16**| 21/09 (Seg) | Presencial | 2h | **CRUD: Create** – Formulário HTML com POST, CSRF, `request.POST`, `create()`, `redirect`. | Criar interface e lógica para inserir registros. | Template `form_exercicio.html` e view `criar_exercicio` (GET/POST). |
| **17**| 22/09 (Ter) | Presencial | 2h | **CRUD: Read (Detalhes) e Update** – `get_object_or_404`, edição com `instance`. | Exibir detalhes e editar registros. | View/template `detalhes_exercicio` e view de edição reutilizando formulário. |
| **18**| 28/09 (Seg) | Presencial | 2h | **CRUD: Delete** – View de confirmação, template com POST, `Model.delete()`. | Implementar exclusão segura. | View `deletar_exercicio` com página de confirmação. |
| **–** | **19/09 (Sáb)** | Sáb. Letivo | 2h | **AMT‑2** – “CRUD de Alunos” | Implementar CRUD completo para `Aluno` (réplica do de Exercicio). | Entrega via GitHub. |
| **19**| 29/09 (Ter) | Presencial | 2h | **Plantão de dúvidas e refatoração** | Sanar dúvidas; consolidar CRUD. | Refatoração coletiva dos pontos de maior dificuldade. |
| **20**| 05/10 (Seg) | Presencial | 2h | **2ª AVALIAÇÃO PRESENCIAL** | Models, Migrations, Admin e CRUD. | Criar model `Categoria` e implementar seu CRUD completo. |
| **21**| 06/10 (Ter) | Presencial | 2h | **Devolutiva da avaliação** | Corrigir prova; feedback do bimestre. | Resolução comentada da avaliação. |

**Feriado/Recesso:** 13/10  
**Semana Nacional de Ciência e Tecnologia:** 19 e 20/10 (aulas temáticas – sem conteúdo da disciplina)

---

## 3. Avaliações do 3º Bimestre (Valor: 10,0)

- **Avaliação 1 (12/09, assíncrona) – 3,0 pts**  
  *Objetivo:* Avaliar setup, URLs, views, templates com herança e Bootstrap.  
  *Descrição:* Criar app `biblioteca`; view que exiba lista de livros em tabela Bootstrap, herdando de `base.html`.  
  *Critérios:* Criação/registro da app (0,5); URL correta (0,5); view com contexto (1,0); template com herança e `{% for %}` (1,0).  
  *Entrega:* link do repositório GitHub.

- **Avaliação 2 (05/10, presencial) – 3,5 pts**  
  *Objetivo:* Models, migrações, Admin e CRUD.  
  *Descrição:* Criar model `Categoria` (campo `nome`) e implementar CRUD completo com templates herdados e Bootstrap.  
  *Critérios:* Model/migrações (0,5); listagem (1,0); criação (1,0); detalhes/edição (0,5); exclusão (0,5).  
  *Entrega:* código funcionando no laboratório.

- **AMTs (total 3,5 pts):**
  - **AMT‑0 (25/07)** – Questionário sobre vídeos da aula inaugural (1,0 pt bônus).
  - **AMT‑1 (01/08)** – Tutorial “Configurando meu Ambiente” (1,5 pts).
  - **AMT‑2 (19/09)** – “CRUD de Alunos” completo (2,0 pts).

---

## 4. Cronograma do 4º Bimestre (Projeto Integrador em Grupo)

**Foco:** Os alunos, organizados em grupos, desenvolverão uma aplicação web completa com tema diverso. O professor orienta cada etapa, garantindo a aplicação dos conteúdos vistos no 3º bimestre.

| Aula | Data | Tipo | CH | Conteúdo / Atividade | Objetivos | Entregáveis / Evolução do Projeto |
|:---:|:---:|:---:|:---:|---|---|:---|
| **–** | **31/10 (Sáb)** | Sáb. Letivo | 2h | **AMT‑3 – “Pré‑projeto”** | Definir tema, escopo e entidades do projeto. | Documento com tema, descrição breve e lista de entidades/modelos previstos. |
| **22**| 26/10 (Seg) | Presencial | 2h | **Formação das equipes e kick‑off** – Escolha de temas, definição de escopo, criação do repositório no GitHub. | Organizar grupos, definir regras de colaboração e iniciar o versionamento. | Repositório do grupo criado; `README.md` inicial com tema e integrantes. |
| **23**| 27/10 (Ter) | Presencial | 2h | **Modelagem de dados** – Der para cada projeto, models e relacionamentos. | Traduzir o escopo em models Django (com ForeignKey). | Models definidos e migrações iniciais executadas. |
| **24**| 03/11 (Ter) | Presencial | 2h | **Admin e população de dados** – Registro dos models no Admin, criação de superusuário, inserção de dados de teste. | Familiarizar‑se com os dados via Admin. | Admin configurado; dados de teste inseridos. |
| **25**| 14/11 (Sáb) | Presencial | 2h | **CRUD – parte 1** – Implementação das operações de **listagem** e **criação** para a entidade principal do projeto. | Aplicar CRUD no contexto do tema do grupo. | Listagem e formulário de criação funcionais. |
| **–** | **07/11 (Sáb)** | Sáb. Letivo | 2h | **AMT‑4 – “Checkpoint de progresso”** | Relatar o andamento do projeto. | Relatório simples (PDF) com capturas de tela comentadas mostrando o CRUD parcial. |
| **–** | **09 e 10/11** | JICAS | – | *Semana temática – sem conteúdo regular* | – | – |
| **26**| 16/11 (Seg) | Presencial | 2h | **CRUD – parte 2** – Detalhes, edição e exclusão. | Completar o CRUD da entidade principal. | CRUD completo para a entidade principal. |
| **27**| 17/11 (Ter) | Presencial | 2h | **Funcionalidades extras** – Filtros, dashboard simples, página inicial com contagens. | Enriquecer a aplicação com recursos de navegação e visualização. | Página inicial com cards de resumo; filtro por relacionamento (ex: listar itens por categoria). |
| **28**| 23/11 (Seg) | Presencial | 2h | **1ª AVALIAÇÃO DO 4º BIMESTRE** (individual prática) | Avaliar capacidade de implementar funcionalidade em contexto novo. | Avaliação prática em laboratório (ver descrição abaixo). |
| **29**| 24/11 (Ter) | Presencial | 2h | **Refinamento e acessibilidade** – Revisão de templates, Bootstrap, contraste, atributos `aria`, legendas. | Polir a interface e garantir requisitos mínimos de acessibilidade. | Sistema com design consistente e elementos acessíveis. |
| **30**| (a definir) | Síncrono remoto | 2h | **Preparação para apresentação final** – Orientações sobre o vídeo de demonstração. | Alinhar expectativas para a entrega final. | Roteiro do vídeo e últimos ajustes. |
| **–** | (a definir) | – | – | **AVALIAÇÃO FINAL (AMT‑5)** – Vídeo de demonstração do projeto | Apresentar o sistema finalizado. | Vídeo (3‑5 min) com legendas mostrando funcionalidades e trecho de código. |

---

## 5. Avaliações do 4º Bimestre (Valor: 10,0)

- **Avaliação 1 (23/11, presencial) – 3,5 pts**  
  *Objetivo:* Aferir a capacidade individual de implementar CRUD com relacionamento em situação nova.  
  *Descrição:* Cada aluno receberá a especificação de um mini‑projeto (ex.: “Gerenciador de Playlists”) e deverá criar models, migrações e CRUD completo para duas entidades relacionadas.  
  *Critérios:* Models e relacionamentos (1,0); CRUD funcional (2,0); templates com herança e Bootstrap (0,5).  
  *Entrega:* código funcionando no laboratório.

- **Avaliação 2 (AMT‑5) – 3,5 pts**  
  *Objetivo:* Demonstrar o projeto integrador finalizado, praticar comunicação e documentação.  
  *Descrição:* Vídeo de 3‑5 min apresentando o sistema do grupo: funcionalidades, decisões de design e um trecho de código relevante. O vídeo deve conter legendas (revisadas, não apenas automáticas).  
  *Critérios:* Demonstração completa das funcionalidades (2,0); clareza e organização (1,0); análise do código (0,5).  
  *Entrega:* link do vídeo (YouTube não listado, Google Drive) + link do repositório GitHub do grupo.

- **AMTs (total 3,0 pts):**
  - **AMT‑3 (31/10)** – Documento de pré‑projeto (tema, escopo, entidades) – 1,5 pts.
  - **AMT‑4 (07/11)** – Relatório de progresso com capturas de tela comentadas – 1,5 pts.

---

## 6. Diretrizes de Acessibilidade

Para garantir a plena participação da aluna com deficiência auditiva:
- **Materiais:** Vídeos com janela de Libras ou legendas revisadas; slides visuais e textos objetivos.
- **Sala de aula:** Professor fala de frente para a turma; instruções verbais sempre acompanhadas de registro escrito.
- **Atividades:** Entregas que envolvem vídeo (AMT‑5) devem incluir legendas, promovendo um ambiente inclusivo.
- **Avaliações:** Enunciados com frases curtas e vocabulário técnico previamente definido; tempo adicional se necessário.
- **Referências:** Glossário bilíngue de termos técnicos construído com a turma.

---

## 7. Metodologias Ativas

- **Aprendizagem Baseada em Projetos (ABP):** todo o semestre converge para o projeto integrador.
- **Sala de Aula Invertida:** AMTs preparam o terreno para as aulas presenciais práticas.
- **Prática Guiada e Demonstração:** professor programa junto nas primeiras aulas de cada tópico.
- **Refatoração Coletiva:** correção de erros comuns com participação da turma.
- **Trabalho em Equipe:** 4º bimestre inteiramente colaborativo, com repositórios e responsabilidades compartilhadas.

---

## 8. Recursos Didáticos

- Laboratório de informática com Python 3.10+, Git, VS Code.
- Projetor multimídia para demonstrações.
- Quadro branco para diagramas e mapas de URL.
- GitHub (versionamento e entrega).
- Google Sala de Aula (central de materiais e entregas).

---

## 9. Bibliografia Básica

1. **Documentação Oficial do Django** – [https://docs.djangoproject.com/](https://docs.djangoproject.com/)  
2. **Tutorial Django Girls (PT‑BR)** – [https://tutorial.djangogirls.org/pt/](https://tutorial.djangogirls.org/pt/)  
3. **MDN Web Docs – Tutorial Django** – [https://developer.mozilla.org/pt-BR/docs/Learn/Server-side/Django](https://developer.mozilla.org/pt-BR/docs/Learn/Server-side/Django)  
4. **Cartilha de Acessibilidade na Web (W3C Brasil)** – [https://www.w3c.br/pub/Materiais/PublicacoesW3C/cartilha-w3cbr-acessibilidade-web-fasciculo-I.html](https://www.w3c.br/pub/Materiais/PublicacoesW3C/cartilha-w3cbr-acessibilidade-web-fasciculo-I.html)

---
**Observação:** Este cronograma é um guia vivo. Ajustes podem ser feitos conforme o ritmo da turma, respeitando sempre os objetivos de aprendizagem e a inclusão de todos.