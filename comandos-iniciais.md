# Tutorial de Git - Comandos Iniciais

<<<<<<< HEAD
## Instalando git

```Bash
$ sudo apt-get update
$ sudo apt-get install git
```
=======
Tutorial completo como instalar e usar o git no [link](https://www.atlassian.com/br/git/tutorials/install-git).
>>>>>>> 64aef4e (Adicionando link nos comandos iniciais)

<div style="text-align:justify">
Este é um tutorial de Git que abrange alguns dos comandos básicos para começar a usar o Git em um projeto.
</div>

## Configuração Inicial

<div style="text-align:justify">
Antes de começar, é importante configurar o Git com suas informações pessoais.
</div>

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

<div style="text-align:justify">

Essas configurações serão usadas para identificar os autores dos commits que você criar.

</div>

## Inicializando um Repositório

<div style="text-align:justify">

Para começar a usar o Git em um projeto, é necessário inicializar um repositório.

</div>

```bash
git init
```

<div style="text-align:justify">

Esse comando cria um novo repositório Git no diretório atual.

</div>

## Adicionando Arquivos

<div style="text-align:justify">

Após inicializar um repositório, você pode adicionar arquivos a ele para serem rastreados pelo Git.

</div>

```bash
git add nome_do_arquivo
```

<div style="text-align:justify">

Esse comando adiciona um arquivo específico ao próximo commit. Você também pode usar git add . para adicionar todos os arquivos modificados.

</div>

## Fazendo um Commit

<div style="text-align:justify">

Quando você tiver arquivos prontos para serem registrados no histórico do Git, você pode fazer um commit.

</div>

```bash
git commit -m "Mensagem do commit"
```

<div style="text-align:justify">

Esse comando cria um novo commit com as alterações adicionadas anteriormente. A mensagem do commit deve descrever as alterações realizadas.

</div>

## Verificando o Status

<div style="text-align:justify">

A qualquer momento, você pode verificar o status atual do seu repositório.

</div>

```bash
git status
```

<div style="text-align:justify">

Esse comando mostra o status atual do repositório, incluindo arquivos modificados, arquivos adicionados e branch atual.

</div>

## Visualizando o Histórico de Commits

<div style="text-align:justify">

Você pode visualizar o histórico de commits no repositório.

</div>

```bash
git log
```

<div style="text-align:justify">

Esse comando mostra uma lista de commits no repositório, exibindo informações como autor, data, hora e mensagem do commit.

</div>