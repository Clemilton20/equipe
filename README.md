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

## Adicionar uma nova feature

```sh
git flow feature start css
```

## Publicar as alterações da Branch atual na Develop

```sh
git flow feature publish css
```

## Finalizar, transferir para a Develop e excluir a Branch atual

```sh
git flow feature finish css
```
