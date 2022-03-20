## Histórico de Versão<br>

|Data | Versão | Descrição | Autor(es)|
| :-:|:-:|:-:|:-: |
| 17.03.2022 | 0.1 | Criação do GOF Builder | [Jonathan Jorge](https://github.com/Jonathan-Oliveira)|
| 20.03.2022 | 0.2 | Correção Builder | [Nilvan Peres](https://github.com/NilvanPeres)|
| 18.03.2022 | 0.3 | Adição GOF Absract Factory | [Nilvan Peres](https://github.com/NilvanPeres)|

## Participantes

* [Jonathan Jorge](https://github.com/Jonathan-Oliveira)
* [Nilvan Peres](https://github.com/NilvanPeres)

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


## Builder
<p align="justify">&emsp;&emsp;
    O Builder é um padrão de projeto de software  criacional quer permite a construção de objetos passo a passo. Permite a produção e representação de objetos complexos usando o mesmo código de construção, baseado em regras e parâmetros que sejam informados ao objeto responsável pela construção.
</p>
<p align="justify">&emsp;&emsp;
    A estrutura desse padrão pode ser visualizado abaixo, na figura 3:
</p>

<p align='center'>
  <img src='../../../../assets/img/gof/structure_builder.png'>
  <figcaption align='center'>
        <b>
            <a href='../../../../assets/img/gof/structure_builder.png'>
               Figura 3: Estrutura do padrão Builder
            </a>
        </b>   
      <br>
      <small>Fonte: GAMMA et al., 1995 </small>
  </figcaption>
</p>

<p align="justify">&emsp;&emsp;
    Esse padrão deve ser aplicado quando:
    <li>O algoritmo resposável pela criação do objeto é complexo e deve ser independente das partes e da forma que serão montadas.</li>
    <li> O processo de construção deve permitir diferentes representações para os ojetos que foram construídos.[2]</li> 
</p>

<p align="justify">&emsp;&emsp;
    O padrão Builder poderia ser aplicado caso a aplicação tivesse a funcionalidade de baixar os dados do dashboard em diversos formatos, como por exemplo CSV, JSON, XML, etc. Para a aplicação da funcionalidade citada a cima, o padrão seria aplicado com a seguinte estrutura que será representada na figura 4:
</p>

<p align='center'>
  <img src='../../../../assets/img/gof/application_builder.png'>
  <figcaption align='center'>
        <b>
            <a href='../../../../assets/img/gof/application_builder.png'>
               Figura 4: Estrutura da aplicação do padrão Builder
            </a>
        </b>   
      <br>
        <small>Autor: <a href='https://github.com/Jonathan-Oliveira'>Jonathan Jorge</a>, 2022.</small>
  </figcaption>
</p>

<p align="justify">&emsp;&emsp;
    Os participantes dessa estrutura são:
    <ul>
        <li> 
            Builder (ConverterDashboard)
            <ol>
                <li>
                    Especifica uma interface abstrata para criar partes de um objeto de Product. 
                </li>
            </ol>
        </li>
        <li>
            ConcreteBuilder (ConversorJson, ConversorCsv, ConversorXml)
            <ol>
                <li>
                    Constrói e monta partes do produto através da implementação da interface Builder. 
                </li>
                <li>
                    Define e mantém um registo da representação que cria. 
                </li>                
                <li>
                    Fornece uma interface para a recuperação do produto (ex., ObterCsv, ObterJSON, etc.).
                </li>
            </ol>
        </li>
        <li>
            Director (ExportaDashboard)
            <ol>
                <li>
                    Constrói um objeto usando a interface Builder.
                </li>
            </ol>
        </li>
        <li>
            Product ( Arquivo CSV,  Arquivo JSON,  Arquivo XML)
            <ol>
                <li>
                     Representa o objeto complexo em construção. O ConcreteBuilder constrói a representação interna do produto e define o processo pelo qual este é montado.
                </li>
                <li>
                    Inclui classes que definem as partes constituintes, incluindo interfaces para a montagem das peças no resultado final.
                </li>
            </ol>
        </li>
    </ul>
</p>

<p align="justify">&emsp;&emsp;
    De acordo com GAMMA, a aplicação do builder tem as seguintes vantagens:
    <ol>
    <li> Permite variar a representação interna de um produto;</li>
    <li> Isola o código de construção e representação; </li>
    <li>  Proporciona um melhor controle sobre o processo de construção.</li>
    </ol>
</p>

<p align="justify">&emsp;&emsp;
    Dessa forma, podemos concluir que, o padrão Builder facilita na separação de toda a lógica de criação dos objetos, evitando que as classes que representam esses objetos finais fiquem muito extensas e de pouca manutenibilidade, além de prover a implementação de múltiplos builders especializados, onde tem-se objetos construídos em cima de uma interface.
</p>


## Referências

> [1] SERRANO, Milene. Módulo Padrões de Projeto GoF(s) Criacionais. Disponível em : <https://aprender3.unb.br/course/view.php?id=11018&section=4>. Acesso em 16, mar de 2022.

> [2] GAMMA, E. et al. Design Patterns: Elements of Reusable Object-Oriented Software. USA:
Addison-Wesley Longman Publishing Co., Inc., 1995. ISBN 0201633612.

> [3] Design Patterns - Abstract Factory, DO FACTORY. Disponível em: <https://www.dofactory.com/javascript/design-patterns/abstract-factory>, Acesso em 18, mar de 2022.

> [4] Builder Disponível em: <https://refactoring.guru/pt-br/design-patterns/builder>. Acesso em 17, Mar de 2022.

> [5] 007 – Padrão de Projeto BUILDER – Padrão GoF de Criação – Curso de Design Patterns Disponível em: <http://davesbalthazar.com.br/007-padrao-de-projeto-builder-padrao-gof-de-criacao-curso-de-design-patterns/>. Acesso em 17, Mar de 2022.

> [6] Desing Patterns na prática - Desvendando o Builder (parte 2) Disponível em: <http://www.linhadecodigo.com.br/artigo/2576/desing-patterns-na-pratica-desvendando-o-builder-parte-2.aspx>. Acesso em 17, Mar de 2022.

