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
git push -f origin main
```

## Baixar versão do GitHub (Download)

```sh
git pull -f origin main
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
