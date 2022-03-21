## Histórico de Versão<br>
|Data | Versão | Descrição | Autor(es)|
| :-:|:-:|:-:|:-: |
| 18.03.2022| 0.1 | Criação do Iterator | [Lucas Ferraz](https://github.com/mibasFerraz)|
| 19.03.2022| 0.2 | Criação do Mediator | [Nilvan Peres](https://github.com/NilvanPeres)|
| 20.03.2022| 0.3 | Revisão do Mediator | [Davi Matheus ](https://github.com/DaviMatheus)|
| 21.03.2022| 0.4 | Revisão do Iterator | [Nilvan Peres](https://github.com/NilvanPeres)|

## Participantes
 [Lucas Ferraz](https://github.com/mibasFerraz)
 [Nilvan Peres](https://github.com/NilvanPeres)


## Iterator

&emsp;&emsp;A ideia principal o iterator é permitir percorrer os elementos de uma coleção sem expor sua representação subjacente (lista, pilha, árvore etc.). A ideia principal do padrão é extrair o comportamento de passagem de uma coleção para um objeto separado denominado iterador.

&emsp;&emsp;Além de implementar o algoritmo em si, um objeto iterador encapsula todos os detalhes do percurso, como a posição atual e quantos elementos faltam para o final. Por causa disso, vários iteradores podem passar pela mesma coleção ao mesmo tempo, independentemente uns dos outros. Todos os iteradores devem implementar a mesma interface. Isso torna o código do cliente compatível com qualquer tipo de coleção ou qualquer algoritmo de passagem, desde que haja um iterador adequado. Se você precisa de uma maneira especial de percorrer uma coleção, basta criar uma nova classe iteradora, sem ter que alterar a coleção ou o cliente.

&emsp;&emsp;Segundo o RefactoringGuru, o iterator deve ser aplicado quando:

- Quando você deseja que o código realiza iterações sobre diferentes estrutura de dados, ou quando os tipos dessas estruturas ainda não são conhecidos.
- O  padrão permite a redução de duplicatas desnecessárias de códigos.
- Use o padrão Iterator quando sua coleção tiver uma estrutura de dados complexa de árvores, mas você quer esconder sua complexidade dos clientes (seja por conveniência ou por razões de segurança). 

&emsp;&emsp; Os principais participantes dessa padrão em JS são:

- <b>Client</b> : referencia e invoca o iterator para ser utilizado na coleção de objetos.
- <b>Iterator</b>: implementa a interface da iteração, com os métodos first(), next().
- <b>Items</b>: Objetos individuais de uma coleção que está sendo iterada.

&emsp;&emsp;Como o Front-end da nossa aplicação é feita no framework React.JS, estamos utilizando uma abstração do padrão iterator. A linguagem JavaScript utiliza abstrações do padrão por meio de loops. Porém, pode ser considerada uma aplicação exagerada caso o sistema em questão trabalhe apenas com coleções simples e de baixa complexidade.

<p align="justify">&emsp;&emsp;
Na figura 2 abaixo, será representada a utilização desse padrão em código que pode ser encontrada no repositório do <a href='https://github.com/UnBArqDsw2021-2/2021.2_g2_kilimpinho_frontend/blob/develop/src/components/SideMenu/MenuItem.tsx'>frontend</a>.
</p>
<p style="text-align: center">
<img src='https://i.ibb.co/g7xS1mf/Screenshot-from-2022-03-21-08-35-02.png' width='80%'>
  <figcaption align='center'>
      <b>
          <a href='https://i.ibb.co/g7xS1mf/Screenshot-from-2022-03-21-08-35-02.png'>
                Figura 2: Aplicação do iterator no projeto
          </a>
      </b>
  </figcaption>
</p>


## Mediator

<p align="justify">&emsp;&emsp;
    O padrão mediator permite que um objeto encapsule como será a interação com outros objetos, o mediator permite que o desacoplamento evitando que os objetos fiquem referenciando entre si. [1]
</p>
<p align="justify">&emsp;&emsp;
    O mediator deve ser aplicado quando:
        <li> Um grupo de objetos que se comunicam de forma definida, porém complexa. Resultando em interdependências não estruturadas e complexas de serem entendidas.</li>
        <li> A reutilização de um objeto se torna complexa, pois o mesmo está se comunicando ou se referindo a vários outros objetos.</li>
        <li> Um comportamento que é distruibuído entre várias classes e que deveria ser customizável.[2]</li> 
</p>
<p align="justify">&emsp;&emsp;
    <li><b>Vantagens:</b> </li>
        <ol>
            <li>Limita o uso de subclasses.</li>
            <li>Permite o desacoplamento das classes colegas.</li>
            <li>Simplifica os protocolos dos objetos. O mediador permite substituir a intereção de muitos para muitos, para uma interação de um (mediator) para muitos (colleagues).</li>
            <li>Abstração de como os objetos se relacionam. [2]</li>
        </ol>
    <li><b>Desvantagens:</b> </li>
        <ol>
            <li>Centralização do controle. O mediator permite que a troca de complexidade de interação para uma complexidade no próprio mediator. Como um mediador encapsula protocolos, ele pode se tornar mais complexo que qualquer colega individual. Isso pode tornar o mediador monolítico e complexo de manter.</li>
        </ol>
</p>
<p align="justify">&emsp;&emsp;
    Os principais participantes desse padrão são <b>Mediator(interface para comunicação com objetos colegas)</b>, <b>ConcreteMediator( implemena os comportamentos cooperativos a partir da coordenação dos objetos colegas), </b><b>Products(a instância do produto criado pela factory)</b>, <b> ColeagueClasses (se comunica com seu mediator quando necessário, caso contrário se comunica com outro colega)</b>. No código abaixo, será introduzindo um exemplo de prático de como aplicar esse padrão em JavaScript.
</p>

```
var Participant = function (name) {
    this.name = name;
    this.chatroom = null;
};

Participant.prototype = {
    send: function (message, to) {
        this.chatroom.send(message, this, to);
    },
    receive: function (message, from) {
        console.log(from.name + " to " + this.name + ": " + message);
    }
};

var Chatroom = function () {
    var participants = {};

    return {

        register: function (participant) {
            participants[participant.name] = participant;
            participant.chatroom = this;
        },

        send: function (message, from, to) {
            if (to) {                      // single message
                to.receive(message, from);
            } else {                       // broadcast message
                for (key in participants) {
                    if (participants[key] !== from) {
                        participants[key].receive(message, from);
                    }
                }
            }
        }
    };
};
```
Fonte: <a href="https://www.dofactory.com/javascript/design-patterns/mediator">DoFactory</a>[3]


## Referências

> [1] SERRANO, Milene. Módulo Padrões de Projeto GoF(s) Comportamentais. Disponível em : <https://aprender3.unb.br/course/view.php?id=11018&section=4>. Acesso em 16, mar de 2022.

> [2] GAMMA, Erich; HELM Richard; JOHNSON, Ralph; and VLISSIDES, John. Design Patterns: Elements of Reusable Object-oriented Software, 1995. Addison-Wesley Longman Publishing Co., Inc.

> [3] Design Patterns - Mediator, DO FACTORY. Disponível em: <https://www.dofactory.com/javascript/design-patterns/mediator>, Acesso em 18, mar de 2022.

> - [4] Iterator - DOFactory;. Disponível em : <https://www.dofactory.com/javascript/design-patterns/iterator>.  Último acesso em 18/03/2022.
> - [5] Desgin Patterns - Iterator. Disponível em : <https://brizeno.wordpress.com/2011/09/15/mao-na-massa-iterator/>. Último acesso em 18/03/2022.
> - [6] Padrões de projeto comportamentais: Disponível em <https://refactoring.guru/pt-br/design-patterns/behavioral-patterns>. Último acesso em 18/03/2022.
> - [7] SHVETS, Alexander. Dive Into Design Patterns. Disponível em <https://refactoring.guru/design-patterns>. Último acesso em 18/03/2022. 
