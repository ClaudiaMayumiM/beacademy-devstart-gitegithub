# beacademy-devstart-gitegithub
Repositório criado para armazenar o entregável do projeto Devstart da edtech BeAcademy, referente ao conteúdo de GIT e GitHub.

Abaixo encontram-se algumas informações referentes aos comandos GIT mais popularmente utilizados.

## Estados possíveis:

- Modificado (modified)
- Preparado (staged/index)
- Consolidado (comitted)

## Ajuda

```bash
  git help 
```

## Configuração

Setar usuário

```bash
  git config --global user.name "Seu Nome"
```

Setar e-mail 

```bash
  git config --global user.email "seuemail@..."
```

## Comandos GIT mais utilizados e suas funções

### Repositório local 

Criar novo repositório

```bash
  git init
```

Verificar o estado dos arquivos/diretórios

```bash
  git status
```

Adicionar arquivo/diretório (staged area)

```bash
  git add nome_arquivo.txt

  git add . 
  (adiciona todos os arquivos de uma vez)
```

Comitar arquivo/diretório

```bash
  git commit -m "Mensagem referente ao commit"
```

Remover arquivo/diretório

```bash
  git rm nome_arquivo.txt
```

Exibir histórico

```bash
  git log
```

Desfazer alteração local (staging area) 
- Este comando deve ser utilizado quando o arquivo já foi adicionado na staged area

```bash
  git reset HEAD nome_arquivo.txt
```

### Repositório remoto

Exibir os repositórios remotos

```bash
  git remote
  git remote -v
```

Enviar arquivos/diretórios para o repositório remoto

```bash
  git push 
  (o primeiro push de um repositório deve conter o nome do repositório remoto e a branch)
```

Atualizar repositório local de acordo com o repositório remoto:

- Atualizar os arquivos na branch atual

```bash
  git pull 
```

- Buscar as alterações, mas não aplicá-las na branch atual

```bash
  git fetch
```

Clonar um repositório remoto já existente

```bash
  git clone (endereço ou chave ssh aqui)
```

### Branches

Lista as branches existentes 

```bash
  git branch
```

Criar uma nova branch

```bash
  git branch nome_da_branch
```

Trocar para uma branch existente

```bash
  git checkout nome_da_branch
```

Criar uma nova branch e trocar

```bash
  git checkout -b nome_da_branch
```

Excluir uma branch 

```bash
  git branch -d nome_da_branch 
```

Realizar o merge entre branches
- Necessário estar na branch que deverá receber as alterações

```bash
  git merge nome_da_branch 
```

### Stash 

- O stash é uma espécie de branch temporária, 
  na qual é possível acumular as alterações em um outro diretório de trabalho

Criar um stash 

```bash
  git stash 
```

Listar stashes 

```bash
  git stash list 
```

Remover o stash mais recente 

```bash
  git stash pop 
```

Remover um stash específico

```bash
  git stash pop stash @{1}
  (o 1 é o índice do stash desejado)
```

Incluir arquivos não trackeados no stash 

```bash
  git stash --include-untracked
```

### Mais alguns comandos 

Reverter um commit 

```bash
  git revert <hash> 
```

Mostrar as diferenças entre arquivos

```bash
  git diff 
```


## Autor

- [@ClaudiaMayumiM](https://github.com/ClaudiaMayumiM)
