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

# Git Flow (Equipe)

## Iniciar o Git Flow

```sh
git flow init
```
