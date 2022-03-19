
|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 16.03.2022 | 0.1.1 | Adição do multiton | [Natanael Filho](https://github.com/fernandes-natanael) |

## Multiton

&emsp;&emsp;O Multiton é um padrão que pouco se difere do Singleton. Basicamente, enquanto no Singleton a instância da classe está delimitada na criação de apenas **um** objeto, o Multiton delimita um número de múltiplos objetos, limitado a uma quantidade especificada, que serão criados,  fornecendo vários objetos para serem usados em caráter global para todo o projeto.

&emsp;&emsp;Como exemplo trago uma classe ProdutoLimpeza, nela queremos instanciar 4 produtos diferentes, sendo eles, cera automotiva, sabão para carro,  limpa vidros e espuma multiúso, a partir de uma estrutura de HashMap, podemos instanciar cada objeto de forma única possuindo valores conhecidos e diferentes. A estrutura se mantêm bem semelhante à utilizada no Singleton.

&emsp;&emsp;A situação atual em que se encontra o projeto não há classe que se beneficiária do uso de Multiton, já que não há limitações de N objetos. Além disso, mesmo usando o exemplo dos produtos de limpeza, a plataforma atualmente não possui  o objetivo de gerenciar produtos de limpezas, por isso não se torna viável. 

## Referências

> [1] **GOFs Criacionais**. Disponível em: <https://unbarqdsw2021-1.github.io/2021.1_G6_Curumim/padroes-de-projeto/gofs-criacionais/#multiton>. Acesso em 16, mar de 2022.