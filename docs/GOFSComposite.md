# <center> GOFS Estruturais (Composite)

### Histórico de versão<br>

| Data      | Versão | Descrição               | Autor(es)                                   |
| --------- | ------ | ----------------------- | ------------------------------------------- |
| 15.3.2022 | 0.1    | Criação do documento    | [Yuri Alves](https://github.com/yuriAlves5) |
| 15.3.2022 | 0.2    | adição da introdução    | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.3    | Adição do diagrama      | [Yuri Alves](https://github.com/yuriAlves5) |
| 21.3.2022 | 0.3    | Adição da implementação | [Yuri Alves](https://github.com/yuriAlves5) |

### Participantes

-   [Yuri Alves](https://github.com/yuriAlves5)

### Introdução

<p align="justify">&emsp;&emsp;
    O <i>composite</i> é um padrão de desing estrutural que permite o reuso de um mesmo objeto. O composite reune os objetos em formato de estrutura de árvore.de acordo com Erich Gamma em <i>Design Patterns</i>, essa forma de estruturação é possivel tratar objetos individuais e objetos compostos de forma uniforme. Toda essa estrutura é baseada  no Polimorfismo dos objetos. 
</p>

### Metodologia

<p align="Estrutura">&emsp;&emsp; 
    Uma tipica estrutura da forma <i>composite</i> deve seguir em principios a seguinte forma.
    <p align='center'>
    <img src='../assets/img/gof/compositeDiagrama.jpeg'>
    <figcaption align='center'>
        <b>Figura 1: Exemplo de árvore</b>
        <br>
        <small>Autor: Yuri Alves, 2021.</small>
    </figcaption>
    </p>
    <li>
    Onde o "aComposite" define o comportamente das filhas, salvando o seus componentes e implementando um relaao de operação "<i>child-related</i>" entre elas.
    </li>
    <li>
    Já o "aFolha" define a folha da estrutura em forma de arvores onde ela não poderá ter filhos e com um comportamento de objetos primitivos.
    </li>
</p>

### Implementação

<p align="justify">&emsp;&emsp;
    Ainda de acordo com Erich Gamma em <i>Design Patterns</i>, a implementação do <i>composite</i> cria inumeras questões a serem consideradas podendo citar:
    <ol>
        <li>
            <strong>referencial parental explicitado.</strong> Mantendo as referencias dos componentes filhos de seus parentes pode simplificar o controle da estrutura <i>composite</i>. Uma forma usual de definir a referencial parental é dentro do componente da classe.
        </li>
        <li>
            <strong>Compartilhamento de componentes.</strong> Ainda seguindo Erich Gamma em <i>Design Patterns</i> o compartilhamente de componentes se mostra bem benefico para redução de requiquerimentos de espaço, mas quando um componente não pode ter mais um de um parente, esse compartilhamento se torna bem complicado. Uma possivel solução é dos filhos poderem guardar multiplos parentes e acessar os mesmos.
        </li>
         <li>
            <strong>Ordenamento de filhos</strong> Diversos designs especificam a ordem dos filhos no <i>composite</i> onde deve ser ordenando de forma a refletir o programa mas com cuidados para manter o controle da sequencia dos filhos.
        </li>
        <li>
            <strong>Ordenamento de filhos</strong> Diversos designs especificam a ordem dos filhos no <i>composite</i> onde deve ser ordenando de forma a refletir o programa mas com cuidados para manter o controle da sequencia dos filhos.
        </li>
        <li>
            <strong>Melhor estrutura de dados para salvar componentes</strong> Pode se utilziar de uma variedade de estruturas de dados para salvar os componentes, como uma lista, árvore, pilha, etc.A escolha vai depender da eficiencia e da necessidade de armazenamento dos dados.
        </li>
    </ol>
</p>

## Referências

> [1] Design Patters - Elements of Reusable Object-Oriented Software. Disponível em: http://www.uml.org.cn/c%2B%2B/pdf/DesignPatterns.pdf. Acesso em: 15 mar. de 2022.
