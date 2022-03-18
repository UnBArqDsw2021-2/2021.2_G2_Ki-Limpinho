### Histórico de Versão<br>

| Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 18.03.2022 | 0.1 | Criação do documento | Lucas Lima |

## Bridge
O padrão Bridge é mais um dos vinte e três padrões descritos no livro “Design Patterns: Elements of Reusable Object-Oriented Software“ e é muito utilizado quando se deseja separar abstração de implementação justamente porque lida diretamente com a estrutura com que as interfaces e classes são elaboradas. Essa característica peculiar o elevou a ser considerado como um padrão estrutural e tornou possível sua aplicação em pontes de conexão com Banco de Dados.
Por ser um padrão de projeto estrutural é possível que você divida uma classe grande ou um conjunto de classes intimamente ligadas em duas hierarquias separadas: Abstração e Implementação que podem ser desenvolvidas independentemente umas das outras.
De acordo com o GoF, o padrão Bridge significa desacoplar uma abstração de sua implementação para que as duas possam variar independentemente.

### Abstração
A Abstração nesse modelo nada mais é do que a interface que o cliente usa para interagir com a abstração do mundo real e que é implementada pela Abstração Concreta. Nessa abstração concreta é mantido uma referência a uma interface de um Implementador e é exatamente o que torna possível desacoplar a abstração da implementação porque agora a abstração faz referências a um ou mais métodos da classe implementador. Essa camada não deve fazer nenhum tipo de trabalho por conta própria. Ela deve delegar o trabalho para a camada de implementação.

### Implementação
Camada de que terá a responsabilidade de implementar um comportamento específico de um objeto.


## Bibliografia
> - LARMAN, Craig. Utilizando UML e Padrões: Uma introdução à análise e ao projeto orientados a objetos e ao desenvolvimento iterativo. 3. ed. [S. l.: s. n.], 2004.
> - Source Making. 2019. Design patterns. [ONLINE] Available at: https://sourcemaking.com/design_patterns/. Último acesso em 18/03/2022.
> - Padrões de projeto comportamentais: https://refactoring.guru/pt-br/design-patterns/behavioral-patterns. Último acesso em 18/03/2022.
> - GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. Design Patterns: Elements of Reusable Object-Oriented Software. Estados Unidos: Hardback, 1995. 416 p. Erich Gamma, Richard Helm, Ralph Johnson, John Vlissides.