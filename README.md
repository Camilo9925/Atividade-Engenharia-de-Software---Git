🧩 Task Manager API

📌 Descrição

O Task Manager API é um sistema simples para gerenciamento de tarefas, desenvolvido com o objetivo de simular um ambiente profissional de desenvolvimento utilizando boas práticas de versionamento com Git.

A aplicação permite operações básicas de um CRUD:

- Criar tarefas
- Listar tarefas
- Atualizar tarefas
- Deletar tarefas

«⚠️ Observação: O foco deste projeto não é a implementação da lógica de negócio, mas sim a adoção de um fluxo profissional de versionamento com Git.»

---

🚀 Tecnologias Utilizadas

- Estrutura baseada em backend e frontend (simulada)
- Arquivos ".txt" para representação das funcionalidades
- Git e GitHub para controle de versão

---

▶️ Como Rodar o Projeto

Este projeto é apenas estrutural, portanto não há necessidade de instalação de dependências.

Passos:

git clone <URL_DO_REPOSITORIO>
cd task-manager-api

---

🌳 Estratégia de Branches

O projeto segue uma adaptação do modelo Git Flow:

- "main" → ambiente de produção
- "develop" → ambiente de integração
- "feature/*" → desenvolvimento de novas funcionalidades
- "hotfix/*" → correções urgentes em produção

---

🔄 Fluxo de Desenvolvimento

O fluxo adotado segue um padrão profissional:

1. Criar uma branch a partir da "develop"
   
   git checkout develop
git checkout -b feature/nome-da-feature

2. Realizar commits organizados

3. Subir a branch
   
   git push origin feature/nome-da-feature

4. Abrir Pull Request (PR) para "develop"

5. Revisar e realizar merge na "develop"

6. Para release:
   
   git checkout main
git merge develop

---

📝 Padrão de Commits

Este projeto utiliza Conventional Commits:

- "feat:" → nova funcionalidade
- "fix:" → correção de bug
- "docs:" → documentação
- "refactor:" → melhoria interna de código
- "chore:" → tarefas gerais (configuração, inicialização)

Exemplos:

feat: adiciona criação de tarefas
fix: corrige erro ao deletar tarefa
docs: atualiza README
refactor: reorganiza estrutura do projeto

---

🔢 Versionamento

O projeto segue o padrão de Versionamento Semântico (SemVer):

Formato:

Versões:

- "v1.0.0" → primeira release estável
- "v1.0.1" → correção de bug (hotfix)
- "v1.1.0" → adição de novas funcionalidades

Criação de tags:

- git tag v1.0.0
- git push origin v1.0.0

---

🐞 Hotfix (Correção em Produção)

Fluxo para correção emergencial:

git checkout main
git checkout -b hotfix/nome-do-bug

# corrigir problema
git commit -m "fix: descrição do problema"

git checkout main
git merge hotfix/nome-do-bug
git tag v1.0.1
git push origin main --tags

# importante: sincronizar com develop
git checkout develop
git merge hotfix/nome-do-bug

---

🔀 Pull Requests

Cada funcionalidade deve conter um Pull Request com:

- Descrição clara do que foi implementado
- Justificativa da mudança
- Como testar

Exemplo de PR:

Título: feat: adiciona criação de tarefas

Descrição:

- Implementa funcionalidade de criação de tarefas
- Adiciona estrutura inicial no backend

Como testar:

- Verificar conteúdo do arquivo "backend/arquivo.txt"

---

📂 Estrutura do Projeto

src/
├── backend/
│   └── atualizarTarefa.txt
│   └── CorrigindoBug.txt
│   └── criarTarefa.txt
│   └── deletarTarefa.txt
│   └── ListarTarefa.txt
├── frontend/
│   └── arquivo2.txt
├── .gitignore
├── README.md
└── LICENSE

---

📦 Releases

As versões do projeto são marcadas com tags no Git.

Para visualizar:

git tag

Ou diretamente na plataforma (GitHub/GitLab) na aba de Releases.

---

📄 Licença

Este projeto está sob a licença MIT.

---

✅ Objetivo Acadêmico

Este projeto foi desenvolvido com fins educacionais para simular:

- Uso profissional do Git
- Organização de branches
- Fluxo de desenvolvimento em equipe
- Versionamento semântico
- Boas práticas de commits

---