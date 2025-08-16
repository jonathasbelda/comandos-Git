
# Comandos Básicos de SQL

## ⌨ CONFIGURAR UM NOVO PROJETO
Para configurar um novo projeto no **Git**, o primeiro passo é inicializar um repositório local usando o comando **git init**. Em seguida, adicione os arquivos ao repositório com **git add** e crie um commit inicial com **git commit**. Finalmente, conecte seu repositório local a um repositório remoto (como GitHub) usando **git remote add origin** e envie suas alterações com **git push**. 

<br>

**PASSOS DETALHADOS:**

**1. Inicializar o repositório local:**

```
-- Inicializar o repositório local:
-- Abra o terminal ou prompt de comando e navegue até a pasta do seu projeto. 
-- Execute o comando git init para criar um novo repositório Git na pasta

```
<br>

**2. Adicionar arquivos ao repositório:**
```
-- Use o comando git add seguido do nome do arquivo ou para adicionar todos os arquivos da pasta. Ex: git add . 
-- Para adicionar arquivos específicos, use git add nome_do_arquivo. 

```

<br>

**3. Criar o primeiro commit:**

```
-- Após adicionar os arquivos, use git commit -m "Mensagem do commit" para criar um commit com uma descrição do que foi adicionado. Ex: git commit -m "Initial commit"

```

<br>

**4. Conectar ao repositório remoto (opcional, se já existir um repositório remoto):**

```
-- Se você já tem um repositório remoto (por exemplo, no GitHub), copie a URL do repositório. 
-- Execute o comando git remote add origin URL_DO_REPOSITORIO_REMOTO para adicionar a origem remota. 
-- Ex: git remote add origin git@github.com:usuario/meu-projeto.git. 

```

**5. Enviar as alterações para o repositório remoto:**

```
-- Use o comando git push -u origin main para enviar as alterações para o repositório remoto (substitua main pela sua branch principal, se for diferente). 

```

<br>

**EXEMPLO COMPLETO:**

```
-- Se você já tem um repositório remoto (por exemplo, no GitHub), copie a URL do repositório. 
-- Execute o comando git remote add origin URL_DO_REPOSITORIO_REMOTO para adicionar a origem remota. 
-- Ex: git remote add origin git@github.com:usuario/meu-projeto.git. 

```


* Crie uma pasta para o seu projeto.
* Abra o terminal e navegue até essa pasta.
* Execute git init.
* Crie alguns arquivos no seu projeto (ex: index.html, app.js).
* Execute git add . para adicionar todos os arquivos.
* Execute git commit -m "Adicionando arquivos iniciais" para criar o primeiro commit.
* Se você já tem um repositório no GitHub, copie a URL.
* Execute git remote add origin URL_DO_REPOSITORIO_REMOTO.
* Execute git push -u origin main para enviar as alterações para o GitHub.

<br>

**COMANDOS UTÉIS:**

```
`mkdir` <NOME DO REPOSITORIO>   { CRIA UM LOCAL }
`C:`    <NOME DO REPOSITORIO>   { ENTRA DENTRO DO REPOSITÓRIO }
`git init` | INICIALIZA UM NOVO REPOSITÓRIO GIT NO DIRETÓRIO ATUAL |
`git config --global user.name` { CADASTRA UM USUÁRIO |
`git config --global user.email`{ CADASTRA  UM E-MAIL |
`git status` { Verifica o estado atual do repositório }
`git log`    { Mostra o histórico de commits }
`git clone`  { URL_DO_REPOSITORIO: Cria uma cópia local de um repositório remoto existente }
`git pull`   { Baixa as alterações do repositório remoto } 


```

<br>

## ⌨ HISTÓRICO E RASTREAMENTO

O comando **git log** exibe o histórico de commits de um repositório **Git**. Ele mostra informações como o autor, data, mensagem e identificador único (hash) de cada commit. Isso permite rastrear as alterações feitas no projeto ao longo do tempo, facilitando a identificação de quando e por quem determinadas mudanças foram introduzidas. 

**O que o git log faz:**

```
-- Exibe o histórico de commits: Mostra uma lista de todos os commits, do mais recente para o mais antigo. 
-- Fornece detalhes sobre cada commit: Inclui o autor, data e hora, mensagem de commit e o hash único que identifica o commit. 
-- Permite filtragem e formatação: Existem diversas opções para filtrar o histórico por autor, data, mensagem, etc., e para formatar a saída de acordo com as necessidades do usuário.

```

**COMANDOS UTÉIS:**

```
`git log` { Exibe o histórico completo de commits da branch atual } 
`git log --oneline` { Exibe uma versão mais resumida do histórico, mostrando apenas o hash abreviado e a primeira linha da mensagem de cada commit } 
`git log --author="Nome do Autor"` {Exibe apenas os commits feitos por um autor específico } 
`git log --after="2024-01-01"` --before="2024-01-31" { Exibe os commits feitos entre duas datas específicas } 
`git log --oneline -- graph --decorate --all` { Mostra o histórico de commits em um gráfico visual compacto } 
`git diff HEAD^ HEAD` { Mostra as mudanças introduzidas pelo último commit }
`git blame <arquivo> -L 10,20` { Mostra quem alterou as linhas de 10 a 20 em um arquivo }

```

## ⌨ TRABALHANDO COM BRANCHS:

**Branch** (ou ramificação) é uma linha de desenvolvimento independente dentro de um repositório. Imagine-o como um "ramo" da árvore do seu projeto, onde você pode fazer alterações e experimentar coisas novas sem afetar o código principal (o "tronco" da árvore). 

Em resumo, os branches são uma ferramenta essencial para o desenvolvimento colaborativo e organizado no Git, permitindo que você trabalhe em diferentes partes do seu projeto de forma isolada e segura, com a possibilidade de mesclar as alterações quando estiverem prontas. 

<br>

**COMANDOS UTÉIS:**

```
`git branch` { Lista todos os branches do repositório } 
`git branch <nome_do_branch>`   { Cria um novo branch com o nome especificado }
`git checkout <nome_do_branch>` { Alterna para o branch especificado } 
`git merge <nome_do_branch>`    { Mescla as alterações de um branch em outro. 
`git branch -d <nome_do_branch>`{ Exclui um branch local (apenas se não houver alterações não mescladas } 
`git branch -D <nome_do_branch>`{ Exclui um branch local à força "mesmo que haja alterações não mescladas" } 
`git branch -a` { Lista rodas as branchs, incluindo as remotas }   
`git checkout -b feature/nova-feature`    { Cria e muda para uma nova branch para a sua feature }
`git push -u origin feature/nova-feature` { Envia a noba branch para o remoto e configura o rastreamento upstream } 
`git branch -d feature/velha-feature`     { Deleta uma branch local após a fusão } 

```


