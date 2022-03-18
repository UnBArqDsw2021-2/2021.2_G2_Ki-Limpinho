# <center> GRASP Criador

### Histórico de versão<br>

| Data       | Versão | Descrição            | Autor(es)                    |
| ---------- | ------ | -------------------- | ---------------------------- |
| 12.03.2022 | 0.1    | Criação do documento | [Lucas Melo](https://github.com/luucas-melo)<br>[Nilvan Peres](https://github.com/NilvanPeres) |

### Participantes

- [Lucas Melo](https://github.com/luucas-melo)
- [Nilvan Peres](https://github.com/NilvanPeres)

### Introdução

<p align="justify">&emsp;&emsp;
    Creator ou Criador é um dos padrões de Projeto GRASP, que assim como os outros tentam atribuir responsabilidades, papéis e colaborações. A criação de desenho de software desse padrão foca em identificar os responsáveis ideais para criação de objetos. Essa atribuição de obrigações de criação de objetos é de extrema importância para a modelagem do domínio, pois permite que a construção do software reduza acomplamentos desnecessários, além de facilitar o encapsulameno e reutilização do software. [2]
</p>

<p align="justify">&emsp;&emsp;
    Determinar isso pode não ser uma tarefa tão simples, por isso é importante analisar bem. Uma forma para determinar o responsável pela criação desses objetos é verificando da seguinte forma, supondo que temos uma classe A e B. A classe A cria a classe B se[1]:
</p>

<li>B contém ou agrega A</li>
<li>B registra a existência de A</li>
<li>B usa A</li>
<li>B tem os dados necessários para a inicialização de A que serão passados ao construtor de A</li>

<div style="width: 480px; height: 360px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:480px; height:360px" src="https://lucid.app/documents/embeddedchart/92a215e1-c772-41b4-b751-9ca7cb76976c" id="9T82cDyCgAB5"></iframe></div>



### Referências

> [1] GRASP: Designing Objetos com Responsabilidades. [s.l: s.n.]. Disponível em: <https://www.ic.unicamp.br/~ariadne/mc436/1s2017/Lar16GRASP.pdf>. Acesso em: 13 mar. 2022.
> [2] SERRANO, Milene. Módulo de padrões de projeto GRASPs. 07a -VídeoAula - GRASP Criador.  Disponível em: <https://aprender3.unb.br/course/view.php?id=11018&section=4>. Acesso em: 15 mar. 2022.

‌
