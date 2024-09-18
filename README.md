# MeuPrimeiroCommit
# MeuPrimeiroCommit
## Configuração Inicial

**Configurar Nome e E-mail: Estes são usados para identificar suas mudanças nos commits.**
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"

**Verificar Configurações: Para listar as configurações atuais do Git.**
git config --list

## Gerenciamento de Repositórios

**Criar um Novo Repositório:**
*Inicializa um novo repositório Git no diretório atual.*
git init

**Clonar um Repositório Existente:**
*Clona um repositório remoto para o seu diretório local.*
git clone https://github.com/username/repository.git

## Trabalhando com Arquivos
*Adicionar Arquivos ao Controle de Versão:*
*Adicionar um arquivo específico:*
git add nome-do-arquivo.txt

*Adicionar todos os arquivos modificados:*
git add .

**Verificar o Status dos Arquivos:**
*Mostra quais arquivos foram modificados, adicionados ou deletados.*   
git status

**Remover Arquivos do Controle de Versão:**
*Remove um arquivo do repositório e do diretório de trabalho.*
git rm nome-do-arquivo.txt

**Commit e Histórico**
*Fazer um Commit das Alterações:*
*Adiciona as mudanças ao histórico do repositório com uma mensagem descritiva.*
git commit -m "Mensagem descritiva do commit"

**Verificar o Histórico de Commits:**
*Mostra o histórico de commits, incluindo IDs, autores e mensagens.*
git log

**Verificar Diferenças entre Commits:**
*Mostra as diferenças entre arquivos modificados e o último commit.*

## Trabalhando com Branches

**Criar uma Nova Branch:**
*Cria uma nova branch com o nome especificado.*
git branch nome-da-branch

**Mudar para uma Branch:**
*Muda para a branch especificada.*
git checkout nome-da-branch

*Ou combine com a criação de uma nova branch:*
git checkout -b nome-da-branch

**Mesclar Branches:**
*Mescla as mudanças da branch especificada na branch atual.*
git merge nome-da-branch

**Excluir uma Branch:**
*Remove uma branch local.*
git branch -d nome-da-branch
*Use -D para forçar a exclusão, mesmo se houver mudanças não mescladas.*

## Trabalhando com Repositórios Remotos

**Adicionar um Repositório Remoto:**
*Associa um repositório remoto com um nome (geralmente origin).*
git remote add origin https://github.com/username/repository.git

**Enviar Commits para o Repositório Remoto:**
*Envia suas mudanças para a branch especificada no repositório remoto.*
git push origin nome-da-branch

**Puxar Mudanças do Repositório Remoto:**
*Atualiza sua branch local com mudanças do repositório remoto.*
git pull origin nome-da-branch

**Verificar Repositórios Remotos:**
*Mostra os URLs dos repositórios remotos associados.*
git remote -v

## Resolução de Conflitos e Outras Operações
**Resolver Conflitos de Merge:**
*Após um merge que gera conflitos, edite os arquivos para resolver os conflitos e, em seguida:*
git add nome-do-arquivo-resolvido
git commit

**Reverter um Commit:**
*Cria um novo commit que desfaz as alterações do commit especificado.*
git revert ID-do-commit

**Resetar o Repositório para um Estado Anterior:**
*Atenção: Esse comando altera o histórico e pode causar perda de dados se não for usado corretamente.*
git reset --hard ID-do-commit

