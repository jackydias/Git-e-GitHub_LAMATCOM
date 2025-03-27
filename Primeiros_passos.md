# Primeiro dia
Instalando e configurando o Git e GitHub
============

### Windows
- Acessar o site do [Git](https://git-scm.com/downloads) para fazer o download do instalador.
- Clique em "Download for Windows".
- Execute o instalador baixado e siga as instrução.
 
### Ubuntu
  - A instalação é via terminal
  - Abra um terminal e digite
    ```Git
    sudo apt-get update
    sudo apt-get install git
    ```

### Verificando a versão do Git
- Abra um terminal e digite...
```
git --version
```

### Criando conta no GitHub
- Acessar o site do [GitHub](https://github.com/) para fazer o cadastro.
  
### Configuração Inicial:

- Após a instalação do Git e criação da conta no GitHub, abra um terminal.

- Configure seu nome de usuário e endereço de e-mail:

```
git config --global user.name "seu_nome"
git config --global user.email "seu@email.com"
```
### Verificando se a configuração deu certo 
```
git config --list
```

### Fazendo fork de um repositório 
- Acesse o repositório original e click na opção 'fork'
- Faça uma modificação em qualquer arquivo do repositório, preencha o commit e click na opção 'Pull request'
- Na tela do 'Pull request' click em 'Create pull requeste'

### Clonando um repositório remoto para o computador local
- Copie o endereço https do repositório
- Abra o terminal no diretorio onde deseja clonar o repositório e digite
```
git clone "cole o endereço_https"
```
### Fazendo alterações no repositório
- Faça alguma alteração em algum arquivo do seu repositório
- Inclua as alterações digitando
```
git add .
git commit -m "mensagem"
git push origin main
```

### Criando um repositório local
- Crie o repositório no GitHub com o mesmo nome da pasta criada no computador
- Crie uma pasta no seu computador e insira seus docs
- Abra um terminal e digite
  
```
git init
git add .
git commit -m "mensagem"
git branch -M main
git branch
git remote add origin "endereço do repositório"
git push -u origin main
```



Comandos Git
============

### Obtendo & Criação de Projetos

| Comando | Descrição |
| ------- | --------- |
| `git init` | Inicializa um repositório Git local |
| `git clone ssh://git@github.com/[usuario]/[nome-repositorio].git` | Cria uma cópia local de um repositório remoto |

### Básicos

| Comando | Descrição |
| ------- | --------- |
| `git status` | Checa o status |
| `git add [nome-arquivo.txt]` | Adiciona um arquivo para área de stage |
| `git add -A` | Adiciona todos os arquivos novos ou modificados para a área de stage |
| `git commit -m "[Mensagem de Commit]"` | Comita as alterações |
| `git rm -r [nome-arquivo.txt]` | Remove um arquivo (ou pasta) |

### Branching & Merging

| Comando | Descrição |
| ------- | --------- |
| `git branch` | Lista as branches (o asterisco denota a branch atual) |
| `git branch -a` | Lista todas as branches (local e remoto) |
| `git branch [nome da branch]` | Cria uma nova branch |
| `git branch -d [nome da branch]` | Deleta uma branch |
| `git push origin --delete [nome da branch]` | Deleta uma branch remota |
| `git checkout -b [nome da branch]` | Cria uma nova branch e muda para ela |
| `git checkout -b [nome da branch] origin/[nome da branch]` | Clona uma branch remota e muda para ela |
| `git checkout [nome da branch]` | Seleciona uma branch |
| `git checkout -` | Muda para a última branch |
| `git checkout -- [nome-arquivo.txt]` | Descarta modificações de um arquivo |
| `git merge [nome da branch]` | Faz um merge de uma branch na branch atual |
| `git merge [source branch] [branch alvo]` | Faz um merge de uma branch em outra branch |
| `git stash` | Tirar o estado sujo do seu diretório de trabalho |
| `git stash clear` | Remove todas as entradas 'stash' |

### Sharing & Updating Projects

| Comando | Descrição |
| ------- | --------- |
| `git push origin [nome da branch]` | Enviar uma branch para seu repositório remoto |
| `git push -u origin [nome da branch]` | Envia as alterações da branch informada para um repositório remoto (and selecionar a branch) |
| `git push` | Envia as alterações para o repositório remoto (branch atual) |
| `git push origin --delete [nome da branch]` | Deletar uma branch remota |
| `git pull` | Atualiza o repositório local para o último commit |
| `git pull origin [nome da branch]` | Recebe alterações do repositório remoto |
| `git remote add origin ssh://git@github.com/[usuario]/[nome-repositorio].git` | Adicionar um repositório remoto |
| `git remote set-url origin ssh://git@github.com/[usuario]/[nome-repositorio].git` | Seta um repositório da origin branch para o SSH |

### Inspeção & Comparação

| Comando | Descrição |
| ------- | --------- |
| `git log` | Ver modificações |
| `git log --summary` | Ver modificações (detalhadas) |
| `git diff [branch original] [branch alvo]` | Visualizar alterações antes de mesclar |







Jacky Ramires Dias
