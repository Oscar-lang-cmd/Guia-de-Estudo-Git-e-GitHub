# GUIA COMPLETO DE GIT E GITHUB 😎🚀

-----------------------------------------
SEÇÃO 1: INTRODUÇÃO AO GIT E GITHUB 
-----------------------------------------
- **O que é Git?**
  - Sistema de Controle de Versão Distribuído (DVCS).
  - Funciona offline e salva o histórico de alterações localmente.

- **O que é GitHub?**
  - Plataforma de hospedagem e colaboração para projetos Git.
  - Permite versionamento remoto, compartilhamento e trabalho em equipe.

- **Diferenças entre Git e GitHub:**
  - GIT: Gerencia versões localmente.
  - GITHUB: Hospeda repositórios Git na nuvem.

-----------------------------------------
SEÇÃO 2: CONFIGURANDO O GIT
-----------------------------------------
1. Configurar nome e email:
   $ git config --global user.name "Seu Nome"
   $ git config --global user.email "Seu Email"

2. Alterar branch padrão para `main`:
   $ git config --global init.defaultBranch main

3. Ver configurações atuais:
   $ git config --global --list

-----------------------------------------
SEÇÃO 3: INICIANDO UM REPOSITÓRIO
-----------------------------------------
1. Criar um repositório local:
   $ git init - inicia um repositório local git 

2. Clonar um repositório remoto:
   $ git clone <URL>

-----------------------------------------
SEÇÃO 4: FLUXO BÁSICO DE TRABALHO
-----------------------------------------
1. Adicionar arquivos ao stage:
   $ git add arquivo.txt
   $ git add .  (Adiciona todos os arquivos)

2. Fazer um commit:
   $ git commit -m "Descrição do commit"
   
3. Vincular o respositório local com o respositório remoto
  $ git remote add origin main <URL> do repositório remoto

4. Enviar para o repositório remoto:
   $ git push -u origin main

5. Atualizar com alterações do remoto:
   $ git pull origin main

6. Verificar status dos arquivos:
   $ git status

-----------------------------------------
SEÇÃO 5: TRABALHANDO COM BRANCHES
-----------------------------------------
1. Criar uma nova branch:
   $ git checkout -b "nome da nova branch"

2. Alternar entre branches:
   $ git checkout "nome da branch desejada"

3. Excluir uma branch:
   $ git branch -d "nome da nova branch"

-----------------------------------------
SEÇÃO 6: RESOLUÇÃO DE CONFLITOS
-----------------------------------------
1. Atualizar repositório local:
   $ git pull origin main

2. Resolver conflitos manualmente.

3. Salvar ajustes:
   $ git add arquivo.txt

4. Commitar resoluções:
   $ git commit -m "Conflitos resolvidos"

5. Enviar alterações ao remoto:
   $ git push origin main

-----------------------------------------
SEÇÃO 7: DESFAZER ALTERAÇÕES
-----------------------------------------
1. Reverter arquivo ao estado original:
   $ git restore arquivo.txt

2. Remover commits recentes:
   a) Manter alterações no stage:
      $ git reset --soft <hash>
   b) Manter alterações no diretório:
      $ git reset --mixed <hash>
   c) Descartar todas as alterações:
      $ git reset --hard <hash>

3. Alterar última mensagem de commit:
   $ git commit --amend -m "Nova mensagem"

-----------------------------------------
SEÇÃO 8: TRABALHANDO COM .GITIGNORE
-----------------------------------------
1. Criar um arquivo `.gitignore` para ignorar arquivos ou pastas:
   $ echo "nome_arquivo" > .gitignore
   $ git add .gitignore
   $ git commit -m "Adicionando .gitignore"

-----------------------------------------
SEÇÃO 9: COMANDOS ÚTEIS NO DIA A DIA
-----------------------------------------
- Verificar status do repositório:
  $ git status

- Exibir histórico de commits:
  $ git log

- Listar branches:
  $ git branch

- Ver repositórios remotos configurados:
  $ git remote -v

- Arquivar mudanças temporárias:
  $ git stash
  $ git stash list

-----------------------------------------
SEÇÃO 10: DICAS IMPORTANTES
-----------------------------------------
1. Sempre resolva conflitos manualmente com atenção.
2. Use `git reset --hard` com cuidado, pois é irreversível.
3. Configure chaves SSH para autenticação com o GitHub.
4. Faça backups usando `git reflog`.

# FIM DO GUIA

