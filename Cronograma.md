## 1. Visão Geral do Semestre

### Objetivos
* **Geral:** Capacitar o estudante a planejar, codificar e implantar uma aplicação web funcional com arquitetura baseada em framework, utilizando o ecossistema Django, persistência de dados em SQLite e interface responsiva.
* **Específicos:** Compreender o fluxo de requisição e resposta na arquitetura MVT; manipular dados relacionais via ORM; criar interfaces dinâmicas usando herança de templates; e gerenciar o código-fonte profissionalmente com Git/GitHub.

### Competências
* Desenvolver aplicações web dinâmicas integrando camadas de lógica, apresentação e persistência.
* Utilizar frameworks estruturados para otimização do processo de desenvolvimento de software.
* Identificar e mitigar erros de sintaxe, lógica e configuração em ambientes de desenvolvimento web.

### Habilidades
* Configurar ambientes virtuais Python e instalar dependências via terminal.
* Mapear tabelas de bancos de dados por meio de classes (*Models*) e gerenciar o ciclo de vida com *Migrations*.
* Codificar visualizações (*Views*) capazes de processar requisições HTTP e realizar operações de CRUD no banco de dados.
* Construir páginas web dinâmicas reutilizando componentes e layouts via *Django Template Language* (DTL).

---

## 2. Cronograma do 3º Bimestre (Foco: Estrutura, MVT e Front-end no Django)

O objetivo deste bimestre é que o estudante domine a estrutura de pastas do Django e consiga criar a interface do sistema integrando o Bootstrap. Ao fim deste período, todas as telas do projeto estarão criadas e navegáveis, usando dados estáticos.

| Aula | C.H. | Conteúdo | Objetivos | Atividade Prática | Evolução do Projeto | Avaliação |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **01** | 2h | Apresentação da Disciplina e Ambiente | Compreender o escopo do semestre e a proposta do Projeto Integrador. | Instalação do Python, VS Code e extensões recomendadas. | Instalação das ferramentas no laboratório. | Diagnóstica |
| **02** | 2h | Conceito de Framework e Virtualenv | Compreender a utilidade de um framework e isolar dependências com `venv`. | Criação e ativação do ambiente virtual via terminal. | Criação da pasta raiz do projeto de treinos. | - |
| **03** | 2h | Criando o Projeto Django | Compreender os comandos de inicialização e a diferença entre Projeto e App. | Execução do `django-admin startproject` e análise do `manage.py`. | Criação da estrutura base do projeto do sistema. | Formativa |
| **04** | 2h | Criando a Primeira Aplicação | Criar a primeira aplicação interna e registrá-la em `settings.py`. | Execução do `startapp core` e registro no projeto principal. | Criação do app `core` (responsável pelo fluxo inicial). | - |
| **05** | 2h | Fluxo de Request/Response: URLs | Compreender como o Django mapeia rotas HTTP para funções. | Configuração do arquivo `urls.py` do projeto e do app. | Criação da rota inicial (`/`) para a página de boas-vindas. | - |
| **06** | 2h | Fluxo de Request/Response: Views | Criar funções que recebem requisições e retornam respostas simples (`HttpResponse`). | Escrita de funções baseadas em funções (FBVs) no arquivo `views.py`. | Exibição de uma mensagem "Bem-vindo ao Sistema de Treinos" via código. | Formativa |
| **07** | 2h | Introdução ao MVT (Templates) | Compreender onde e como armazenar arquivos HTML renderizados pelo Django. | Criação da pasta `templates/` e renderização de HTML usando a função `render()`. | Substituição do texto simples por uma página HTML estruturada de Home. | - |
| **08** | 2h | Git e GitHub no Django | Aplicar controle de versão ignorando arquivos desnecessários (`.gitignore`). | Inicialização do repositório, escrita do `.gitignore` e primeiro `push` para o GitHub. | Publicação do esqueleto inicial do sistema no GitHub de cada aluno. | **Início da AMT 1** |
| **09** | 2h | Integração com Bootstrap | Acoplar bibliotecas CSS externas aos templates gerenciados pelo Django. | Download do Bootstrap e estilização inicial da página home. | Criação de um layout básico visual para a tela inicial do sistema. | - |
| **10** | 2h | Arquivos Estáticos (`staticfiles`) | Configurar e carregar arquivos CSS, imagens e JS customizados. | Configuração de `STATIC_URL` e uso da tag `{% load static %}`. | Inclusão de um arquivo `estilos.css` próprio e logotipo no sistema. | Formativa |
| **11** | 2h | DRY e Herança de Templates | Entender o conceito *Don't Repeat Yourself* e o funcionamento de blocos. | Criação do template base (`base.html`) com `{% block content %}`. | Isolamento do topo (navbar) e do rodapé que serão fixos no sistema. | - |
| **12** | 2h | Construindo as Telas: Aluno | Aplicar a herança de templates para criar novas páginas com esforço reduzido. | Criação da tela de listagem de alunos utilizando tabelas estáticas do Bootstrap. | Extensão do `base.html` para criar a página `/alunos/`. | **Avaliação 1 (Prática)** |
| **13** | 2h | Construindo as Telas: Exercício | Replicar a arquitetura de herança para novas entidades do escopo. | Criação da tela de listagem de exercícios (ex: Supino, Agachamento). | Extensão do `base.html` para criar a página `/exercicios/`. | - |
| **14** | 2h | Construindo as Telas: Treino | Praticar rotas, views e herança in conjunto para fechar o ciclo visual. | Criação da página visual com os cartões (*cards*) dos treinos dos alunos. | Extensão do `base.html` para criar a página `/treinos/`. | - |
| **15** | 2h | Template Tags e Navegação | Utilizar a tag `{% url %}` para interconectar as páginas criadas sem links fixos. | Alteração das tags `href` do menu flutuante utilizando as rotas nomeadas. | Menu de navegação do sistema funcionando de forma integrada. | - |
| **16** | 2h | Consolidação do Layout do Projeto | Revisar a fidelidade visual e a estrutura de diretórios criada até o momento. | Ajustes finos no CSS customizado e tratamento de links quebrados. | Sistema estático de controle de treinos completamente navegável. | **Entrega da AMT 1** |
| **17** | 2h | Revisão Prática Geral | Solucionar dúvidas acumuladas sobre MVT e links dinâmicos. | Exercício rápido de criação de uma rota extra (ex: página "Sobre o sistema"). | Fechamento do ciclo front-end do projeto. | Formativa |
| **18** | 2h | Avaliação Bimestral Prática | Verificar a autonomia do estudante na montagem de um fluxo MVT estático completo. | Desenvolvimento individual em laboratório a partir de um conjunto de requisitos. | Replicação das competências em um cenário similar. | **Avaliação 2 (Prática)** |
| **19** | 2h | Feedback e Ajustes no Repositório | Corrigir problemas nos códigos e atualizar os repositórios para o próximo bimestre. | Correção guiada da avaliação e sincronização dos códigos com o GitHub. | Garantia de que todos os alunos tenham a base pronta para os Models. | Formativa |
| **20** | 2h | Fechamento do Bimestre | Organização das notas e nivelamento técnico para a introdução ao banco de dados. | Organização de arquivos e documentação básica do projeto (Readme). | Repositório limpo e pronto para o 4º bimestre. | Formativa |

---

## 3. Avaliações do 3º Bimestre

### Avaliação 1: Construção da Infraestrutura e Primeira Rota Dinâmica
* **Objetivo:** Avaliar se o aluno consegue criar o ambiente virtual, iniciar um projeto/app Django do zero e criar uma rota renderizando um HTML próprio.
* **Critérios de Avaliação:**
  * Configuração correta do ambiente e registro do app (20%)
  * Configuração sem erros das URLs do projeto e do app (30%)
  * Escrita correta da view baseada em função (20%)
  * Renderização do arquivo HTML aplicando tags estruturais corretas (30%)
* **Forma de Entrega:** Verificação presencial no computador do laboratório e avaliação do código-fonte produzido em tempo real.
* **Valor Sugerido:** 30 Pontos.

### Avaliação 2: Interface Completa do Projeto Integrador com Herança de Templates
* **Objetivo:** Avaliar a capacidade de estruturar o front-end do sistema dentro do Django, fazendo uso de herança de templates e arquivos estáticos (Bootstrap).
* **Critérios de Avaliação:**
  * Criação eficiente do arquivo `base.html` e uso correto das tags `{% block %}` (30%)
  * Integração funcional do Bootstrap e de arquivos CSS locais via `{% load static %}` (20%)
  * Criação das 3 telas estáticas solicitadas: Alunos, Exercícios e Treinos (30%)
  * Menu de navegação funcional utilizando o mapeamento dinâmico de `{% url %}` (20%)
* **Forma de Entrega:** Projeto executável em laboratório + envio do link do repositório GitHub para correção do histórico de commits.
* **Valor Sugerido:** 50 Pontos.

### Atividade Mediada por Tecnologia (AMT 1): Portfólio Digital e Registro de Progresso
* **Objetivo:** Estimular o hábito de versionamento contínuo e documentação, fixando os conceitos da arquitetura de diretórios do Django.
* **Critérios de Avaliação:**
  * Histórico de commits organizado e uso correto do arquivo `.gitignore` (40%)
  * Criação de um arquivo `README.md` simples contendo o nome do projeto, tecnologias utilizadas e capturas de tela (*printscreens*) das telas criadas com pequenas legendas explicativas sobre o fluxo MVT (60%)
* **Forma de Entrega:** Link do repositório público do GitHub postado na plataforma de aprendizagem (AVA) da instituição.
* **Valor Sugerido:** 20 Pontos.

---

## 4. Cronograma do 4º Bimestre (Foco: Models, ORM e CRUD Completo)

Este bimestre introduz a camada de dados. O estudante aprenderá como salvar informações de forma persistente e criar as operações de inclusão, leitura, atualização e exclusão (CRUD) para gerenciar o sistema de treinos de forma dinâmica.

| Aula | C.H. | Conteúdo | Objetivos | Atividade Prática | Evolução do Projeto | Avaliação |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **21** | 2h | Introdução à Camada de Models | Compreender como o Django mapeia classes Python para tabelas SQL via ORM. | Criação do primeiro modelo: classe `Aluno` no arquivo `models.py`. | Definição dos campos Nome, Matrícula e Data de Nascimento do Aluno. | - |
| **22** | 2h | Migrations (Migrações) | Compreender os comandos `makemigrations` e `migrate` e a alteração do banco SQLite. | Geração dos arquivos de migração e execução para criar a tabela física. | Criação real da tabela de alunos no banco de dados local. | Formativa |
| **23** | 2h | Django Admin | Habilitar a interface de gerenciamento nativa para inserção de dados de teste. | Criação de um `superuser` e registro do modelo no `admin.py`. | Cadastro manual de 3 alunos de teste pela interface administrativa. | - |
| **24** | 2h | ORM Básico: Consultas (Read) | Compreender como buscar dados do banco usando `Model.objects.all()`. | Modificação da view de Alunos para buscar registros reais do banco de dados. | Substituição da tabela estática de Alunos por dados dinâmicos da tabela. | Formativa |
| **25** | 2h | Exibindo Dados no Template | Dominar a estrutura de repetição `{% for %}` para listar os dados buscados pela view. | Escrita do laço no HTML para gerar as linhas da tabela dinamicamente. | Exibição em tela dos alunos inseridos via Django Admin. | **Início da AMT 2** |
| **26** | 2h | Criando Dados (Create): Forms | Compreender a captura de dados via requisições POST e formulários HTML comuns. | Criação de uma página contendo um formulário HTML estruturado para o Aluno. | Criação da tela `/alunos/novo/` para cadastro de novos atletas. | - |
| **27** | 2h | Processando o Salvamento | Aprender a receber dados do dicionário `request.POST` e invocar o método `.save()`. | Escrita da lógica de validação básica e salvamento do aluno na view. | Fluxo completo de cadastro de alunos funcionando de ponta a ponta. | Formativa |
| **28** | 2h | Remoção de Dados (Delete) | Compreender a passagem de parâmetros via URL (IDs) para exclusão de registros. | Configuração de rotas dinâmicas como `<int:id>/deletar/` e chamada do `.delete()`. | Inclusão de um botão "Excluir" em cada linha da tabela de Alunos. | **Avaliação 3 (Prática)** |
| **29** | 2h | Atualização de Dados (Update) | Combinar a lógica de busca por ID, preenchimento do form e salvamento. | Criação de rota para edição, recuperação do objeto com `get_object_or_404` e re-salvamento. | Inclusão de um botão "Editar" que abre o formulário pré-preenchido. | - |
| **30** | 2h | Consolidando o CRUD do Aluno | Fixar o ciclo completo do CRUD revisando rotas, views e templates. | Refatoração de caminhos e validação visual de mensagens de sucesso. | CRUD completo da entidade Aluno 100% operacional. | Formativa |
| **31** | 2h | Model Exercício | Replicar os conhecimentos adquiridos criando a segunda tabela independente do sistema. | Escrita do modelo `Exercicio`, execução de migrations e registro no Admin. | Definição dos campos Nome do Exercício e Grupo Muscular. | - |
| **32** | 2h | CRUD Rápido do Exercício | Estimular a autonomia aplicando a repetição de padrões para criar telas semelhantes. | Desenvolvimento da listagem, cadastro e exclusão para a entidade Exercício. | CRUD da entidade Exercício finalizado pelos próprios alunos. | Formativa |
| **33** | 2h | Relacionamentos: ForeignKey | Compreender o conceito de chave estrangeira aplicado ao ORM do Django. | Criação do modelo `Treino` contendo um campo `ForeignKey` apontando para `Aluno`. | Amarração lógica: cada registro de treino agora pertence obrigatoriamente a um aluno. | - |
| **34** | 2h | Migrations com Relacionamentos | Resolver pendências de migração quando existem tabelas dependentes. | Execução de migrações em lote e testes de inserção via Django Admin. | Banco de dados totalmente estruturado no modelo relacional planejado. | Formativa |
| **35** | 2h | CRUD de Treinos com Seleção | Renderizar uma caixa de seleção (`<select>`) alimentada dinamicamente com dados de outra tabela. | Busca de todos os alunos no banco para exibir como opções no formulário de treino. | Criação da tela de agendamento/cadastro de treinos vinculados a alunos. | - |
| **36** | 2h | Ajustes Finais do Sistema | Garantir a coesão visual e funcional de todas as pontas do sistema integrado. | Testes manuais cruzados entre alunos para detectar falhas de integridade. | Aplicação "PersonalPro" completamente estável e preenchida. | **Entrega da AMT 2** |
| **37** | 2h | Oficina de Dúvidas e Laboratório | Oferecer espaço de mentoria focado para os alunos com atraso nas entregas. | Plantão de correções de bugs individuais nos códigos dos alunos. | Equalização do andamento técnico da turma. | Formativa |
| **38** | 2h | Avaliação Final Prática | Mensurar a capacidade de estender o sistema implementando uma funcionalidade do zero. | Adição individual de um novo campo ou pequena alteração estrutural sob supervisão. | Comprovação prática das habilidades de manipulação de banco e MVT. | **Avaliação 4 (Prática)** |
| **39** | 2h | Apresentação dos Projetos | Desenvolver habilidades de comunicação técnica demonstrando o software funcionando. | Demonstração breve da aplicação rodando localmente no laboratório. | Validação social do esforço produtivo do aluno. | Formativa |
| **40** | 2h | Encerramento e Conselho de Classe | Consolidação de resultados pedagógicos e encerramento das atividades. | Arquivamento dos códigos finais no GitHub e feedback de autoavaliação. | Conclusão do ciclo da disciplina. | Formativa |

---

## 5. Avaliações do 4º Bimestre

### Avaliação 3: Implementação do Primeiro Fluxo de Persistência (Create e Read)
* **Objetivo:** Avaliar a transição do front-end estático para uma aplicação dinâmica conectada ao banco de dados SQLite.
* **Critérios de Avaliação:**
  * Escrita correta do modelo `Aluno` com os tipos de campos adequados (25%)
  * Execução bem-sucedida das migrações sem corromper o banco (25%)
  * Construção da View de listagem puxando os dados via ORM (25%)
  * Renderização dinâmica do laço `{% for %}` no HTML exibindo os dados salvos (25%)
* **Forma de Entrega:** Execução da rotina ao vivo no computador do laboratório.
* **Valor Sugerido:** 30 Pontos.

### Avaliação 4: CRUD Completo e Relacionamento de Tabelas (Projeto Integrador)
* **Objetivo:** Avaliar a entrega final do sistema, focando no funcionamento dos formulários de modificação (Update/Delete) e na integridade do relacionamento ForeignKey.
* **Critérios de Avaliação:**
  * Funcionamento correto e seguro da edição e exclusão de registros (30%)
  * Implementação correta da ForeignKey relacionando Treinos a Alunos (30%)
  * Renderização dinâmica do componente `<select>` populado com dados do banco (20%)
  * Ausência de erros de execução internos do Django (Erros 500) durante o uso ordinário (20%)
* **Forma de Entrega:** Envio do link final do repositório no GitHub acompanhado de uma arguição prática de 3 minutos no laboratório.
* **Valor Sugerido:** 50 Pontos.

### Atividade Mediada por Tecnologia (AMT 2): Screencast Técnico explicativo
* **Objetivo:** Avaliar a compreensão do código escrito, mitigando cópias literais e garantindo que o aluno saiba explicar a lógica estruturada.
* **Critérios de Avaliação:**
  * Clareza na gravação (áudio e vídeo compreensíveis) (20%)
  * Demonstração prática do CRUD funcionando no navegador (incluindo inserção e checagem no Admin) (40%)
  * Explicação sucinta de onde estão localizadas as rotas, a view e o model da funcionalidade demonstrada (40%)
* **Forma de Entrega:** Gravação de um vídeo de **no máximo 3 minutos** (via ferramentas como Loom ou Clipchamp) com envio do link na plataforma oficial.
* **Valor Sugerido:** 20 Pontos.

---

## 6. Evolução do Projeto Integrador Aula por Aula (Resumo de Engenharia)

O sistema de gerenciamento de treinos evoluirá conforme os passos lógicos a seguir:

1. **Aulas 01 a 04:** O projeto nasce vazio no terminal (`personalpro`). Configura-se a estrutura interna e cria-se o aplicativo principal `core`.
2. **Aulas 05 a 07:** O sistema ganha as primeiras rotas. Acessar `/` exibe uma página de boas-vindas simples em HTML puro.
3. **Aulas 09 a 11:** O visual melhora. Cria-se o arquivo `base.html` que desenha uma barra de navegação superior azul (Bootstrap) que se repetirá por todo o sistema.
4. **Aulas 12 a 16:** O usuário clica nos links do menu e consegue navegar por páginas estáticas vazias: `/alunos/`, `/exercicios/` e `/treinos/`, povoadas com tabelas simuladas.
5. **Aulas 21 a 23:** O banco de dados ganha vida. A classe `Aluno` vira uma tabela no SQLite. O professor entra na rota `/admin/` e cadastra os primeiros alunos reais.
6. **Aulas 24 a 25:** A página `/alunos/` deixa de exibir dados falsos e passa a listar os nomes reais cadastrados no passo anterior.
7. **Aulas 26 a 30:** Adiciona-se o botão "Cadastrar Aluno". Abre-se um formulário limpo que salva registros na tabela. Em seguida, adicionam-se os botões de "Editar" e "Excluir" em cada linha.
8. **Aulas 31 a 32:** O mesmo processo do ciclo de Alunos é replicado rapidamente para a tabela de `Exercicio` (Supino, Corrida, Leg Press).
9. **Aulas 33 a 36:** O ápice do projeto. Cria-se a tabela `Treino`. Ao cadastrar um treino, o sistema exibe uma caixa de seleção contendo a lista de alunos cadastrados dinamicamente, permitindo associar uma rotina de exercícios àquele aluno específico de forma persistente.

---

## 7. Metodologias Ativas Utilizadas

* **Aulas Expositivas Dialogadas Curtas (MÁXIMO 20-30 MIN):** Explicação focada no quadro ou projetor sobre o conceito do dia, abrindo espaço imediato para testes.
* **Estudo Dirigido com Codificação Guiada (*Live Coding*):** O professor escreve trechos de código em tempo real no projetor, explicando os erros de digitação mais comuns que travam a execução do framework.
* **Instrução aos Pares (*Peer Instruction*):** Alunos que concluem os desafios diários mais rápido são estimulados a apoiar os colegas que estão enfrentando erros de sintaxe ou configuração nos computadores vizinhos.
* **Aprendizagem Baseada em Projetos (PBL):** O engajamento é mantido alto porque o aluno percebe o crescimento prático e cumulativo de um sistema real, fugindo de exercícios isolados que não fazem sentido sistêmico.

---

## 8. Recursos Didáticos

* **Laboratório de Informática:** Computadores individuais com interpretador Python instalado e editores de código configurados.
* **Projetor Multimídia (Datashow):** Utilizado pelo docente para demonstração ao vivo da escrita do código e análise dos logs do terminal do Django.
* **Quadro Branco:** Essencial para desenhar o fluxo de requisições do MVT e ilustrar as relações das tabelas (Chave Estrangeira) de forma visual antes de ir para o código.
* **Ambiente Virtual de Aprendizagem (AVA/Moodle/Google Classroom):** Centralizador para postagem de links de referência, códigos de exemplo estruturados e espaço de entrega das AMTs.

---

## 9. Bibliografia Básica

1. **DOCUMENTAÇÃO OFICIAL DO DJANGO.** *Django Documentation.* Disponível em: <https://docs.djangoproject.com/>.
2. **BOOTSTRAP TEAM.** *Bootstrap Docs.* Disponível em: <https://getbootstrap.com/>.
3. **MELO, Alexandre S.** *Desenvolvimento Web com Python e Django.* Editora Novatec, 2021.