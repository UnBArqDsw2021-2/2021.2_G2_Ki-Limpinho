# <center> GRASPS


### Histórico de Versão
|    Data    | Versão | Descrição            | Autor(es)       |
| :--------: | :----: | :------------------: | :-------------: |
| 20/03/2022 |  0.1   | Criação do Documento | [Lucas Lima](https://github.com/mibasFerraz) |
| 21/03/2022 |  0.2   | Adição da introdução | [Lucas Lima](https://github.com/mibasFerraz) |
| 21/03/2022 |  0.3   | Adição de Alta Coesão | [Lucas Lima](https://github.com/mibasFerraz) |
| 21/03/2022 |  0.3   | Adição de Baixo Acoplamento | [Lucas Lima](https://github.com/mibasFerraz) |
| 21/03/2022 |  0.3   | Adição de Controlador | [Lucas Lima](https://github.com/mibasFerraz) |


### Introdução

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

 &emsp;&emsp;No nosso projeto utilizamos os GRASP criador, baixo acoplamento, controlador e criador.

 ### Alta Coesão

### Definição

&emsp;&emsp; Alta coesão é um principio avaliativo que prega a divisão de responsabilidades entre as classe. Isso é, uma classe coesa é aquela que lhe foi delegada apenas as suas responsabilidades que estão fortemente relacionadas e altamente focadas. Classes com baixa coesão frequentemente são de difícil compreensão, difíceis de se reutilizar, manter ou alterar.

### Utilização

&emsp;&emsp; Utilização da alta coesão deve estar presente durante todo o projeto para garantir que cada classe possua um única responsabilidade, dessa forma deixando-a entendível, reutilizável e enxuta. Dessa maneira tornando as interfaces de comunicação mais claras, enquanto deixa as classes mais legíveis e amigáveis a expansões e alterações mantendo a complexidade gerenciável.

## Conclusão

&emsp;&emsp; Com o presente documento é possível demonstrar a importância dos padrões de projeto GRASP dentro da construção da base do código, isto é, ser capaz de se identificar quais são as atribuições e responsabilidades de cada um dos componentes presentes.


## Baixo Acoplamento

### Definição

&emsp;&emsp; Para definir o princípio do Baixo Acoplamento, antes é preciso definir em termos palpáveis o que é acoplamento: Larman define o acoplamento como uma métrica para mensurar o quão fortemente conectado se encontra o estado de um código específico, isto é, o quão dependente a camada de *conhecer* está entre os diversos componentes do sistema [1]. A partir disso, o princípio do baixo acoplamento fornece a visão necessária para a decisão da melhor forma de implementação que satisfaça:

- a menor dependência entre as classes;
- menor impacto por mudanças em classes existentes;
- maior potencial de reutilização de código.

### Utilização

&emsp;&emsp; Ao utilizarmos os padrões já estabelecidos por uma REST API usando express, mongoose em NodeJS(ES6), já estamos utilizando as práticas de Baixo acoplamento, visto que cada um dos arquivos tem sua própria responsabilidade e seus próprios métodos definidos. Desta forma, a própria ferramenta já proporciona um nível adequado de conexão entre os componentes do código e também de modularização e reutilização do código.

## Conclusão

&emsp;&emsp; Após todo o conteúdo explicitado neste documento, é possível evidenciar a importância dos padrões de projeto GRASP dentro da construção da base de código do projeto, isto é, é capaz de se identificar quais são as atribuições e responsabilidades de cada um dos componentes presentes no código.


<p align="justify">&emsp;&emsp;O grasp controller ou controlador delega a responsabilidade pelo tratamento de evento do sistema à classes diferente da interface do usuário, ele delega o trabalho que precisa ser feito para outros objetos. Entre as normas que fazem parte desse padrão temos o Controller sobre qual estaremos falando.
</p>

## Metodologia

<p align="justify">&emsp;&emsp;  O controlador é a camada responsável por receber as entradas que os usuários fazem através da interface do usuário e tratar desses eventos, geralmente é a camada intermediária entre as requisições dos atores e o backend que responde às requisições dessas requisições. Essa camada é responsável por entender as requisições dos usuários e logo em seguida redireciona essa requisição para o elemento no backend responsável por tratá-la. Em nosso código usamos muito o padrão controller e abaixo temos um exemplo de sua implementação. A metodologia que utilizaremos seria os controllers(controladores) do nosso projeto.
</p>

## Resultados

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

## Conclusão

<p align="justify">&emsp;&emsp;

Este padrão, trabalha como uma camada de indireção para acontecimentos do projeto. Deixando os eventos causados pela Interface desacoplados dos objetos responsáveis por tratar a requisição, tornando o sistema mais flexível de fácil manutenção.
</p>