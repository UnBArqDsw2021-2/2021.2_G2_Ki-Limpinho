# <center> Observer

### Histórico de versão<br>

| Data       | Versão | Descrição            | Autor(es)  |
| ---------- | ------ | -------------------- | ---------- |
| 16.03.2022 | 0.1    | Criação do documento | [Peniel Etèmana](https://github.com/zpeniel09) |

### Participantes

- Peniel Etèmana 

### Introdução

<p align="justify">&emsp;&emsp;
GoFs Comportamentais são padrões voltados para alterações no nível do comportamento dos objetos. Auxiliam quando é necessério, por exemplo, usar vários algoritmos diferentes, cada qual mais apropriado para um determinado contexto. 

Permitem, nesse caso, usar mecanismos/recursos para facilitar tanto a incorporação de novos algoritmos para 
novos contextos quanto a seleção de qual algoritmo usar dado um contexto.

Entre os principais GoFs comportamentais temos o Observer, que consiste em definir um mecanismo eficiente para reagir
às alterações realizadas em determinados objetos.

</p>

### Metodologia

<p>
    No pattern observer, é criado uma relação de dependência um-para-muitos entre objetos que funciona da forma seguinte:
    quando um certo objeto, chamado subject tem seu estado modificado, outros objetos, chamados observers, são notificados. 
</p>

<p>
    O Observer é formado por métodos que possuem padrões de nomenclatura e comportamentos específicos. É importante seguir estes padrões para que implementações diferentes do Observer possam ser facilmente identificadas por desenvolvedores que não as codificaram.
</p>

### Resultados

<center>
<img src="../../../assets/img/padroes/observer-padrao.png" class="zoom"> 
<h6>Figura 1: Observer Padrão.</h6>
<h6>Fonte: Padrões de Projetos.</h6>
</center>

<center>
<img src="../../../assets/img/padroes/imagem-observer.png" class="zoom"> 
<h6>Figura 2: Exemplo de imagem sobre Observer.</h6>
<h6>Fonte: Padrões de Projetos.</h6>
</center>

## Referências

> [1] Arquitetura e Desenho de Software AULA - GOFS COMPORTAMENTAIS Profa. Milene Serrano

> [2] Wikipédia. Disponível em: <https://pt.wikipedia.org/wiki/Observer>. Acesso em: 16 mar. 2022.

>‌ [3] Refactoring Guru. **Observer**. Disponível em: <https://refactoring.guru/design-patterns/observer>. Acesso em: 16 mar. 2022.

> [4] Wikipédia. Disponível em: <https://en.wikipedia.org/wiki/Observer_pattern>. Acesso em: 16 mar. 2022.
