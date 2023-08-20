# Git em Equipe

## Inicializar o repositório

```sh
git init
```

## Clonar pasta do Git

```sh
git clone https://github.com/Usuario/pastaProjeto.git .
```

## Adicionar todos os arquivos no Stage

```sh
git add -A
# ou
git add .
```

## Adicionar um arquivo no Stage

```sh
git add arquivo.php
```

## Criar commit

```sh
git commit -m 'nome do commit'
```

## Ver se tem alguma coisa para fazer commit

```sh
git status
```

## Listar commits

```sh
git log --oneline
```

## Andar na linha do tempo

```sh
git checkout 4eb96e7
```

## Ver a diferença de um arquivo

```sh
git diff arquivo.php
```

## Enviar para GitHub (Upload)

```sh
# subindo apenas uma
git push -f origin main

# subindo todas
git push -f --all
```

## Baixar versão do GitHub (Download)

```sh
# baixando apenas uma
git pull -f origin main

# baixando todas
git pull -f --all
```

# Branchs

## Criar uma nova Branch

```sh
git branch -b nomeBranch
```

## Listar todas as Branchs

```sh
git branch
```

## Trocar Branch

```sh
git checkout nomeBranch
```

## Criação de um branch a partir de outro branch

```sh
git checkout -b feature4 develop
```

# Git Flow (Equipe)

## Iniciar o Git Flow

```sh
git flow init
```

## Adicionar uma nova feature (Função)

```sh
git flow feature start css
```

## Publicar as alterações da feature (Função) na Develop (Desenvolvimento)

```sh
git flow feature publish css
```

## Finalizar, transferir para a Develop (Desenvolvimento) e excluir a feature (Função)

```sh
git flow feature finish css
```

## Criar uma versão de release (Testes)

```sh
git flow release start 1.0
```

## finalizar a versão de release (Testes)

```sh
git flow release finish 1.0
```

## Fazer pequnas correções na versão final

```sh
# Criar
git flow hotfix start 1.1

# Publicar e deixar aberta para a equipe
git flow hotfix pulish 1.1

# Finalizar, excluir e publicar na Develop e Main
git flow hotfix finish 1.1
```

## Ver as tags das versões produzidas pela release (Testes) e hotfix (Correções)

```sh
git tag
```

# Merge

## Merge de uma Branch na outra

```sh
# ir para Branch que ainda não tem as alterações
git checkout main

# copiar as alterações feitas na outra Branch
git merge develop
```

# Resumo

```sh
main
develop
	git flow feature publish css # envia para o github e mantem a branch
	git flow feature finish css # faz o merge apenas na develop
	git flow release finish 1.0 # faz o merge na develop e main e gera uma nova tag
	git flow hotfix finish 1.1 # faz o merge na develop e main e gera uma nova tag
```
