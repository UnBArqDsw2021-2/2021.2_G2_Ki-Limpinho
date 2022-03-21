| Data       | Versão | Descrição            | Autor(es)  |
| ---------- | ------ | -------------------- | ---------- |
| 16.03.2022 | 0.1    | Adição do observer | [Peniel Etèmana](https://github.com/zpeniel09) |
| 21.03.2022 | 0.1    | Revisão | [Nilvan Peres](https://github.com/NilvanPeres) |

## Participantes

- [Peniel Etèmana](https://github.com/zpeniel09)


&emsp;&emsp;GoFs Comportamentais são padrões voltados para alterações no nível do comportamento dos objetos. Auxiliam quando é necessério, por exemplo, usar vários algoritmos diferentes, cada qual mais apropriado para um determinado contexto. Permitem, nesse caso, usar mecanismos/recursos para facilitar tanto a incorporação de novos algoritmos para 
novos contextos quanto a seleção de qual algoritmo usar dado um contexto.

&emsp;&emsp;Entre os principais GoFs comportamentais temos o Observer, que consiste em definir um mecanismo eficiente para reagir
às alterações realizadas em determinados objetos.

&emsp;&emsp;No pattern observer, é criado uma relação de dependência um-para-muitos entre objetos que funciona da forma seguinte:quando um certo objeto, chamado subject tem seu estado modificado, outros objetos, chamados observers, são notificados. 

&emsp;&emsp;O Observer é formado por métodos que possuem padrões de nomenclatura e comportamentos específicos. É importante seguir estes padrões para que implementações diferentes do Observer possam ser facilmente identificadas por desenvolvedores que não as codificaram.

&emsp;&emsp; Na figura 4 abaixo, será representado como funciona esse padrão no nível de modelagem, e quais são os participantes desse design.
<center>
<img src="../../../assets/img/padroes/observer-padrao.png" class="zoom"> 
<h6>Figura 4: Observer Padrão.</h6>
<h6>Fonte: Padrões de Projetos.</h6>
</center>

<center>
<img src="../../../assets/img/padroes/imagem-observer.png" class="zoom"> 
<h6>Figura 4: Exemplo de imagem sobre Observer.</h6>
<h6>Fonte: Padrões de Projetos.</h6>
</center>

&emsp;&emsp; Abaixo, um exemplo em código de como aplicar esse padrão em Javascript:

```
function Click() {
    this.handlers = [];  // observers
}

Click.prototype = {

    subscribe: function (fn) {
        this.handlers.push(fn);
    },

    unsubscribe: function (fn) {
        this.handlers = this.handlers.filter(
            function (item) {
                if (item !== fn) {
                    return item;
                }
            }
        );
    },

    fire: function (o, thisObj) {
        var scope = thisObj || window;
        this.handlers.forEach(function (item) {
            item.call(scope, o);
        });
    }
}

function run() {

    var clickHandler = function (item) {
        console.log("fired: " + item);
    };

    var click = new Click();

    click.subscribe(clickHandler);
    click.fire('event #1');
    click.unsubscribe(clickHandler);
    click.fire('event #2');
    click.subscribe(clickHandler);
    click.fire('event #3');
}
```
Fonte: [DoFactory](https://www.dofactory.com/javascript/design-patterns/observer)

## Referências

> [14] Arquitetura e Desenho de Software AULA - GOFS COMPORTAMENTAIS Profa. Milene Serrano

> [15] Wikipédia. Disponível em: <https://pt.wikipedia.org/wiki/Observer>. Acesso em: 16 mar. 2022.

> [16] Refactoring Guru. **Observer**. Disponível em: <https://refactoring.guru/design-patterns/observer>. Acesso em: 16 mar. 2022.

> [17] Wikipédia. Disponível em: <https://en.wikipedia.org/wiki/Observer_pattern>. Acesso em: 16 mar. 2022.
