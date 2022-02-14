# <center> Diagrama de Implementação

### Histórico de Versão

|    Data    | Versão |      Descrição       |     Autor(es)     |
| :--------: | :----: | :------------------: | :---------------: |
| 12/02/2022 |  0.1   | Criação do documento | Henrique Amorim |
| 13/02/2022 |  0.2  | Criação do documento | Natanael Filho |
| 13/02/2022 |  0.2  | Revisão do documento | Davi Matheus |

### Participantes

- Henrique Amorim
- Natanael Filho

## 1. Introdução


<div align="justify" style="margin-bottom: 20px"> 

Na UML, diagramas de implementação fazem a modelagem da arquitetura física de um sistema, logo é necessário analisar e encontrar componentes de software e hardware, e como ocorrem o relacionamento entre eles.[2]
</div>
<div align="justify"> 
Além disso, o desenvolvimento de um diagrama de implementação agrega em uma melhor noção da organização física dos nós em sistema distribuído, os artefatos armazenados em cada nó, os componentes e outros elementos que os artefatos implementam.[2]
</div>

### 1.1. Componentes 

#### 1.1.1. Nós

<div align="justify"> 
São modelos que representam recursos computacionais de um sistema, como, por exemplo, computadores pessoais, sensores, dispositivos de impressão ou servidores.[3]
</div>

#### 1.1.2. Esteriótipos

<div align="justify"> 
Esteriótipos servem para facilitar o intendimento do que se trata aquele nó. Além disso, é escrito entre <code><<>></code>.[3]
</div>

#### 1.1.3. Artefatos

<div align="justify"> 
São modelos representativos que buscam representar unidades físicas de execução, como, por exemplo, arquivos executáveis, bibliotecas, componentes de software.[3]
</div>

#### 1.1.4. Associação de comunicação

<div align="justify"> 
Associação entre nós são representadas por linhas sólidas, acompanhadas do protocolo de comunicação entre eles, chamadas conexões. As conexões representam os mecanismos de comunicação entre os nós, podendo ser meios físicos (cabo coaxial, fibras óticas e outros) ou protocolos de comunicação (TCP/IP, HTTP, HTTPS, e outros).[3]
</div>

## 2. Metodologia

<div align="justify"> 
Com este diagrama buscamos uma visualização, especificação e documentação eficaz de como o sistema se comporta em um relacionamento cliente/servidor, os quais normalmente distinguem entre a interface com o usuário e os dados persistentes de um sistema.[1]
</div>

## 3. Resultados

### 3.1. Diagrama versão 1

<p align='center'>
    <div style="width: 640px; height: 480px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:480px" src="https://lucid.app/documents/embeddedchart/ac04bd32-b224-4b50-8c55-8044675a3d90" id="I9dT2KsZNWzZ"></iframe></div>
    <figcaption align='center'>
        <b>Figura 1: Diagrama de implementação, primeira versão</b>
        <br>
        <small>Autor: Henrique Amorim, 2021.</small>
    </figcaption>
</p>

### 3.2. Diagrama versão 2

<p align='center'>
    <div style="width: 640px; height: 480px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:480px" src="https://lucid.app/documents/embeddedchart/cfe944f0-b4ac-4c6d-ab59-33ff0f492510" id="z_dTBxegRyMB"></iframe></div>
    <figcaption align='center'>
        <b>Figura 1: Diagrama de implementação, segunda versão</b>
        <br>
        <small>Autor: Natanael Filho, 2022.</small>
    </figcaption>
</p>


## 4. Bibliografia

> [1] O que é um diagrama de implementação? **Lucidchat**. Disponível em: [https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-implementacao-uml) (último acesso em 12/02/2022)

> [2] Diagramas de Implementação. **IMB**. Disponível em: [https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams](https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=topologies-deployment-diagrams) (último acesso em 12/02/2022)

> [3] Entendendo o Diagrama de Implantação | #12. **Estudo na Web**. Disponível em : [https://www.youtube.com/watch?v=P0wXFFsdMzI](https://www.youtube.com/watch?v=P0wXFFsdMzI) (último acesso em 13/02/2022)
