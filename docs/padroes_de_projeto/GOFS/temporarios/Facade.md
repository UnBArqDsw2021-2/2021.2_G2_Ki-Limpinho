| Data       | Versão | Descrição        | Autor(es)                                      |
| ---------- | ------ | ---------------- | ---------------------------------------------- |
| 17.03.2022 | 0.1    | Adição do Facade | [[Caio Martins](https://github.com/linktocaio) |

## Facade

&emsp;&emsp;A intenção primeira do padrão facade é a de prover uma interface unificada de nível mais alto para um conjunto de interfaces de um subsistema. Isso é, o facade cria um intermédio entre o usuário e os subsistemas definidos. Assim como uma api, ele torna a interação mais simplificada quebrando o sistema em camadas de abstração, dando um ponto de comunicação para cada um dos subsistemas ao definir operações a serem realizadas por eles. Note que o facade não tira a visibilidade de tais subsistemas, permitindo assim a customização quando desejada.

&emsp;&emsp;Uma boa utilização do facade seria por exemplo em um sistema complexo de sensores, cada um com seu driver e método de comunicação específicos. Com o facade você pode criar uma interface que defina a inicialização dos sistemas, testes de funcionamento, requisição de leituras, desligamento etc.

<p align='center'>
    <img src='../assets/img/gofs/facade.png'>
    <figcaption align='center'>
        <b>Figura 1: Estrutura Facade</b>
        <br>
        <small>Autor: <a href='https://refactoring.guru/pt-br/design-patterns/facade'>Refactoring Guru</a>, 2022.</small>
    </figcaption>
</p>

## Referências

> [1] BRIENZO, Marcos. Facade. Disponível em: <https://brizeno.wordpress.com/category/padroes-de-projeto/facade/>. Acesso em 17, mar de 2022.
> [2] Refactoring Guru. Facade. Disponível em: <https://refactoring.guru/pt-br/design-patterns/facade>. Acesso em: 17 de mar de 2022.
