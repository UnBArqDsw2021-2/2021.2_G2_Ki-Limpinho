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
    Os principais participantes desse padrão são <b>Mediator(interface para comunicação com objetos colegas)</b>, <b>ConcreteMediator( implemena os comportamentos cooperativos a partir da coordenação dos objetos colegas), </b><b>Products(a instância do produto criado pela factory)</b>, <b> ColeagueClasses (se comunica com seu mediator quando necessário, caso contrário se comunica com outro colega)</b>. Para aplicar esse conceito no projeto, será feito um exemplo-TOY. Lembrando que são necessárias adaptações, pois o projeto está sendo desenvolvido em JavaScript.[3].
</p>

<p align='center'>
  <img src='https://i.ibb.co/yB6r5WL/Screenshot-from-2022-03-19-18-56-55.png'>
  <figcaption align='center'>
        <b>
            <a href='https://i.ibb.co/yB6r5WL/Screenshot-from-2022-03-19-18-56-55.png'>
               Figura 2: Aplicação do padrão Mediator - ToyExample
            </a>
        </b>   
      <br>
        <small>Autor: <a href='https://github.com/NilvanPeres'>Nilvan Peres</a>, 2022.</small>
  </figcaption>
</p>


## Referências

> [1] SERRANO, Milene. Módulo Padrões de Projeto GoF(s) Comportamentais. Disponível em : <https://aprender3.unb.br/course/view.php?id=11018&section=4>. Acesso em 16, mar de 2022.

> [2] GAMMA, Erich; HELM Richard; JOHNSON, Ralph; and VLISSIDES, John. Design Patterns: Elements of Reusable Object-oriented Software, 1995. Addison-Wesley Longman Publishing Co., Inc.

> [3] Design Patterns - Mediator, DO FACTORY. Disponível em: <https://www.dofactory.com/javascript/design-patterns/mediator>, Acesso em 18, mar de 2022.