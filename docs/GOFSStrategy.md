# <center> GOFS Comportamentais (Strategy)

### Histórico de versão<br>

| Data      | Versão | Descrição                | Autor(es)                                   |
| --------- | ------ | ------------------------ | ------------------------------------------- |
| 15.3.2022 | 0.1    | Criação do documento     | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.2    | Adição da introdução     | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.3    | Adição da aplicabilidade | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.4    | Revisão do documento  | [Peniel Etèmana](https://github.com/zpeniel09) |

### Participantes

-   [Yuri Alves](https://github.com/yuriAlves5)

### Introdução

<p align="justify">&emsp;&emsp;
    Seguindo o conceito de GOFS Comportamentais o padrão de estrategia é fundamental para formação de um projeto bem consolidado e com funcionalidade estendidas e manutenções menos custosas. De acordo com o livro Design Patterns de (Gamma et al.) o padrão de estrategia é utilizado de forma a manter o encapsulamento dos algoritimos alem de mante-los intercambiaveis. 
</p>

### Aplicabilidade

<p align="justify">&emsp;&emsp; 
    Ainda seguindo Gamma a utilização dos padrões de estrategia é sugestivo quando:
    <li> Muitas classes relacionadas se diferenciando somente pelo seu comportamento. Com as estrategias é possivel configurar a classe com um ou mais comportamentos.
    </li>
    <li> Você precisa de diferentes variações de um algoritimos
    </li>
    <li> O algoritimo usa dados que os clientes não devem saber. Com o uso do padrão de estrategia, é possivel evitar de expor a estrutura de dados de certos algoritimos especificos.
    </li>
</p>

### Consequencias

<p align="justify">&emsp;&emsp;
    Os seguintes beneficios são constados nos padrões de estrategia:
    <li> <strong>Alternativa para subclassing.</strong> Com subclassing o algoritmo fica dificil de entender,manter e até mesmo estender.já com a tecnica de encapsulamento do algoritipo em classes estrategias separadas, permite a independencia dos contextos do mesmo, melhorando a comprenção
    </li>
    <li> <strong>Elimina condicionais.</strong> O uso de estrategias de GOFS permite a elimanação de declaraçoes condicionais.
    </li>
    <li> <strong>Escolha de implementações.</strong> Permite diferentes formas de implementção do mesmo comportamento
    </li>
</p>

## Referências

> [1] Serrano, Milene. 2020. Aula GoFs Comportamentais. Acesso em 21/03/2022.
