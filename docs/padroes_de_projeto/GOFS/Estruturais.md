# <center> Estruturais

## Histórico de Versão<br>

| Data | Versão | Descrição | Autor(es)|
| :--: | :--: | :--: | :--: |
| 15.3.2022 | 0.2    | Criação do Composite | [Yuri Alves](https://github.com/yuriAlves5) |
| 15.3.2022 | 0.3    | Adição da introdução no Composite | [Yuri Alves](https://github.com/yuriAlves5) |
| 17.03.2022 | 0.4 | Adição do Facade | [Caio Martins](https://github.com/linktocaio) |
| 17.03.2022 | 0.5    | Adição do Facade | [Caio Martins](https://github.com/linktocaio) |
| 18.03.2022 | 0.6 | Adição do Bridge | [Lucas Lima](https://github.com/mibasFerraz) |
| 18.03.2022 | 0.7 | Adição do Proxy | [Davi Matheus](https://github.com/DaviMatheus) |
| 21.03.2022 | 0.8 | Revisão do Bridge | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.03.2022 | 0.9 | Adição do Flyweight | [Davi Matheus](https://github.com/DaviMatheus) |
| 21.3.2022 | 0.10  | Adição do diagrama no Composite | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.11    | Adição da implementação no Composite| [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.12   | Revisão do Composite | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |
| 21.03.2022 | 0.13    | Revisão do Facade | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |
| 21.03.2022 | 0.14    | Revisão do documento | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |
| 21.03.2022 | 0.15    | Revisão do documento |[Davi Matheus](https://github.com/DaviMatheus)  |

## Participantes

* [Davi Matheus](https://github.com/DaviMatheus)
* [Yuri Alves](https://github.com/yuriAlves5)
* [Caio Martins](https://github.com/linktocaio)

## Resultados

### Composite

#### Introdução

<p align="justify">&emsp;&emsp;
    O <i>composite</i> é um padrão de desing estrutural que permite o reúso de um mesmo objeto. O composite reúne os objetos em formato de estrutura de árvore.de acordo com Erich Gamma em <i>Design Patterns</i>, essa forma de estruturação é possível tratar objetos individuais e objetos compostos de forma uniforme. Toda essa estrutura é baseada no Polimorfismo dos objetos.
</p>

#### Metodologia


<p align="Estrutura">&emsp;&emsp; 
    Uma típica estrutura da forma <i>composite</i> deve seguir em princípios a seguinte forma.
    <p align='center'>
    <img src='..\..\..\assets\img\gof\compositeDiagrama.jpeg'>    <figcaption align='center'>
        <b>Figura 2: Exemplo de árvore</b>
        <br>
            <small>Autor: <a href='https://github.com/yuriAlves5'>Yuri Alves</a>, 2022.</small>
    </figcaption>
    </p>
    <li>
    Onde o "aComposite" define o comportamento das filhas, salvando o seus componentes e implementando um relação de operação "<i>child-related</i>" entre elas.
    </li>
    <li>
    Já o "aFolha" define a folha da estrutura em forma de árvores onde ela não poderá ter filhos e com um comportamento de objetos primitivos.
    </li>
</p>

#### Implementação

<p align="justify">&emsp;&emsp;
    Ainda de acordo com Erich Gamma em <i>Design Patterns</i>, a implementação do <i>composite</i> cria inúmeras questões a serem consideradas podendo citar:
    <ol>
        <li>
            <strong>referencial parental explicitado.</strong> Mantendo as referencias dos componentes filhos de seus parentes pode simplificar o controle da estrutura <i>composite</i>. Uma forma usual de definir a referencial parental é dentro do componente da classe.
        </li>
        <li>
            <strong>Compartilhamento de componentes.</strong> Ainda seguindo Erich Gamma em <i>Design Patterns</i> o compartilhamento de componentes se mostra bem benéfico para redução de requerimentos de espaço, mas quando um componente não pode ter mais um de um parente, esse compartilhamento se torna bem complicado. Uma possível solução é dos filhos poderem guardar múltiplos parentes e acessar os mesmos.
        </li>
         <li>
            <strong>Ordenamento de filhos</strong> Diversos designs especificam a ordem dos filhos no <i>composite</i> onde deve ser ordenando de forma a refletir o programa mas com cuidados para manter o controle da sequencia dos filhos.
        </li>
        <li>
            <strong>Melhor estrutura de dados para salvar componentes</strong> Pode se utilizar de uma variedade de estruturas de dados para salvar os componentes, como uma lista, árvore, pilha, etc.A escolha vai depender da eficiência e da necessidade de armazenamento dos dados.
        </li>
    </ol>
</p>


### Proxy


<p align="justify">&emsp;&emsp;
O  padrão Estrutural  Proxy  permite a encapsulação de um objeto através de um outro caso ele possui a mesma interface, de forma que o segundo objeto, conhecido como “Proxy”, controla o acesso ao primeiro, que é o objeto real,assim sendo, o proxy é algo que fica no meio do caminho entre a chamada do objeto e o próprio objeto.
</p>

<p align='center'>
    <img src='..\..\..\assets\img\grasp\proxy.jpeg'>
    <figcaption align='center'>
        <b>
            <a href='..\..\..\assets\img\grasp\proxy.jpeg'>
               Figura 3. Diagrama do padrão Proxy
            </a>
        </b>
        <br>
        <small>Fonte:<a href='https://www.devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066'>DevMedia Padrão GOF-Proxy</a></small>
    </figcaption>
</p>

<p align="justify">&emsp;&emsp;
    <li><b>Vantagens:</b> </li>
        <ol>
            <li>Permite deixar transparente o local (endereço) do objeto real. O cliente não precisa conhecer se o objeto é remoto ou não, este tipo de proxy é conhecido como Remote Proxy. [1] </li>
            <li>Útil para realizar otimizações, como cache de objetos.</li>
            <li>Pode ser implementado rotinas de logs e controle de acesso (segurança). Este tipo de proxy é conhecido como Virtual Proxy.</li>
</p>

<p align="justify">&emsp;&emsp;
Na aplicação do Ki-limpinho usamos a variação de Proxy de Proteção, que como já foi dito, é responsável pelo processo de autenticação, como podemos observar na imagem do código abaixo.
</p>

<p align='center'>
    <img src='..\..\..\assets\img\gofs\proxy_code.jpeg'>
    <figcaption align='center'>
        <b>
            <a href='..\..\..\assets\img\gofs\proxy_code.jpeg'>
               Figura 4. Diagrama do padrão Proxy
            </a>
        </b>
        <br>
    </figcaption>
</p>

### Flyweight

<p align="justify">&emsp;&emsp;
O Flyweight é um padrão de projeto estrutural que permite a você colocar mais objetos na quantidade de RAM disponível, compartilhando com uma grande eficiência quantidades de objetos, em que esse  padrão compartilhar partes comuns de estado entre os múltiplos objetos ao invés de manter todos os dados em cada objeto.
</p>

<p align='center'>
    <img src='..\..\..\assets\img\gofs\flyweight.jpeg'>
    <figcaption align='center'>
        <b>
            <a href='..\..\..\assets\img\grasp\proxy.jpeg'>
               Figura 5. Diagrama do padrão Flyweight
            </a>
        </b>
        <br>
        <small>Fonte:<a href='https://refactoring.guru/pt-br/design-patterns/flyweight'>Flyweight-Guru</a></small>
    </figcaption>
</p>

### Bridge

&emsp;&emsp;O padrão Bridge é mais um dos vinte e três padrões descritos no livro “Design Patterns: Elements of Reusable Object-Oriented Software“ e é muito utilizado quando se deseja separar abstração de implementação justamente porque lida diretamente com a estrutura com que as interfaces e classes são elaboradas. Essa característica peculiar o elevou a ser considerado como um padrão estrutural e tornou possível sua aplicação em pontes de conexão com Banco de Dados.
Por ser um padrão de projeto estrutural é possível que você divida uma classe grande ou um conjunto de classes intimamente ligadas em duas hierarquias separadas: Abstração e Implementação que podem ser desenvolvidas independentemente umas das outras.
De acordo com o GoF, o padrão Bridge significa desacoplar uma abstração de sua implementação para que as duas possam variar independentemente.

&emsp;&emsp;A Abstração nesse modelo nada mais é do que a interface que o cliente usa para interagir com a abstração do mundo real e que é implementada pela Abstração Concreta. Nessa abstração concreta é mantido uma referência a uma interface de um Implementador e é exatamente o que torna possível desacoplar a abstração da implementação porque agora a abstração faz referências a um ou mais métodos da classe implementador. Essa camada não deve fazer nenhum tipo de trabalho por conta própria. Ela deve delegar o trabalho para a camada de implementação.

&emsp;&emsp;Camada de que terá a responsabilidade de implementar um comportamento específico de um objeto.


### Facade

&emsp;&emsp;A intenção primeira do padrão facade é a de prover uma interface unificada de nível mais alto para um conjunto de interfaces de um subsistema. Isso é, o facade cria um intermédio entre o usuário e os subsistemas definidos. Assim como uma api, ele torna a interação mais simplificada quebrando o sistema em camadas de abstração, dando um ponto de comunicação para cada um dos subsistemas ao definir operações a serem realizadas por eles. Note que o facade não tira a visibilidade de tais subsistemas, permitindo assim a customização quando desejada.

&emsp;&emsp;Uma boa utilização do facade seria por exemplo em um sistema complexo de sensores, cada um com seu driver e método de comunicação específicos. Com o facade você pode criar uma interface que defina a inicialização dos sistemas, testes de funcionamento, requisição de leituras, desligamento etc.

<p align='center'>
    <img src='..\..\..\assets\img\gofs\facade.png'>
    <figcaption align='center'>
        <b>Figura 6: Estrutura Facade</b>
        <br>
        <small>Autor: <a href='https://refactoring.guru/pt-br/design-patterns/facade'>Refactoring Guru</a>, 2022.</small>
    </figcaption>
</p>

## Conclusão

&emsp;&emsp;Em fim nesse padrao de gofs Estruturais , fizemos uso dos padrões a seguir: Proxy, Facade,
em que para o Proxy usamos a variação de Proteção, que como já foi dito, é responsável pelo processo de autenticação, estes são padrões que lidam com o encapsulamento de objetos, voltados a criar objetos de maneira adequada à situação. Eles ajudam a tornar um sistema mais unificado e conciso  ajudando na organição do nosso projeto.
</p>

## Referências

> [1] Conheça o Pattern Proxy - GoF (Gang of Four) Disponível em : <https://www.devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066>. Acesso em 20, mar de 2022.

> [2] LARMAN, Craig. Utilizando UML e Padrões: Uma introdução à análise e ao projeto orientados a objetos e ao desenvolvimento iterativo. 3. ed. [S. l.: s. n.], 2004.

> [3] Source Making. 2019. Design patterns. [ONLINE] Disponível em: <https://sourcemaking.com/design_patterns/>. Acesso em 18, mar de 2022.

> [4] Padrões de projeto comportamentais. Disponível em: <https://refactoring.guru/pt-br/design-patterns/behavioral-patterns>. Acesso em 18, mar de 2022.

> [5] GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. Design Patterns: Elements of Reusable Object-Oriented Software. Estados Unidos: Hardback, 1995. 416 p. Erich Gamma, Richard Helm, Ralph Johnson, John Vlissides.

> [6] FlyweightTambém conhecido como: Peso mosca, Cache Disponível em:  <https://refactoring.guru/pt-br/design-patterns/flyweight>.  Acesso em 21, mar de 2022.

> [7] Design Patters - Elements of Reusable Object-Oriented Software. Disponível em: <http://www.uml.org.cn/c%2B%2B/pdf/DesignPatterns.pdf>. Acesso em: 15 mar. de 2022.

> [8] BRIENZO, Marcos. Facade. Disponível em: <https://brizeno.wordpress.com/category/padroes-de-projeto/facade/>. Acesso em 17, mar de 2022.

> [9] Refactoring Guru. Facade. Disponível em: <https://refactoring.guru/pt-br/design-patterns/facade>. Acesso em: 17 de mar de 2022.

> [10] WIKIPEDIA CONTRIBUTORS. Command pattern. Disponível em: <https://en.wikipedia.org/wiki/Command_pattern>. Acesso em: 15 mar. 2022.

> [11] AND, A. Learning Python Design Patterns - Second Edition. Disponível em: <https://www.oreilly.com/library/view/learning-python-design/9781785888038/ch07s04.html>. Acesso em: 16 mar. 2022.

> [12] Design Patterns and Refactoring. Disponível em: <https://sourcemaking.com/design_patterns/command>. Acesso em: 16 mar. 2022.

‌