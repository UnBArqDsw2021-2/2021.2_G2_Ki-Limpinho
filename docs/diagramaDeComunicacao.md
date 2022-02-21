# <center> Diagrama de Comunicação

### Histórico de versão<br>

| Data       | Versão | Descrição                        | Autor(es)       |
| ---------- | ------ | -------------------------------- | --------------- |
| 17.02.2022 | 0.1    | Criação do documento             | Yuri Alves      |
| 18.02.2022 | 0.2    | Adição da introdução             | Yuri Alves      |
| 20.02.2022 | 0.3    | Adição dos diagramas             | Yuri Alves      |
| 20.02.2022 | 0.4    | Complementação da introdução     | Henrique Amorim |
| 21.02.2022 | 0.5    | Complementação dos diagramas     | Henrique Amorim |
| 21.02.2022 | 0.5.1  | Revisão Documento                | Nilvan Peres    |
| 21.02.2022 | 0.5.1  | Revisão Documento                | Nilvan Peres    |
| 21.02.2022 | 0.5.2  | Revisão e melhoria da introdução | Lucas Melo      |

## Participantes

- Yuri Alves
- Henrique Amorim

<br><br>

## 1-Introdução

<div align="justify"> 
    <p style="text-indent: 2rem;">
        O diagrama de comunicação é um diagrama de estrutura UML que mostra o comportamento que representa a comunicação entra um ou mais participantes, mostrando o fluxo de mensagens entre os objetos em uma interação[1].
    </p>
    <p style="text-indent: 2rem;">
        Os diagramas de comunicação assemelham-se aos diagramas de objetos, nos quais uma linha de vida representa os objetos na interação e as setas representam as mensagens transmitidas entre as linhas de vida. Pontas de setas indicam a direção das mensagens, para frente ou para trás, e números de sequência indicam a ordem na qual as mensagens são transmitidas.
    </p>
    <h3>Representações</h3>
    <strong>Objetos</strong>
    <li>Um objeto é representado por um símbolo que mostra seu nome e sua classe sublinhados, separados por dois-pontos[2]</li>
    <strong>Agentes</strong>
    <li> Normalmente, uma instância de agente ocorre no diagrama de comunicação, como o chamador da interação.
    [2]</li>
     <strong>Links</strong>
    <li> Um link é um relacionamento existente entre objetos, entre os quais pode haver troca de mensagens
    [2]</li>
     <strong>Mensagens</strong>
    <li> Mensagem é uma comunicação entre objetos que contém as informações para o início da atividade em questão.
    [2]</li>

</div>

## 2-Diagramas

<p align='center'>
    <img src='../assets/img/comunicacao/comunicacaoClient.png'>
    <figcaption align='center'>
        <b>Figura 1: Comunicação cliente</b>
        <br>
        <small>Autor: Yuri Alves, 2021.</small>
    </figcaption>
</p>

<p align='center'>
    <img src='../assets/img/comunicacao/comunicacaoManager.png'>
    <figcaption align='center'>
        <b>Figura 2: Comunicação gerente criação lava jato</b>
        <br>
        <small>Autor: Yuri Alves, 2021.</small>
    </figcaption>
</p>

<p align='center'>
    <img src='../assets/img/comunicacao/comunicacaoFinancas.png'>
    <figcaption align='center'>
        <b>Figura 3: Comunicação controle de finanças</b>
        <br>
        <small>Autor: Henrique Amorim, 2022.</small>
    </figcaption>
</p>

<p align='center'>
    <img src='../assets/img/comunicacao/comunicacaoServicos.png'>
    <figcaption align='center'>
        <b>Figura 4: Comunicação controle de serviços</b>
        <br>
        <small>Autor: Henrique Amorim, 2022.</small>
    </figcaption>
</p>

## Referências

> [1] - Rational Software Architect RealTime Edition. Disponível em: <https://www.ibm.com/docs/pt-br/rsar/9.5?topic=diagrams-creating-communication>. Acesso em: 17 fev. 2022. <br> > [2] - Diretriz: Diagrama de Comunicação. Disponível em: <https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/guidelines/communication_diagram_FFFEA1B5.html>. Acesso em: 17 fev. 2022. <br> > [3] - Diagramas de comunicação. Disponível em: <https://www.ibm.com/docs/pt-br/radfws/9.6?topic=SSRTLW_9.6.0/com.ibm.xtools.sequence.doc/topics/ccommndiag.html>. Acesso em: 20 fev. 2022. <br>
