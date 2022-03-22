# <center> GRASPS

## Histórico de Versão

|    Data    | Versão | Descrição            | Autor(es)       |
| :--------: | :----: | :------------------: | :-------------: |
| 20.03.2022 |  0.1   | Criação do Documento | [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  0.2   | Adição da introdução | [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  0.3   | Adição de Alta Coesão | [Caio Martins](https://github.com/linktocaio) <br> [Yuri Alves](https://github.com/yuriAlves5)<br> [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  0.4   | Adição de Baixo Acoplamento | [Henrique Amorim](https://github.com/HenriqueAmorim20) <br> [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  0.5   | Adição de Controlador | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) <br> [Peniel Etèmana](https://github.com/zpeniel09) <br> [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  0.6   | Adição de Criador | [Lucas Melo](https://github.com/luucas-melo)<br>[Nilvan Peres](https://github.com/NilvanPeres)<br> [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  0.7   | Adição das Referências | [Lucas Lima](https://github.com/mibasFerraz) |
| 21.03.2022 |  1.0   | Revisão do documento | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |
| 21.03.2022 |  1.1   | Revisão do documento | [Lucas Lima](https://github.com/mibasFerraz) |

## Introdução

&emsp;&emsp; GRASP é um acrônimo para **General Responsability Assignment Software Patterns**, que em tradução livre significa **Padrões de Software para Atribuições Gerais de Responsabilidades**. Para a compreensão dos GRASP's, é primeiro necessário a contextualização da abordagem em mais alto nível, esta chamada de **Responsability-Driven-Development**, ou simplesmente **RDD**, que em tradução livre significa **Projeto Guiado por Responsabilidades**.

&emsp;&emsp; Larman define que o **RDD** é uma maneira de pensar em projetos de Orientação a Objetos que inclui a abstração de comportamentos entre os diferentes módulos do sistema. O _RDD_ é baseado em duas grandes camadas de abstração, a camada de _conhecer_, relacionada com instâncias e comunicações internas do código, e a camada de _fazer_, relacionada com os comportamentos e métodos implementados pelos diferentes módulos. A partir do **RDD**, tem-se que os GRASP's são um conjunto pragmático de princípios básicos que fornecem um referencial sólido para a programação orientada a objetos. [1]
Alta coesão é um padrão avaliativo que tenta manter os objetos adequadamente focados, gerenciáveis e compreensíveis. A alta coesão é geralmente utilizada em suporte de baixo acoplamento. A alta coesão significa que as responsabilidades de um determinado elemento estão fortemente relacionadas e altamente focadas. A quebra de programas em classes e subsistemas é um exemplo de atividades que aumentam as propriedades coesivas de um sistema. Alternativamente, a baixa coesão é uma situação em que um determinado elemento tem muitas responsabilidades distintas, não relacionadas. Elementos com baixa coesão muitas vezes sofrem de ser difíceis de entender, reutilizar, manter e são avessos à mudança.[4]

&emsp;&emsp;Desta forma, é válido afirmar que os GRASP's buscam oferecer um guia bem estruturado para soluções de software que se baseiam no paradigma da Orientação a Objetos. Como consequência direta da utilização dos padrões dentro de um projeto de software, tem-se a produção de uma base de código robusta e que apresenta um enorme fator de adaptabilidade diante de novas necessidades de projeto, de negócio ou, simplesmente, futuras mudanças planejadas para o código. Um código que segue as diretrizes propostas pelos GRASP's apresenta uma ótima organização entre os diferentes módulos; uma fácil manutenção e, por fim; uma boa capacidade de compreensão por diferentes desenvolvedores. [2]

&emsp;&emsp;Os GRASP são descritos pelos seguintes tópicos:

-   GRASP Criador;
-   GRASP Especialista;
-   GRASP da Alta Coesão;
-   GRASP do Baixo Acoplamento;
-   GRASP Controlador;
-   GRASP do Polimorfismo;
-   GRASP da Invenção Pura;
-   GRASP da Indireção;
-   E, por fim, GRASP de Variações Protegidas.

 &emsp;&emsp;No nosso projeto utilizamos os GRASP criador, especialista, baixo acoplamento, controlador e criador.

## Resultados


### Criador

#### Introdução

<p align="justify">&emsp;&emsp;
    Creator ou Criador é um dos padrões de Projeto GRASP, que assim como os outros tentam atribuir responsabilidades, papéis e colaborações. A criação de desenho de software desse padrão foca em identificar os responsáveis ideais para criação de objetos. Essa atribuição de obrigações de criação de objetos é de extrema importância para a modelagem do domínio, pois permite que a construção do software reduza acoplamentos desnecessários, além de facilitar o encapsulamento e reutilização do software. [2]
</p>

#### Metodologia

<p align="justify">&emsp;&emsp;
    Determinar isso pode não ser uma tarefa tão simples, por isso é importante analisar bem. Uma forma para determinar o responsável pela criação desses objetos é verificando da seguinte forma, supondo que temos uma classe A e B. A classe A cria a classe B se[1]:
</p>

<li>B contém ou agrega A</li>
<li>B registra a existência de A</li>
<li>B usa A</li>
<li>B tem os dados necessários para a inicialização de A que serão passados ao construtor de A</li>

#### Conclusão

<div style="width: 480px; height: 360px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:480px; height:360px" src="https://lucid.app/documents/embeddedchart/92a215e1-c772-41b4-b751-9ca7cb76976c" id="9T82cDyCgAB5"></iframe></div>


### Especialista

#### Introdução

&emsp;&emsp;Especialista na informação, ou apenas Expert, é um dos princípios básicos dentre os 9 GRASP’s existentes, em que visa uma abordagem genérica que atribui a responsabilidade de fazer ou conhecer algo, assim, basicamente o padrão de projeto Especialista se preocupa em atribuir responsabilidades para entidade do projeto.

&emsp;&emsp;Primeiramente, para esta atribuição é importante seguir um caminho objetivo onde  defini-se quais são as informações necessárias para se concluir uma tarefa obrigatória do sistema. Após a identificação é preciso avaliar qual é a camada que concentra o maior conhecimento acerca da tarefa em específica. Ao fim, com os módulos mapeados e levantados, aquele que possuir o maior conhecimento da tarefa é o forte candidato para especialista.


#### Aplicação

&emsp;&emsp;A partir da definição do padrão, trazemos como exemplo analisado a API do Backend do projeto Ki-Limpinho.


<center>
<img src='..\..\..\assets\img\grasp\especialista.jpeg'>
    <figcaption align='center'>
        <b>Figura 1: Estrutura de arquivos na camada Backend</b>
        <br>
        <small>Autor: Davi Matheus, 2022.</small>
    </figcaption>
</center>

#### Conclusão

Na figura anterior, vemos que o projeto é feito em node.js e evidenciamos que os especialistas são separados em diretórios, onde cada um possuem arquivos característicos para as suas respectivas funções, sendo elas:

- ```auth```, responsável pela a autenticação do projeto, controlando as rotas e os controllers.
- ```helpers```, responsável por ajudar e complementar algumas functios que o sistema percise;
- ```tests```, responsável pela implementação dos testes;
- ```user```, responsável por mapear  e implementar os endpoints e os metodos dos users, como as rotas as models os controlleres e etc;


### Alta Coesão

#### Definição

&emsp;&emsp; Alta coesão é um principio avaliativo que prega a divisão de responsabilidades entre as classe. Isso é, uma classe coesa é aquela que lhe foi delegada apenas as suas responsabilidades que estão fortemente relacionadas e altamente focadas. Classes com baixa coesão frequentemente são de difícil compreensão, difíceis de se reutilizar, manter ou alterar.

#### Utilização

&emsp;&emsp; Utilização da alta coesão deve estar presente durante todo o projeto para garantir que cada classe possua um única responsabilidade, dessa forma deixando-a compreensível, reutilizável e enxuta. Dessa maneira tornando as interfaces de comunicação mais claras, enquanto deixa as classes mais legíveis e amigáveis a expansões e alterações mantendo a complexidade gerenciável.

#### Conclusão

&emsp;&emsp; Com o presente documento é possível demonstrar a importância dos padrões de projeto GRASP dentro da construção da base do código, isto é, ser capaz de se identificar quais são as atribuições e responsabilidades de cada um dos componentes presentes.

### Baixo Acoplamento

#### Definição

&emsp;&emsp; Para definir o princípio do Baixo Acoplamento, antes é preciso definir em termos palpáveis o que é acoplamento: Larman define o acoplamento como uma métrica para mensurar o quão fortemente conectado se encontra o estado de um código específico, isto é, o quão dependente a camada de *conhecer* está entre os diversos componentes do sistema [1]. A partir disso, o princípio do baixo acoplamento fornece a visão necessária para a decisão da melhor forma de implementação que satisfaça:

- a menor dependência entre as classes;
- menor impacto por mudanças em classes existentes;
- maior potencial de reutilização de código.

#### Utilização

&emsp;&emsp; Ao utilizarmos os padrões já estabelecidos por uma REST API usando express, mongoose em NodeJS(ES6), já estamos utilizando as práticas de Baixo acoplamento, visto que cada um dos arquivos tem sua própria responsabilidade e seus próprios métodos definidos. Desta forma, a própria ferramenta já proporciona um nível adequado de conexão entre os componentes do código e também de modularização e reutilização do código.

#### Conclusão

&emsp;&emsp; Após todo o conteúdo explicitado neste documento, é possível evidenciar a importância dos padrões de projeto GRASP dentro da construção da base de código do projeto, isto é, é capaz de se identificar quais são as atribuições e responsabilidades de cada um dos componentes presentes no código.

### Controlador

#### Definição

&emsp;&emsp;O grasp controller ou controlador delega a responsabilidade pelo tratamento de evento do sistema à classes diferente da interface do usuário, ele delega o trabalho que precisa ser feito para outros objetos. Entre as normas que fazem parte desse padrão temos o Controller sobre qual estaremos falando.


#### Metodologia

<p align="justify">&emsp;&emsp;  O controlador é a camada responsável por receber as entradas que os usuários fazem através da interface do usuário e tratar desses eventos, geralmente é a camada intermediária entre as requisições dos atores e o backend que responde às requisições dessas requisições. Essa camada é responsável por entender as requisições dos usuários e logo em seguida redireciona essa requisição para o elemento no backend responsável por tratá-la. Em nosso código usamos muito o padrão controller e abaixo temos um exemplo de sua implementação. A metodologia que utilizaremos seria os controllers(controladores) do nosso projeto.
</p>

#### Utilização

<p align="justify">&emsp;&emsp;
Aqui temos cinco classes onde são implementados os controllers, uma para alguns dos principais objetos do sistema. O diagrama completo do projeto está disponível no <a href='../../../DiagramaDeClasses'>diagrama do classes</a>.
</p>
<p style="text-align: center">
<img src='..\..\..\assets\img\grasp\controlador.jpg' width='80%'>
  <figcaption align='center'>
      <b>
          <a href='..\..\..\assets\img\grasp\controlador.jpg'>
                Figura 1: Aplicação do controller no projeto
          </a>
      </b>
  </figcaption>
</p>

#### Conclusão

<p align="justify">&emsp;&emsp;

Este padrão, trabalha como uma camada de indireção para acontecimentos do projeto. Deixando os eventos causados pela Interface desacoplados dos objetos responsáveis por tratar a requisição, tornando o sistema mais flexível de fácil manutenção.
</p>



## Referências

> [1] Larman, C. 2005. Applying UML and Patterns – An Introduction to Object-Oriented Analysis and Design and Iterative Development 3rd ed. New Jersey.

> [2] Desenvolvimento com qualidade com GRASP. **DevMedia**. Disponível em: <https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704> (Último acesso em 11/03/2022).

> [3] SERRANO, Milene. Arquitetura e Desenho de Software AULA – GRASP – PARTE I. 36 slides. Disponível em: <https://aprender3.unb.br/pluginfile.php/897140/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP%20BASE%20Parte%20I%20-%20Profa.%20Milene.pdf> (Último acesso em 11/03/2022).

> [4] SERRANO, Milene. Arquitetura e Desenho de Software AULA – GRASP_A - COMPLEMENTAR – PARTE I. 66 slides. Disponível em: <https://aprender3.unb.br/pluginfile.php/897140/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP_A%20-%20Profa.%20Milene%20-%20Complementar.pdf> (Último acesso em 11/03/2022).

> [5] Larman, C. 2005. Applying UML and Patterns – An Introduction to Object-Oriented Analysis and Design and Iterative Development 3rd ed. New Jersey.

>  [6] BOAS, Leandro Vilas. Padrões GRASP - Padrões de Atribuir Responsabilidades. Disponível em: <https://medium.com/@leandrovboas/padr%C3%B5es-grasp-padr%C3%B5es-de-atribuir-responsabilidades-1ae4351eb204>. Acesso em 15, de Março de 2022.

> [7] Universidade Federal de Uberlândia. Padrões GRASP. Disponível em: <http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf>. Acesso em 15, de Março de 2022.

> [8] Controller – Padrões GRASP . Disponível em: <https://www.ramonsilva.net/post/controller-padr%C3%B5es-grasp>. Acesso em 15, de Março de 2022.

> [9] GRASP: Designing Objetos com Responsabilidades. [s.l: s.n.]. Disponível em: <https://www.ic.unicamp.br/~ariadne/mc436/1s2017/Lar16GRASP.pdf>. Acesso em: 13 mar. 2022.

> [10] SERRANO, Milene. Módulo de padrões de projeto GRASPs. 07a -VídeoAula - GRASP Criador.  Disponível em: <https://aprender3.unb.br/course/view.php?id=11018&section=4>. Acesso em: 15 mar. 2022.