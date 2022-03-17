| Data       | Versão | Descrição       | Autor(es)                                      |
| ---------- | ------ | --------------- | ---------------------------------------------- |
| 17.03.2022 | 0.1    | Adição do State | [[Caio Martins](https://github.com/linktocaio) |

## State

&emsp;&emsp;No padrão state o comportamento de um objeto é dependente de seu estado, isso é, o comportamento de determinado objeto deve ser alterado em tempo de execução a depender de seu estado. O padrão state coloca cada condição em uma classe separada, assim o estado do objeto pode ser interpretado como um objeto ele próprio, dessa forma, o objeto original pode trocar de estado ao delegar o trabalho ao objeto relacionado.

&emsp;&emsp;Imagine um jogo onde o personagem pode se apresentar de diversas formas: andando, nadando, dirigindo um carro, um avião etc. Os controles para a interação com o jogador devem ser diferentes para cada um desses estados, dessa forma os controles devem possuir comportamentos diferentes para cada estado em que o personagem se encontra.

<p align='center'>
    <img src='../assets/img/gofs/state.png'>
    <figcaption align='center'>
        <b>Figura 1: Estrutura State</b>
        <br>
        <small>Autor: <a href='https://refactoring.guru/pt-br/design-patterns/state'>Refactoring Guru</a>, 2022.</small>
    </figcaption>
</p>

## Referências

> [1] BRIENZO, Marcos. State. Disponível em: <https://brizeno.wordpress.com/category/padroes-de-projeto/state/>. Acesso em 17, mar de 2022.
> [2] Refactoring Guru. State. Disponível em: <https://refactoring.guru/pt-br/design-patterns/state>. Acesso em: 17 de mar de 2022.
