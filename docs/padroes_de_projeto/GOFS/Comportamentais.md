## Histórico de Versão<br>
|Data | Versão | Descrição | Autor(es)|
| :-:|:-:|:-:|:-: |
| 18.03.2022| 0.1 | Criação do Iterator | [Lucas Ferraz](https://github.com/mibasFerraz)|
| 21.03.2022| 0.2 | Revisão do Iterator | [Nilvan Peres](https://github.com/NilvanPeres)|


## 1. Iterator

&emsp;&emsp;A ideia principal o iterator é permitir percorrer os elementos de uma coleção sem expor sua representação subjacente (lista, pilha, árvore etc.). A ideia principal do padrão é extrair o comportamento de passagem de uma coleção para um objeto separado denominado iterador.

&emsp;&emsp;Além de implementar o algoritmo em si, um objeto iterador encapsula todos os detalhes do percurso, como a posição atual e quantos elementos faltam para o final. Por causa disso, vários iteradores podem passar pela mesma coleção ao mesmo tempo, independentemente uns dos outros. Todos os iteradores devem implementar a mesma interface. Isso torna o código do cliente compatível com qualquer tipo de coleção ou qualquer algoritmo de passagem, desde que haja um iterador adequado. Se você precisa de uma maneira especial de percorrer uma coleção, basta criar uma nova classe iteradora, sem ter que alterar a coleção ou o cliente.

&emsp;&emsp;Segundo o RefactoringGuru, o iterator deve ser aplicado quando:

- Quando você deseja que o código realiza iterações sobre diferentes estrutura de dados, ou quando os tipos dessas estruturas ainda não são conhecidos.
- O  padrão permite a redução de duplicatas desnecessárias de códigos.
- Use o padrão Iterator quando sua coleção tiver uma estrutura de dados complexa de árvores, mas você quer esconder sua complexidade dos clientes (seja por conveniência ou por razões de segurança). 

&emsp;&emsp; Os principais participantes dessa padrão em JS são:

- <b>Client</b> : referencia e invoca o iterator para ser utilizado na coleção de objetos.
- <b>Iterator</b>: implementa a interface da iteração, com os métodos first(), next().
- <b>Items</b>: Objetos individuais de uma coleção que está sendo iterada.

&emsp;&emsp;Como o Front-end da nossa aplicação é feita no framework React.JS, estamos utilizando uma abstração do padrão iterator. A linguagem JavaScript utiliza abstrações do padrão por meio de loops. Porém, pode ser considerada uma aplicação exagerada caso o sistema em questão trabalhe apenas com coleções simples e de baixa complexidade.

<p align="justify">&emsp;&emsp;
Na figura 2 abaixo, será representada a utilização desse padrão em código que pode ser encontrada no repositório do <a href='https://github.com/UnBArqDsw2021-2/2021.2_g2_kilimpinho_frontend/blob/develop/src/components/SideMenu/MenuItem.tsx'>frontend</a>.
</p>
<p style="text-align: center">
<img src='https://i.ibb.co/g7xS1mf/Screenshot-from-2022-03-21-08-35-02.png' width='80%'>
  <figcaption align='center'>
      <b>
          <a href='https://i.ibb.co/g7xS1mf/Screenshot-from-2022-03-21-08-35-02.png'>
                Figura 2: Aplicação do iterator no projeto
          </a>
      </b>
  </figcaption>
</p>



## Referências

> - [1] Iterator - DOFactory;. Disponível em : <https://www.dofactory.com/javascript/design-patterns/iterator>.  Último acesso em 18/03/2022.
> - [2] Desgin Patterns - Iterator. Disponível em : <https://brizeno.wordpress.com/2011/09/15/mao-na-massa-iterator/>. Último acesso em 18/03/2022.
> - [3] Padrões de projeto comportamentais: Disponível em <https://refactoring.guru/pt-br/design-patterns/behavioral-patterns>. Último acesso em 18/03/2022.
> - [4] SHVETS, Alexander. Dive Into Design Patterns. Disponível em <https://refactoring.guru/design-patterns>. Último acesso em 18/03/2022. 