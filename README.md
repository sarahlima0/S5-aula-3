# S5-aula-3
# Plano de Ação para a Criação e Estruturação do Repositório

## 1. Definição de Padrões de Branches

Para manter um fluxo de trabalho organizado, adotaremos os seguintes padrões de branches:

- **main**: Branch principal que conterá o código em produção. Apenas o código testado e aprovado será integrado aqui.
- **develop**: Branch de desenvolvimento que conterá a versão mais recente e estável do código em desenvolvimento. Todas as novas funcionalidades e correções serão integradas nesta branch antes de serem movidas para a `main`.
- **feature/xxx**: Branches para desenvolvimento de novas funcionalidades, nomeadas como `feature/nome-da-funcionalidade`.
- **bugfix/xxx**: Branches para correção de bugs, nomeadas como `bugfix/descrição-do-bug`.
- **release/xxx**: Branches para preparar uma nova versão de lançamento, nomeadas como `release/versão`.
- **hotfix/xxx**: Branches para corrigir bugs críticos na `main`, nomeadas como `hotfix/descrição-do-hotfix`.

## 2. Organização de Diretórios e Arquivos

A estrutura de diretórios será a seguinte para facilitar o acesso e entendimento:

## 3. Criação do Repositório no GitHub

**Passos para a criação e configuração inicial do repositório:**

1. **Criar o repositório no GitHub**:
   - Acesse o GitHub e clique em "New Repository".
   - Nomeie o repositório (ex.: `delivery-app`).
   - Adicione uma descrição breve.
   - Selecione "Public" ou "Private", conforme necessário.
   - Inicialize com um `README.md`.

2. **Configurações iniciais**:
   - Adicione `.gitignore` para Node.js.
   - Adicione uma licença adequada (ex.: MIT License).
   - Configure branch protection rules para `main` e `develop`.

3. **Permissões de acesso**:
   - Adicione todos os membros do time como colaboradores.
   - Defina permissões de acesso adequadas (ex.: write access para desenvolvedores, admin access para leads).

## 4. Plano Inicial de Configuração e Primeiro Commit

1. **Clonar o repositório**:
   ```bash
   git clone https://github.com/user/repository.git
   git checkout -b develop
   git push origin develop
   git add .
   git commit -m "Initial commit with project structure"
   git push origin develop

 4. **Adicione e faça commit das mudanças**:
   ```bash
   git add README.md
   git commit -m "Add project planning and structure to README"
   git push origin main
