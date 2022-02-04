# Documento de visão

## Histórico de revisão
| Data   | Versão | Modificação  | Autor  |
| :- | :- | :- | :- |
| 29/01/2022 | 1.0.0 | Criação e elaboração do documento |  Nilvan Júnior |
| 31/01/2022 | 1.0.1 | Correção de alguns erros |  Nilvan Júnior |


## Sumário 
[1 - Introdução](#1---introdução)
* [1.1 - Propósito](#1.1---Propósito)
* [1.2 - Escopo](#1.2---escopo)
* [1.3 - Definições, acrônomos e Abreviações](#1.3---Definições,-acrônomos-e-Abreviações)
* [1.4 - Referências](#1.4---Referências)
* [1.5 - Visão Geral](#1.5---Visão-Geral)

[2 - Posicionamento](#2---Posicionamento)
* [2.1 - Oportunidade de negócios](#2.1---Oportunidade-de-negócios)
* [2.2 - Descrição do problema](#2.2---Descrição-do-problema)
* [2.3 - Descrição de posição de produto](#2.3---Descrição-de-posição-de-produto)

[3 - Descrições da parte interessada e do usuário](#3---Descrições-da-parte-interessada-e-do-usuário)
* [3.1 - Resumo dos envolvidos](#3.1---Resumo-dos-envolvidos)
* [3.2 - Resumo dos usuários](#3.2---Resumo-dos-usuários)
* [3.3 - Perfis dos envolvidos](#3.3---Perfis-dos-envolvidos)
    * [3.3.1 - Equipe de desenvolvimento de software](#3.3.1---Equipe-de-desenvolvimento-de-software )
    * [3.3.2 - Avaliadores](#3.3.2---Avaliadores)
* [3.4 - Perfis dos usuários](#3.4---Perfis-dos-usuários)
    * [3.4.1 - Gerente](#3.4.1---Gerente)
    * [3.4.2 - Proprietário automotivo](#3.4.2---Proprietário-automotivo)
* [3.5 - Ambiente dos usuários](#3.5---Ambiente-dos-usuários)
* [3.6 - Alternativas e concorrências](#3.6---Alternativas-e-concorrências)

[4 - Visão geral do produto](#4---Visão-geral-do-produto)
* [4.1 - Perspectiva do produto](#4.1---Pespectiva-do-produto)
* [4.2 - Resumo de capacidades](#4.1---Resumo-de-capacidades)
* [4.3 - Suposições e Dependências](#4.1---Suposições-e-Dependências)
  
[5 - Recursos do produto](#5---Recursos-do-produto)

[6 - Restrições](#6---Restrições)
* [6.1 - Restrições de design](#6.1---Restrições-de-design)
* [6.2 - Restrições de implementação](#6.2---Restrições-de-implementação)
* [6.3 - Restrições de segurança](#6.3---Restrições-de-segurança)
* [6.4 - Restrições de uso](#6.4---Restrições-de-uso)

### My Multi Word Header

## 1 - Introdução 

### 1.1 - Propósito

<p align="justify">&emsp;&emsp;
  Esse documento tem como principal objetivo principal fornecer uma visão geral sobre o projeto que será desenvolvido, o escopo que está inserido e a finalidade do produto. Aos fatos, também é esperado que ao final dessa leitura estejam claros as principais características e requisitos de nossa aplicação web, entendimento do problema que buscamos resolver, expecativas em relação ao que será desenvolvido, e alguns mecanismos para reduzir riscos que possam afetar a entrega do produto. [1]
</p>

<p align="justify">&emsp;&emsp;
  A estrutura de tópicos desse documento foi inspirada no documento de orientação da IBM(International Businness Machines Corp), e foram realizadas algumas adpatações que julguei pertinente, devido ao nível de abstração que nos encontramos em relação ao nosso projeto.
</p>


### 1.2 - Escopo

<p align="justify">&emsp;&emsp;
  Esse projeto tem como principal objetivo a elaboração de uma aplicação web, que será utilizada por gerentes de algum lava-jato e atender a uma possível clientela da lava-jato em questão. Visando permitir mais flexibilidade para os clientes marcarem os serviços na melhor data e avaliarem a qualidade do serviço prestado, além de facilitar o gerenciamento dos proprietários a partir de dashboards.
</p>

### 1.3 - Definições, acrônomos e Abreviações

<p align="justify">&emsp;&emsp;
  <ul> 
    <li> FGA - Faculdade do Gama (UnB) </li>
    <li> UnB - Universidade de Brasília </li>
    <li> IBM - International Business Machines </li>
    <li> IBGE - Instituto Brasileiro de Geografia e Estatística </li>
    <li> KR's - Key result's </li>
    <li> ArqDsw - Arquitetura e desenho de software </li>
  </ul>
</p>


### 1.4 - Referências

<p align="justify">&emsp;&emsp;

  <ul>
    <li> [1] - IBM Knowlege Center - Documento de visão. Disponível em: < <a href="https://www.ibm.com/docs/pt-br/elm/6.0.5?topic=requirements-vision-document" >https://www.ibm.com/docs/pt-br/elm/6.0.5?topic=requirements-vision-document </a> >.Acesso em: 29 jan. 2022; </li>
    <li> [2] - IBGE - Frota de veículos. Disponível em: < <a href="https://cidades.ibge.gov.br/brasil/pesquisa/22/28120">https://cidades.ibge.gov.br/brasil/pesquisa/22/28120</a> >.Acesso em: 29 jan. 2022</li>
    <li> [3] - GrLavaJato - Principais funcionalidades: Disponível em: < <a href="https://www.grlavajato.com.br/">https://www.grlavajato.com.br</a> >. Acesso em 29 jan. 2002</li>
    <li> Hortum - Documento de Visão. Disponível em: < <a href="https://fga-eps-mds.github.io/2020.2-Hortum/Documento_de_visao/">https://fga-eps-mds.github.io/2020.2-Hortum/Documento_de_visao/</a> >. Acesso em: 29 jan. 2022
  </ul>

</p>


### 1.5 - Visão Geral

<p align="justify">&emsp;&emsp;
  Este documento é consituído em seis tópicos que destrincham as principais características e fornecem uma ideia geral de como será o planejamento de construção do produto.
  <ul> 
    <li>Introdução: Parte na qual as ideias gerais são introduzidas, fornecendo um pequeno overview sobre o projeto.</li>
    <li>Posicionamento: Parte na qual o problema é apresentado, e quais são as hipóteses de solução, além da oportunidade do negócio.</li>
    <li>Perfis dos Envolvidos e dos Usuários: Este tópico abordará os potenciais perfis das partes interessadas no projeto.</li>
    <li>Visão geral do produto:  Esta seção será dedicada para fornecer uma visão de alto nível sobre as principais características do produto.</li>
    <li>Recursos do produto: Parte na qual o sistema será destrinchado, para melhor entendimento dos recursos necessários para entregar um produto de qualidade para os usuários.</li>
    <li>Restrições: O nome é sugestivo, nessa seção serão mapeadas quais serão as principais restrições do projeto, podendo ser externas, operacionais, regulamentares ou de design.</li>
  </ul>
</p>

## 2 - Posicionamento

### 2.1 - Oportunidade de negócios 

<p align="justify">&emsp;&emsp;
  A tecnologia está presente em praticamente todos os setores de nossa economia, e um fato que não se discute é: empresa que não se moderniza fica para trás. Vale ressaltar que, o número da frota de veículos do Brasil é equivalente a metade da população, dessa forma é um nicho que se bem explorado, pode ser bem rentável e acaba abrindo a possibilidade para expansões do negócio. [2]
</p>
<p align="justify">&emsp;&emsp;
  Dessa forma, nosso projeto tem como foco auxiliar gerentes de lava-jato a otimizarem o acesso a informações de seus clientes, e um módulo de dashboards para controle financeiro, além de gráficos mensais com a quantidade de serviçõs prestados e cancelados. Possibilitando maior gerenciamento sobre o estabelecimento e sua clientela.
</p>
<p align="justify">&emsp;&emsp;
  É importante lembrar que a aplicação também será utilizada pelos potenciais clientes, podendo escolher o tipo de lavagem desejada e qual data e horário ficará melhor para o mesmo, permitindo maior flexibilidade e menos perca de tempo para o cliente, além de um sistema feedbacks em relações aos serviços prestados.
</p>


### 2.2 - Descrição do problema

| O problema é  | quem afeta | cujo impacta  | possível solução  |
| :- | :- | :- | :- |
| Lava-jatos que ainda não são informatizadas. | Proprietários/gerentes de lava-jatos.  | A qualidade do monitoramento do estabelecimento, e limita ampliação do negócio. | Aplicação web capaz de otimizar o gerenciamento do estabelecimento com os principais KR's disponibilizados em dashboards, e permitir que os clientes consigam marcar e pagar por um serviço pela aplicação. |


<p align="justify">&emsp;&emsp;
  Uma solução bem-sucedida permitirá: 
  <ul> 
    <li>Com o maior controle sobre o <b>fluxo de caixa</b> do negócio a partir do <b>dashboards</b>, será possível identificar quais são os principais gargalos da empresa que podem estar atrapalhando a expansão do mesmo. </li>
    <li>Será possível implementar um <b>sistema de fidelização dos clientes</b>, isto é, a partir de uma quantidade X de serviços contratatos oferecer descontos satisfatórios para os clientes.</li>
    <li>A partir do <b>sistema de feedback</b> de serviços prestados, será possível bonificar os funcionários responsáveis por esse serviço, ou mapear possíveis melhorias para o estabelecimento.</li>
  </ul>
</p>


### 2.3 - Descrição de posição de produto

<p align="justify">&emsp;&emsp;
  O produto final é uma aplicação web que servirá <b>para</b> auxiliar gerentes e clientes de lava-jatos, para que, tenham um acesso de forma virtual. O <b>CarWashPremium</b> veio para auxiliar o ramo de lava-jatos, ferramentas como dashboards, sistema de feedback, agendamento e pagamento de serviço, e permitirão uma melhor conexão da lava-jato com os clientes. Aplicações como o "Meu Lava Jato" e "Gr lavajato", buscam oferecer um gerenciamento de entrada e saída de carros, assim como cadastro de clientes, e agendamento de serviços, status de serviço,e orçamentos de serviços. Apesar do segundo ser bem completo, o que estamos propondo é algo mais focado no cliente, e funcionalidades essenciais para os gerentes como mostrar KR's a partir de dashboards para facilitar leitura dos dados, facilitando traçar um plano de ação. Além de permitir que proprietários automotivos possam utilizar a aplicação, para que não tenham que ficar horas na fila, e consigam avaliar qualidade do serviço prestado, também acreditamos que o sistema de fidelização em conjunto com o cadastro de promoções será um grande diferencial para retenção de clientes. [3]
</p>


## 3 - Descrições da parte interessada e do usuário

### 3.1 - Resumo dos envolvidos
| Nome  | Descrição | Responsabilidades |
| :- | :- | :-  |
| Equipe de desenvolvimento do Software | Estudantes da disciplina ArqDSW (Arquitetura e Desenho de Software). | Desenvolvimento seguindo padrões de qualidades, testes, documentação geral e específica da arquitetura do produto e implementações do Software. |
| Avaliadores  | Professora na Universidade de Brasília, atual resposável pela disciplina de ArqDSW. | Avaliar e auxiliar os estudantes nas etapas de previstas na disciplina. |

### 3.2 - Resumo dos usuários
| Nome  | Descrição |
| :- | :- |
| Gerente | Proprietários ou gerentes de lava-jatos interessados na otimização de monitoramento do negócio. | Validação informal. |
| Proprietários de veículos | Pessoas interessadas em consumir os serviços ofertados em um lava-jato.  | Validação informal. | 

### 3.3 - Perfis dos envolvidos  

#### 3.3.1 - Equipe de desenvolvimento de software 
| Representantes | Davi Matheus, Nilvan Peres, Natanael Fernandes, Lucas Ferraz, Henrique Amorim, Jonathan Jorge, Yuri Alves, Lucas Melo, Peniel Etèmana e Caio Martins. |
| :--- | :-------- |  
| Descrição | Estudantes do curso de Engenharia de Software da FGA. |
| Responsabilidades | Desenvolver e documentar o projeto, realizar testes e validar o projeto.
| Critérios de Sucesso | Finalizar o aplicativo no prazo determinado, atendendo os requisitos de mais alta prioridade.
| Envolvimento | Alto. |
| Problemas/Comentários | Organizar horários para dez integrantes, seguir prazo de entregas, sobrecarga em algum membro do projeto.|

#### 3.3.2 - Avaliadores
| Representantes | Professora Milene Serrano | 
| :--- | :-------- |  
| Descrição | Professora da disciplina ArqDSW. |  
| Responsabilidades | Orientar e avaliar a equipe em cada fase da disciplina. |
| Critérios de Sucesso | Transmitir conhecimento para a equipe conseguir elaborar os artefatos solicitados, e fornecer feedbacks em relação as entregas. |
| Envolvimento | Médio. |
| Problemas/Comentários | Penalização de integrantes que não estão auxiliando a equipe, tornando o processo mais árduo e possivelmente sobrecarregando outros membros. |

### 3.4 - Perfis dos usuários  

#### 3.4.1 - Gerente
| Representante | Gerente. |
| :--- | :-------- |  
| Descrição | Gerente de algum lava-jato em busca de uma ferramenta o auxiliar a otimizar seu serviço. |
| Responsabilidade  | Monitorar o lava-jato, identificar possíveis melhorias, e realizar estímulos para retenção de clientes |
| Critérios de sucesso | Conseguir aumentar quantidade de serviços prestados por meio da plataforma |
| Envolvimento | Alto. |
| Problemas/Comentários | Não possuir muito conhecimento com aplicações web.|

#### 3.4.1 - Proprietário automotivo
| Representante | Proprietário automotivo.  |
| :--- | :-------- |  
| Descrição | Proprietário automotivo interessados em serviços de um lava-jato.   |
| Responsabilidade  | Procurar e comprar serviço desejado, e realizar avaliação do serviço de acordo com a experiência que lhe foi proporcionada. |
| Critérios de sucesso | Encontrar produto desejado, e ser entregue um serviço de melhor qualidade. |
| Envolvimento | Alto. |
| Problemas/Comentários | Não possuir muito conhecimento com aplicações web.|

### 3.5 - Ambiente dos usuários

<p align="justify">&emsp;&emsp;
  Os usuários poderão utilizar a plataforma a partir de computador ou celular por meio de uma página web.
</p>

### 3.6 - Alternativas e concorrências

<p align="justify">&emsp;&emsp;
  GrLavaJato: Focada bastante no serviço de análise e gerenciamento do lava-jato. Os mesmos, dividiram a aplicação em 4 grandes módulos: serviços, clientes, depesas e indicadores. Entrega funcionalidades interessantes para o gerente, mas não há um espaço onde os clientes possam marcar/visualizar os serviços disponíveis, ou deixar algum tipo de feedback, acreditamos que possamos nos destacar aqui, explorando a conexão entre plataforma e cliente.
</p>
<p align="justify">&emsp;&emsp;
  MeuLavaJato: Aplicação mobile, também fornece algumas funcionalidades para melhor gerenciamento do lava-jato, entretanto é bem mais limitada que a GrLavaJato, as funcionalidades são muito simples, os indicadores são mostrados em um modelo que simplesmente lembra uma calculadora. Acreditamos que com o uso de dashboards com os principais KR's da lava-jato, auxiliará na análise de dados e trará insumos importantes para melhorias no negócio.
</p>


## 4 - Visão geral do produto

### 4.1 - Perspectiva do produto
<p align="justify">&emsp;&emsp;
  A aplicação web <b>CarWashPremium</b> busca atender dois públicos essenciais para o lava-jato, os gerentes, e seus clientes. Para o gerente permitirá maior monitoramento sobre os serviços que estão sendo prestados, além de dashboards que ajudarão a acompanhar o fluxo de caixa do negócio. Para os proprietário automotivos buscará fornecer maior comodidade podendo escolher melhor horário e serviço, conseguir descontos, além de conseguir avaliar como foi o serviço prestado.
</p>

### 4.2 - Resumo das capacidades
| Benefício  |  Recursos de suporte|
| :--- | :-------- |  
| Auxiliar gerentes de lava-jata com suas responsibilidades. | Aplicação web de fácil usabilidade, onde será possível acompanhar fluxo de caixa a partir de gráficos, analisar quantidade de serviços contratados, visualizar feedbacks de clientes e cadastrar promoções.|
| Auxiliar proprietários de carro a contratarem serviços de lava-jato. | Aplicação web com interface intuitiva, onde será possível listar os serviços prestados, escolher uma data e horário para o tipo de lavagem escolhida, contratar, avaliação de serviço prestado.  |

### 4.3 - Suposições e dependências
<p align="justify">&emsp;&emsp;
  <ul> 
    <li>O usuário deverá ter computador/celular e uma conexão estável com a internet.</li>
    <li>A aplicação permitirá maior conexão entre clientes e gerentes da lava-jato.</li>
    <li>O usuário deverá levar o carro ao lava-jato na data que e horário que foi escolhido.</li>
  </ul>
</p>

## 5- Recursos do produto

### 5.1 Recursos do Gerente
<p align="justify">&emsp;&emsp;
  <ul> 
    <li>Cadastro na plataforma.</li>
    <li>Cadastrar promoções.</li>
    <li>Visualizar feedbacks.</li>
    <li>Visualizar gráfico de lucro bruto/líquido mensal.</li>
    <li>Visualizar gráfico com quantidade de serviços contratados/cancelados.</li>
    <li>Visualizar gráfico de fluxo de caixa.</li>
  </ul>
</p>

### 5.2 Recursos do Proprietário do carro
<p align="justify">&emsp;&emsp;
  <ul> 
    <li>Cadastro na plataforma.</li>
    <li>Visualizar tipos de lavagens disponíveis.</li>
    <li>Marcar data e horário, e pagar pelo serviço de escolhido.</li>
    <li>Aplicar cupons de descontos.</li>
    <li>Avaliar qualidade do serviço prestado.</li>
  </ul>
</p>

## 6 - Restrições

### 6.1 - Restrições de design
<p align="justify">&emsp;&emsp;
  O design será elegante e simples, proporcional ao tempo de trabalho estimado (12 semanas), buscando atender, prioritariamente, as essencialidades do projeto. De forma que a aplicação seja intuitiva e de uso fácil e autoexplicativo.
</p>

### 6.2 - Restrições de implementação

<p align="justify">&emsp;&emsp;
  O sistema será desenvolvido fazendo-se uso da linguagen Javascript, utilizando NodeJS para o back-end. E o framework escolhido para o front-end será o ReactJS.
</p>


### 6.3 - Restrições de segurança

<p align="justify">&emsp;&emsp;
É assegurado tanto ao gerente quanto ao cliente total sigilo de suas informações pessoais.
</p>


### 6.4 - Restrições de uso
<p align="justify">&emsp;&emsp;
  Faz-se necessário o acesso à internet pelo usuário, e o navegador escolhido deve ser capaz de suportar o sistema. Caso contrário, o usuário não conseguirá utilizar a plataforma e terá uma experiência desagradável pelos possíveis erros de compatabilidade que podem ocorrer.
</p>



