## Abstract Factory

<p align="justify">&emsp;&emsp;
    Esse padrão permite que uma interface seja responsável pela criação de famílias de objetos que possuem um "tema" em comum, sem a necessidade de especificar a classe concreta. 
</p>
<p align="justify">&emsp;&emsp;
    O abstract factory deve ser aplicado quando:
        <li> Um sistema que deveria ser ser independente em como os produtos são criados, associados e representados.</li>
        <li> Um sistema que deveria ser configurado com múltiplas famílias de produtos.</li>
        <li> Quando é desejado implementar uma classe de produtos, e você deseja que tenham acesso apenas a interface, e não a implementação.[2]</li> 
</p>
<p align="justify">&emsp;&emsp;
    <li><b>Vantagens:</b> </li>
        <ol>
            <li>Há o isolamento das classes concretas. A factory ajuda a encapsular a responsabilidade e o processo de criar ojetos e isola o cliente da classes de implemtações.</li>
            <li>As mudanças nas classes concretas ficam unitárias, tendo que alterar o código em apenas um lugar, caso haja alguma mudança de configuração na classe de fábrica concreta.</li>
            <li>Permite maior consistências dos produtos, permitindo que aplicação use uma família por vez.</li>
        </ol>
    <li><b>Desvantagens:</b> </li>
        <ol>
            <li>A extensão de novos produtos não ocorre de forma fácil, pois é necessário a alteração de diferentes trechos de códigos em múltiplos arquivos, a classe da fábrica abstrata e toda as suas subclasses.</li>
        </ol>
</p>
<p align="justify">&emsp;&emsp;
    Os principais participantes desse padrão são <b>AbstractFactory(interface para criação de produtos)</b>, <b>ConcreteFactory(uma fabrica que "produz" novos produtos), </b><b>Products(a instância do produto criado pela factory)</b>, <b> AbstractProduct (Interface para os produtos que serão criados)</b>. Para aplicar esse conceito no projeto, será feito um exemplo-TOY. Lembrando que são necessárias adaptações, pois o projeto está sendo desenvolvido em JavaScript, dessa forma, não é suportado herança de classes, por isso as classes concretas receberão mesmos métodos e propriedades para garantir que tenham as mesmas definições [3].
</p>

<p align='center'>
  <img src='https://i.ibb.co/ryNmjxr/Screenshot-from-2022-03-19-12-26-02.png'>
  <figcaption align='center'>
        <b>
            <a href='https://i.ibb.co/ryNmjxr/Screenshot-from-2022-03-19-12-26-02.png'>
               Figura 2: Aplicação do padrão AbstractFactory - ToyExample
            </a>
        </b>   
      <br>
        <small>Autor: <a href='https://github.com/NilvanPeres'>Nilvan Peres</a>, 2022.</small>
  </figcaption>
</p>


## Referências

> [1] SERRANO, Milene. Módulo Padrões de Projeto GoF(s) Criacionais. Disponível em : <https://aprender3.unb.br/course/view.php?id=11018&section=4>. Acesso em 16, mar de 2022.

> [2] GAMMA, Erich; HELM Richard; JOHNSON, Ralph; and VLISSIDES, John. Design Patterns: Elements of Reusable Object-oriented Software, 1995. Addison-Wesley Longman Publishing Co., Inc.

> [3] Design Patterns - Abstract Factory, DO FACTORY. Disponível em: <https://www.dofactory.com/javascript/design-patterns/abstract-factory>, Acesso em 18, mar de 2022.