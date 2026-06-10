# Plano de Ensino e Cronograma Semestral: Programação Web com Django
**Carga Horária Total:** 80 Horas (40 encontros de 2 horas-aula)  
**Divisão Escolar:** 3º Bimestre (40h / 20 Aulas) | 4º Bimestre (40h / 20 Aulas)  
**IDE de Desenvolvimento:** PyCharm Community Edition  

---

## 3º Bimestre: Imersão Teórica e Fluxo MVT Completo (40 horas)
*Foco Pedagógico: Aulas expositivas e práticas em regime de Code-Along. O professor desenvolve o "Sistema de Controle de Treinos" no projetor e os alunos replicam no PyCharm.*

| Aula | C.H. | Conteúdo e Atividade Prática no PyCharm | Avaliação / Entregável |
| :--- | :--- | :--- | :--- |
| **1** | 2h | **Apresentação e Setup:** Criação do projeto puro (*Pure Python*) no PyCharm. Ativação automática da `venv` e instalação do Django via terminal embutido (`pip install django`). | Diagnóstica |
| **2** | 2h | **Estrutura de Arquivos:** Criação do projeto central (`core .`) e do primeiro App (`cadastro`) via terminal. Análise da árvore de arquivos no painel *Project* da IDE. | Acompanhamento |
| **3** | 2h | **URLs e Views Básicas:** Configuração de rotas e criação da primeira View retornando uma resposta de texto simples com `HttpResponse`. | Acompanhamento |
| **4** | 2h | **A Camada de Templates:** Criação da pasta `templates/` e uso da função `render()` para exibir páginas HTML isoladas da lógica Python. | Acompanhamento |
| **5** | 2h | **Arquivos Estáticos:** Configuração do `STATIC_URL` no `settings.py` e organização das pastas de CSS e JS locais. | Acompanhamento |
| **6** | 2h | **Integração do Bootstrap:** Download do Bootstrap para a pasta static e criação do template estrutural `base.html` utilizando as tags de herança `{% block %}`. | Acompanhamento |
| **7** | 2h | **Dados Dinâmicos:** Passagem de dicionários de contexto a partir da View e exibição de variáveis no HTML com a sintaxe `{{ variavel }}`. | Acompanhamento |
| **8** | 2h | **Controle de Fluxo no HTML:** Uso prático das tags `{% for %}` para gerar linhas de tabelas dinâmicas e `{% if %}` para exibir alertas de lista vazia. | **AVALIAÇÃO 1: Entrega da Maquete MVT funcional (Peso 4,0)** |
| **9** | 2h | **Introdução aos Models:** Mapeamento de dados com a criação do model `Aluno`. Execução dos comandos `makemigrations` e `migrate` no terminal do PyCharm. | Acompanhamento |
| **10** | 2h | **Django Admin:** Registro do model no arquivo `admin.py`, criação do superusuário (`createsuperuser`) e inserção de dados de teste pelo painel nativo. | Acompanhamento |
| **11** | 2h | **Mapeamento Relacional:** Conceito de chave estrangeira com a criação dos models `Exercicio` e `Treino` utilizando `models.ForeignKey(..., on_delete=models.CASCADE)`. | Acompanhamento |
| **12** | 2h | **Consultas com ORM (Read):** Modificação das Views para extrair dados reais do banco SQLite via `Aluno.objects.all()` e renderização na tabela customizada. | Acompanhamento |
| **13** | 2h | **Rotas Dinâmicas:** Criação da página de perfil/detalhes do aluno capturando parâmetros numéricos na URL (`<int:id>`) e usando o método `.get(id=id)`. | Acompanhamento |
| **14** | 2h | **Formulários Django (Create):** Criação do arquivo `forms.py` e declaração de uma classe baseada em `forms.ModelForm` para automatizar inputs HTML. | Acompanhamento |
| **15** | 2h | **Persistência via POST:** Manipulação de requisições POST na View, validação com `form.is_valid()`, uso obrigatório do `{% csrf_token %}` e redirecionamento de página. | Acompanhamento |
| **16** | 2h | **Atualização de Dados (Update):** Construção da rota e View de edição de registros passando o objeto selecionado como `instance` para o formulário. | Acompanhamento |
| **17** | 2h | **Remoção de Dados (Delete):** Implementação da lógica de exclusão física de registros do banco através do método `.delete()` com página de confirmação. | Acompanhamento |
| **18** | 2h | **CRUD Relacional:** Desenvolvimento do formulário de cadastro de `Treino`, testando a geração automática do elemento `<select>` com os Alunos do banco. | Acompanhamento |
| **19** | 2h | **Versionamento e Limpeza:** Refatoração de código com apoio das ferramentas de inspeção do PyCharm e versionamento final do projeto base via Git/GitHub. | Acompanhamento |
| **20** | 2h | **Consolidação Técnica:** Laboratório de fechamento para correção de bugs e alinhamento do projeto que servirá de consulta para o próximo bimestre. | **AVALIAÇÃO 2: Entrega do CRUD Base Funcional (Peso 6,0)** |

---

## 4º Bimestre: Oficina de Desenvolvimento de Projetos Autorais (40 horas)
*Foco Pedagógico: Regime de laboratório/oficina aplicada. Os alunos trabalham em equipes (ou individualmente) desenvolvendo um sistema de livre escolha, aplicando o passo a passo consolidado no bimestre anterior.*

| Aula | C.H. | Conteúdo e Atividade Prática no PyCharm | Avaliação / Entregável |
| :--- | :--- | :--- | :--- |
| **21** | 2h | **Definição de Temas e Escopo:** Apresentação das propostas dos alunos. Definição do escopo limitado (exatamente 3 models com relacionamento 1:N). | Pitch do Tema |
| **22** | 2h | **Modelagem de Dados:** Desenho do diagrama de tabelas e planejamento das propriedades e tipos de campos para o tema escolhido. | Diagrama de Dados |
| **23** | 2h | **Setup dos Projetos Próprios:** Inicialização de um novo projeto no PyCharm pelos grupos, isolamento de apps e configuração do repositório Git dedicado. | Repositório Ativo |
| **24** | 2h | **Design da Interface Base:** Desenvolvimento do arquivo `base.html` customizado com a identidade visual do tema escolhido pelo grupo usando Bootstrap. | Casca Visual |
| **25** | 2h | **Roteamento Inicial:** Mapeamento das primeiras URLs, Views e Templates de Dashboard para a Home Page do novo sistema. | Navegação Estática |
| **26** | 2h | **Tradução de Models:** Escrita das classes correspondentes às entidades do grupo no arquivo `models.py`, validando as chaves estrangeiras. | Código dos Models |
| **27** | 2h | **Migração de Banco:** Geração e execução das migrations nos projetos autônomos para estruturar o arquivo `db.sqlite3` do grupo. | Base SQLite Pronta |
| **28** | 2h | **Admin nos Projetos Livres:** Habilitação e customização das colunas de visualização dos novos models dentro da interface do Django Admin. | Painel Admin Ativo |
| **29** | 2h | **Alimentação da Base de Teste:** Cadastro manual de dados estruturados através do painel Admin para validar a integridade das tabelas criadas. | **AVALIAÇÃO 3: Modelagem e Painel Admin dos Projetos Livres (Peso 4,0)** |
| **30** | 2h | **Oficina de Consulta (Read - Listagem):** Construção das tabelas HTML dinâmicas puxando as coleções do banco via ORM para as telas de listagem. | Telas de Listagem |
| **31** | 2h | **Oficina de Consulta (Read - Detalhes):** Implementação de rotas dinâmicas capturando IDs para abrir páginas de perfil isoladas de registros. | Páginas de Detalhes |
| **32** | 2h | **Oficina de Escrita (Create - Formulários):** Desenvolvimento dos arquivos `forms.py` específicos para capturar entradas de dados do sistema autônomo. | Criação de Forms |
| **33** | 2h | **Oficina de Escrita (Create - Lógica):** Acoplamento das views para processar envios POST, validar preenchimentos e persistir dados no banco local. | Cadastro Operando |
| **34** | 2h | **Oficina de Escrita (Update):** Criação das rotas, botões de ação e lógicas para alteração/edição de dados nos projetos dos alunos. | Edição Operando |
| **35** | 2h | **Oficina de Escrita (Delete):** Implementação da rota de remoção física de dados com telas de aviso e proteção para o usuário final. | CRUD Completo |
| **36** | 2h | **Oficina de Relacionamentos:** Ajustes finos nas telas e formulários que envolvem chaves estrangeiras para garantir vínculos consistentes entre tabelas. | Vínculos Funcionais |
| **37** | 2h | **Polimento Visual com Bootstrap:** Ajustes estéticos nos inputs gerados pelo Django Forms utilizando classes de estilização responsiva. | Interface Polida |
| **38** | 2h | **Auditoria de Código e Testes Cruzados:** Período para os grupos testarem os sistemas uns dos outros à procura de bugs ou erros 500 no terminal. | Resolução de Bugs |
| **39** | 2h | **Finalização de Documentação e Git:** Commits finais de fechamento, limpeza de linhas de código ociosas e escrita do arquivo `README.md` do projeto. | Upload Final Git |
| **40** | 2h | **Mostra Técnica / Apresentação Final:** Demonstração prática em laboratório do sistema autônomo funcionando de ponta a ponta. | **AVALIAÇÃO 4: Apresentação Técnica do Produto Web Autônomo (Peso 6,0)** |

---

### Orientações Práticas para Execução no PyCharm Community

* **Gerenciamento do Servidor:** Relembre os alunos nas primeiras aulas de que o comando `python manage.py runserver` deve ser digitado manualmente na aba *Terminal* da IDE e que para interromper o processo para rodar uma migração basta pressionar `Ctrl + C`.
* **Criação de Arquivos HTML:** No PyCharm Community, ao criar arquivos dentro da pasta `templates/`, oriente a turma a clicar com o botão direito $\rightarrow$ *New* $\rightarrow$ *HTML File*, o que já gera a estrutura HTML5 base facilitando o trabalho.
