# Tutorial de Git - Resolvendo Conflitos de Merge

Este é um tutorial que aborda a resolução de conflitos de merge no Git. Quando você mescla alterações de diferentes branches ou obtém alterações de um repositório remoto, pode ocorrer um conflito se o Git não conseguir combinar automaticamente as alterações. Aqui está um guia passo a passo sobre como resolver esses conflitos.

## Passo 1: Identificar Conflitos

Após executar um comando de merge ou pull que resulte em um conflito, o Git informará quais arquivos possuem conflitos. Você pode identificar os conflitos abrindo os arquivos em um editor de código ou usando comandos como:

```bash
git status
```

Esse comando lista os arquivos com conflitos no output.

## Passo 2: Visualizar os Conflitos

Abra os arquivos com conflitos em um editor de código. Os conflitos são marcados com marcadores especiais no código, que geralmente se parecem com isto:

```plaintext
Código que está sendo mesclado da outra branch
```

A seção entre `<<<<<<< HEAD` e `=======` representa as alterações da branch atual, enquanto a seção entre `=======` e `>>>>>>> other_branch` representa as alterações da outra branch.

## Passo 3: Resolver Conflitos

Edite o arquivo para resolver os conflitos. Existem algumas maneiras de fazer isso:

Manter apenas uma versão das alterações: Você pode remover completamente uma das seções (incluindo os marcadores) e manter apenas as alterações da outra seção.

Combinar as alterações: Se as alterações de ambas as seções forem relevantes e você precisar mantê-las, você pode editar o código para combinar as alterações de maneira adequada. Certifique-se de remover os marcadores `<<<<<<< HEAD`, `=======` e `>>>>>>> other_branch` depois de fazer a combinação.

Usar uma ferramenta de merge: Você também pode usar uma ferramenta de merge visual, como o git mergetool, que permite resolver conflitos de forma mais visual.

## Passo 4: Adicionar as Alterações Resolvidas

Após resolver os conflitos, adicione os arquivos modificados ao próximo commit usando o comando:

```bash
git add nome_do_arquivo
```

Certifique-se de adicionar todos os arquivos com conflitos que foram resolvidos.

## Passo 5: Finalizar o Merge

Após adicionar as alterações resolvidas, você pode finalizar o merge com o comando:

```bash
git commit
```

O Git criará um novo commit com as alterações resolvidas.