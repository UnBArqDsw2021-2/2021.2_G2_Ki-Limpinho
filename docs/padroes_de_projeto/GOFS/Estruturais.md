### Histórico de Versão<br>

| Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 18.03.2022 | 0.1 | Criação do documento | [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 | 0.2 | Revisado | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.03.2022 | 0.3 | Adição do Flyweight | [Davi Matheus ](https://github.com/DaviMatheus) |

## Bridge
<p align="justify">&emsp;&emsp;
O padrão Bridge é mais um dos vinte e três padrões descritos no livro “Design Patterns: Elements of Reusable Object-Oriented Software“ e é muito utilizado quando se deseja separar abstração de implementação justamente porque lida diretamente com a estrutura com que as interfaces e classes são elaboradas. Essa característica peculiar o elevou a ser considerado como um padrão estrutural e tornou possível sua aplicação em pontes de conexão com Banco de Dados.
Por ser um padrão de projeto estrutural é possível que você divida uma classe grande ou um conjunto de classes intimamente ligadas em duas hierarquias separadas: Abstração e Implementação que podem ser desenvolvidas independentemente umas das outras.
De acordo com o GoF, o padrão Bridge significa desacoplar uma abstração de sua implementação para que as duas possam variar independentemente.
</p>

### Abstração
<p align="justify">&emsp;&emsp;
A Abstração nesse modelo nada mais é do que a interface que o cliente usa para interagir com a abstração do mundo real e que é implementada pela Abstração Concreta. Nessa abstração concreta é mantido uma referência a uma interface de um Implementador e é exatamente o que torna possível desacoplar a abstração da implementação porque agora a abstração faz referências a um ou mais métodos da classe implementador. Essa camada não deve fazer nenhum tipo de trabalho por conta própria. Ela deve delegar o trabalho para a camada de implementação.
</p>

### Implementação
<p align="justify">&emsp;&emsp;
Camada de que terá a responsabilidade de implementar um comportamento específico de um objeto.
</p>

## Flyweight
<p align="justify">&emsp;&emsp;
O Flyweight é um padrão de projeto estrutural que permite a você colocar mais objetos na quantidade de RAM disponível, compartilhando com uma grande eficiência quantidades de objetos, em que esse  padrão compartilhar partes comuns de estado entre os múltiplos objetos ao invés de manter todos os dados em cada objeto.
</p>

<p align='center'>
    <img src='..\..\..\assets\img\gofs\flyweight.jpeg'>
    <figcaption align='center'>
        <b>
            <a href='..\..\..\assets\img\grasp\proxy.jpeg'>
               Figura 2. Diagrama do padrão Flyweight
            </a>
        </b>
        <br>
        <small>Fonte:<a href='https://refactoring.guru/pt-br/design-patterns/flyweight'>Flyweight-Guru</a></small>
    </figcaption>
</p>

<p align="justify">&emsp;&emsp;
Esse padrão não se aplica ao projeto Ki-limpinho, visto que ele é recomendado quando existe uma grande quantidade de objetos, e assim ter problema com alto consumo de memória RAM.
</p>

## Bibliografia
> - LARMAN, Craig. Utilizando UML e Padrões: Uma introdução à análise e ao projeto orientados a objetos e ao desenvolvimento iterativo. 3. ed. [S. l.: s. n.], 2004.
> - Source Making. 2019. Design patterns. [ONLINE] Available at: https://sourcemaking.com/design_patterns/. Último acesso em 18/03/2022.
> - Padrões de projeto comportamentais: https://refactoring.guru/pt-br/design-patterns/behavioral-patterns. Último acesso em 18/03/2022.
> - GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. Design Patterns: Elements of Reusable Object-Oriented Software. Estados Unidos: Hardback, 1995. 416 p. Erich Gamma, Richard Helm, Ralph Johnson, John Vlissides.
> - FlyweightTambém conhecido como: Peso mosca, Cache  Available at:  https://refactoring.guru/pt-br/design-patterns/flyweight. Último acesso em 21/03/2022.