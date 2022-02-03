# <center> Rich Pictures

## Histórico de revisão
| Data   | Versão | Modificação  | Autor  |
| :- | :- | :- | :- |
| 02/02/2022 | 1.0.0 | Criação e elaboração do documento | Davi Matheus |

## Introdução

O principal intuito desse documento é elucidar o processo e as práticas que devem ser seguidas para a **criação de branches** e de **criação de commits.**


## Políticas de Branch

Para a criação de branches, deve ser seguido as seguintes políticas abaixo.

Exemplos do gitflow das branches:

- A branch **main** concentra uma versão estável do produto, contendo código já testado e versionado, pronto para ser entregue ao usuário final ou cliente. Essa branch parte da branch **development** através de pull requests aprovados no fim de cada release.

  Regras:

  1. Existe apenas uma branch **main**.
  2. **Não** são permitidos commits feitos diretamente na **main**.


- A branch **development** contém a versão mais atualizada do código que está sendo desenvolvido. Essa branch está sempre sincronizada com a **main** e é base para as branches **feature**.

  Regras:

  1. Existe apenas uma branch **development**.
  2. Essa branch está sempre sincronizada com a branch **main**.


- As branches **feature** representam as funcionalidades do sistema a serem desenvolvidas, elas devem ter a branch **development** como sua origem e fim.

  Regras:

  1. Essa branch sempre é criada a partir da branch **development**.
  2. Essa branch sempre é mesclada à branch **development**.

  Regras de nomenclatura:

  `numero_da_issue/feature`

- A branch **release** representa o conjunto de funcionalidades provenientes de um ponto específico da branch **development**. Essa branch contém funcionalidades prontas que, provavelmente, estarão presentes na próxima versão estável do produto. Apenas **bug fixes** são permitidos nessa branch.

  Regras:

  1. Essa branch sempre é criada a partir da branch **development**.
  2. Essa branch sempre é mesclada às branches **development** e **master**.
  3. Essa branch aceita apenas mesclagens de branches do tipo **bugfix**.

  Regras de nomenclatura:

  `release/vNúmero-da-versão`

- As branches do tipo **bugfix** são utilizadas para implementar soluções para bugs, encontrados através de testes realizados em releases específicas, na branch **release**. Isso significa que a branch **bugfix** deve ter a branch **release** como sua origem e fim.

  Regras:

  1. Essa branch sempre é criada a partir da branch **release**.
  2. Essa branch sempre é mesclada na branch **release**.

  Regras de nomenclatura:

  `bugfix/issueID-titulo-da-issue`

Observações: O título da issue utilizado no nome das branches deve ser mantido em português.


 Imagens para ajudar a visualizar o fluxo de trabalho descrito:

  ![](https://miro.medium.com/max/640/0*FTwKYpFGADX-5Y0O)

## Políticas de Commits
Os commits deve seguir a seguinte estrutura: 

- categoria_nome do commit #issueID.

- Exemplo: bugs_Correções_Registro #10
- Exemplo2: add_Documento_de_Arquitetura #43

Categorias:

- _**del**_: Deletando algum arquivo/pasta e afins.
- _**format**_: Formatação no código.
- _**docs**_: Adição/atualização de algum documento.
- _**bugs**_: Correção de algum bug.
- _**feat**_: Adição/atualização de nova funcionalidade.
- _**test**_: Adição/modifição de um teste.
- _**refact**_: Refatoração do código.


## Referências

[Git-flow Applied to a Real Project](https://medium.com/empathyco/git-flow-applied-to-a-real-project-c08037e28f88)

[Writing git commit message](https://365git.tumblr.com/post/3308646748/writing-git-commit-messages)

[Acacia - Políticas de contribuição](https://fga-eps-mds.github.io/2019.2-Acacia/#/policies)