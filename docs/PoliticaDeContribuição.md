# <center> Política de Contribuição

### Histórico de revisão
| Data   | Versão | Modificação  | Autor  |
| :- | :- | :- | :- |
| 02/02/2022 | 1.0.0 | Criação e elaboração do documento | Davi Matheus |
| 04.02.2022 | 1.0.1 | Revisão e correção do documento, primeira entrega | Natanael Filho |
| 04.02.2022 | 1.0.2 | Mudança de política de commit | Nilvan Peres |
| 20.02.2022 | 1.0.3 | Adição de política de issues e de documentos | Nilvan Peres |
| 20.02.2022 | 1.0.4 | Review pull request| Caio Martins |

## 1. Introdução

O principal intuito desse documento é elucidar o processo e as práticas que devem ser seguidas para a **criação de issues**, **criação de branches** e de **criação de commits**, e **padronização dos nomes** dos documentos.

## 2. Políticas para criação de issues

A criação de issues deverá ser feita a partir do seguinte template:

``` 
### Descrição:
Uma descrição detalhada sobre o que será feito.

### Tarefas:

- [ ] Tarefa 1.
- [ ] Tarefa 2.

### Critério de aceitação:
A Issue somente será aceita se o critério de aceitação for válido.
```

O primeiro tópico da Issue é justamente para explicar sucintamente o por quê da criação da issue, já o segundo tópico é para descrever quais serão as tarefas que irão que ser feitas para contemplar a Issue, ela serve para guiar o revisor do PR. O último tópico, é em relação ao que deve travar a issue, ou pode atrapalhar o desenvolvimento da mesma.

As labels da issues também são essenciais para facilitar a filtragem delas, no momento as issues serão nomeadas de acordo as entregas que deverão ser feitas em relação a matéria Arquitetura e Desenhos de Software e as sprints de desenvolvimento, porém as listas de labels que poderão ser utilizadas são:
- feature
- bug
- documentation
- refactor
- tests
  

## 3. Políticas de Branch

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

  `numero_da_issue-feature`

- A branch **release** representa o conjunto de funcionalidades provenientes de um ponto específico da branch **development**. Essa branch contém funcionalidades prontas que, provavelmente, estarão presentes na próxima versão estável do produto. Apenas **bug fixes** são permitidos nessa branch.

  Regras:

  1. Essa branch sempre é criada a partir da branch **development**.
  2. Essa branch sempre é mesclada às branches **development** e **master**.
  3. Essa branch aceita apenas mesclagens de branches do tipo **bugfix**.

  Regras de nomenclatura:

  `release-vNúmeroDaVersão`

- As branches do tipo **bugfix** são utilizadas para implementar soluções para bugs, encontrados através de testes realizados em releases específicas, na branch **release**. Isso significa que a branch **bugfix** deve ter a branch **release** como sua origem e fim.

  Regras:

  1. Essa branch sempre é criada a partir da branch **release**.
  2. Essa branch sempre é mesclada na branch **release**.

  Regras de nomenclatura:

  `bugfix-issueIDTituloDaIssue`

Observações: O título da issue utilizado no nome das branches deve ser mantido em português.


 Imagens para ajudar a visualizar o fluxo de trabalho descrito:

  ![](https://miro.medium.com/max/640/0*FTwKYpFGADX-5Y0O)

## 4. Políticas de Commits
Os commits deve seguir a seguinte estrutura: 

- categoria: nome do commit #issueID.

- Exemplo: bugs:Correções Registro #10
- Exemplo2: add: Documento de Arquitetura #43

Categorias:

- _**del**_: Deletando algum arquivo/pasta e afins.
- _**format**_: Formatação no código.
- _**docs**_: Adição/atualização de algum documento.
- _**bugs**_: Correção de algum bug.
- _**feat**_: Adição/atualização de nova funcionalidade.
- _**test**_: Adição/modifição de um teste.
- _**refactor**_: Refatoração do código.

## 5. Criação de documentos
Os documentos deverão ser criados seguindo o arquivo template.md que pode ser encontrado no repositório, o documento consiste nos seguintes tópicos:

- Introdução: Onde deverá ter uma breve descrição explicando sobre o que é artefato que será desenvolvido.
- Metodologia: Esse tópico é referente para explicar as escolhar e métodos utilizados para desenvolver o artefato.
- Resultado: Quais são os resultados que foram atingidos com a documentação
- Referências: Quais foram as fontes que auxiliaram o desenvolvimento do documento.

Regras de nomenclatura para nomear os documentos: CamelCase
Ex: EspecificacaoSuplementar

## 6. Referências

> [1] [Git-flow Applied to a Real Project](https://medium.com/empathyco/git-flow-applied-to-a-real-project-c08037e28f88)

> [2] [Writing git commit message](https://365git.tumblr.com/post/3308646748/writing-git-commit-messages)

> [3] [Acacia - Políticas de contribuição](https://fga-eps-mds.github.io/2019.2-Acacia/#/policies)