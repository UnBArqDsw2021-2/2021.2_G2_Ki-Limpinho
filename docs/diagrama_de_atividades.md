# <center> Diagrama Causa Efeito

### Histórico de Versão

| Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 11.02.2022 | 0.1 | Criação do documento | Davi Matheus |


## 1. Introdução


<p align="justify">&emsp;&emsp; A Linguagem de modelagem unificada inclui diversos subconjuntos de diagramas, incluindo diagramas de estrutura, de interação e de comportamento. Em que diagramas de atividade, com diagramas de caso de uso e de máquina de estados, são considerados diagramas de comportamento porque descrevem o que é necessário acontecer no sistema sendo modelado, e nessa gama de diagramas dinâmicos, destaca-se o diagrama de Atividades.</p>
<p align="justify">&emsp;&emsp;
E nessa gama de diagramas dinâmicos, destaca-se o diagrama de Atividades , em que eles ajudam a unir as pessoas das áreas de negócios e de desenvolvimento de uma organização para entender o mesmo processo e comportamento.  Ou seja, o foco está nos procedimentos, processos de negócio e fluxo de trabalho de um projeto.</p>


## 2. Metodologia

<p align="justify">&emsp;&emsp;Para a modelagem do diagrama de atividades, é necessário primeiro entender sua composição em que alguns dos componentes mais comuns são:</p> 

- Ações: uma etapa da atividade em que o usuário ou software realiza uma determinada tarefa. No Lucidchart, ações são simbolizadas por retângulos de cantos arredondados.
- Nó de decisão: um ramo condicional no fluxo representado por um diamante. Inclui uma única entrada e duas ou mais saídas.
- Fluxos de controle: outro nome dado aos conectores que mostram o fluxo entre as etapas no diagrama.
- Nó inicial: simboliza o início da atividade. É representado por um círculo preto.
Nó final: representa a etapa final da atividade. É representado por um círculo preto delineado.

<p align="justify">&emsp;&emsp; Com isso dito, se conduziu necessário a modularização da aplicação em diversos contextos para que, desta forma, cada fluxo de atividades pudesse ser melhor descrito e para que cada diagrama pudesse ser analisado de maneira independente, em que os fluxos idealizados foram:</p> 

- Cadastro de usuário
- Pagamento de serviços
- Remarcação /Cancelamento de serviços
- Controle dos dashboards da aplicação
- Fluxo de caixa do gerente


<p align="justify">&emsp;&emsp;Vale ressaltar que cada diagrama foi divido em 3 instâncias, estas são as camadas do usuário; do frontend e do backend. Cada camada representa a instância de determinada ação, isto é, em qual nível comportamental uma determinada ação acontece na aplicação. A camada do usuário descreve todas as atividades desempenhadas ao nível da pessoa que utiliza o Animalesco. No que lhe concerne, a camada do frontend engloba todas as atividades desempenhadas pela solução computacional em contato direto com o usuário. Por fim, a camada do backend representa todas as atividades descritas nas regras de negócio e lógicas de processamento da aplicação.</p> 