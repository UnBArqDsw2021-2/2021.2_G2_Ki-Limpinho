## Histórico de versão<br>

| Data       | Versão | Descrição            | Autor(es)  |
| ---------- | ------ | -------------------- | ---------- |
| 16.03.2022 | 0.1    | Adição Prototype | [Peniel Etèmana](https://github.com/zpeniel09) |
| 20.03.2022 | 0.2    | Revisão Prototype | [Nilvan Peres](https://github.com/NilvanPeres) |

## Participantes

- [Peniel Etèmana](https://github.com/zpeniel09)

## Prototype

<p align="justify">&emsp;&emsp;
GoFs Criacionais são padrões que fornecem vários mecanismos de criação de objetos, que aumentam a flexibilidade e a reutilização do código existente. 

Permitem, nesse caso, usar mecanismos/recursos para facilitar tanto a incorporação de novos algoritmos para 
novos contextos quanto a seleção de qual algoritmo usar dado um contexto.

Entre os principais GoFs criacionais temos o Prototype,é um padrão de design criacional que permite copiar objetos existentes sem tornar seu código dependente de suas classes

</p>

<p align="justify">&emsp;&emsp;
O padrão prototype deve ser aplicado quando: 
    <li>Quando  o sistema deve ser independente de como os produtos são criados e representados.</li>
    <li>Quando as classes que serão instanciadas são especificadas no tempo de execucação do código.[2]</li> 
</p>



<p align="justify">&emsp;&emsp;
    O padrão Prototype(protótipo), da forma como foi descrito no livro Design Patterns: Elements of Reusable Object-Oriented Software, contém os seguintes elementos:<br>
</p>

  -  **prototype** — uma classe que declara uma interface para objetos capazes de clonar a si mesmo.
    
  -  **prototype concreto** — implementação de um prototype;
    
  -  **cliente** — cria um novo objeto através de um prototype que é capaz de clonar a si mesmo.


<center>
<img src="../../../assets/img/padroes/prototype-design.png"> 
<h6>Figura 1: Diagrama descrevendo prototype design pattern.</h6>
<h6>Fonte: Wikipédia.</h6>
</center>


<strong>Uso desse padrão no nosso projeto, será represetado na figura 5</strong>
<p align='center'>
  <img src='https://i.ibb.co/pPLVpyj/Screenshot-from-2022-03-20-19-27-16.png'>
  <figcaption align='center'>
        <b>
            <a href='https://i.ibb.co/pPLVpyj/Screenshot-from-2022-03-20-19-27-16.png'>
               Figura 5: Aplicação do padrão Prototype - ToyExample
            </a>
        </b>   
      <br>
        <small>Autor: <a href='https://github.com/NilvanPeres'>Nilvan Peres</a>, 2022.</small>
  </figcaption>
</p>
<p align="justify">&emsp;&emsp;
    Esse padrão pode ser observado no produto, que quando é criado, ele possui uma estrutura com valores pré-definidos, que não sao necessários serem especificados no momento de criação.
    <li><b>Vantagens:</b> </li>
        <ol>
            <li>Adição e remoção de produtos em tempo de exucação, melhorando significamente o desempenho da aplicação.</li>
            <li>Especificando novos objetos a partir de alterações de valores.</li>
            <li>Especificando novos objetos a partir da variação de estruturas.</li>
        </ol>
    <li><b>Desvantagens:</b> </li>
        <ol>
            <li>Cada subclasse do Prototype deverá implementar uma operação de clone, o que é um processo complexo, pois os objetos internos podem não suportar o clone, ou possuir referências circulares.</li>
        </ol>
</p>

<p align="justify">&emsp;&emsp;
    Podemos concluir que, o Prototype faz a criação de novos objetos, mas ao invés de criar objetos com valores não inicializados, ele cria objetos através da cópia dos valores de um protótipo. Esse padrão nos permitirá copiar objetos existentes sem que essa parte do código tenha dependência em classes. Quando quisermos criar um objeto igual, não precisamos acionar essas classes, basta fazer a exata cópia do objeto já criado.
</p>


## Referências

> [1] Arquitetura e Desenho de Software AULA - GOFS CRIACIONAIS Profa. Milene Serrano

> [2] Wikipédia. Disponível em: <https://pt.wikipedia.org/wiki/Prototype>. Acesso em: 16 mar. 2022.

> [3] Refactoring Guru. **Prototype**. Disponível em: <https://refactoring.guru/design-patterns/prototype>. Acesso em: 16 mar. 2022.

> [4] Wikipédia. Disponível em: <https://en.wikipedia.org/wiki/Prototype_pattern>. Acesso em: 16 mar. 2022.
