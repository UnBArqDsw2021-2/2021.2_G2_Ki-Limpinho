## Mediator

<p align="justify">&emsp;&emsp;
    O padrão mediator permite que um objeto encapsule como será a interação com outros objetos, o mediator permite que o desacoplamento evitando que os ojetos fiquem refereciando entre si. [1]
</p>
<p align="justify">&emsp;&emsp;
    O mediator deve ser aplicado quando:
        <li> Um grupo de objetos que se comunicam de forma definida, porém complexa. Resultando em interdependências não estruturadas e complexas de serem entedidas.</li>
        <li> A reutilização de um objeto se torna complexa, pois o mesmo está se comunicando ou se referindo a vários outros objetos.</li>
        <li> Um comportamento que é distruibuído entre várias classes e que deveria ser customizável sem o uso de outras subclasses.[2]</li> 
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
            <li>Centralização do controle. O mediator permite que a troca de complexidade de interação para uma complexidade no próprio mediator. Como um mediador encapsula protocolos, ele pode se tornar mais complexo que qualquer colega individual. Isso pode tornar o mediador monolitico e complexo de manter.</li>
        </ol>
</p>
<p align="justify">&emsp;&emsp;
    Os principais participantes desse padrão são <b>Mediator(interface para comunicação com objetos colegas)</b>, <b>ConcreteMediator( implemena os comportamentos cooperativos a partir da coordenação dos objetos colegas), </b><b>Products(a instância do produto criado pela factory)</b>, <b> ColeagueClasses (se comunica com seu mediator quando necessário, caso contrário se comunica com outro colega)</b>. Na Figura2 abaixo será introduzindo um exemplo de prático de como aplicar esse padrão em JavaScript.
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