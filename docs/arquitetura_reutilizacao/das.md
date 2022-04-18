# <center> Documento de Arquitetura de Software

## Histórico de Versão<br>

|Data | Versão | Descrição | Autor(es)|
| :-:|:-:|:-:|:-: |
| 14.04.2022 | 0.1 | Abertura do documento |[Peniel Etèmana](https://github.com/zpeniel09)|
| 14.04.2022 | 0.2 | Adição introdução, finalidade, escopo |[Peniel Etèmana](https://github.com/zpeniel09)|
| 17.04.2022 | 0.3 | Adição visão geral e representação arquitetural |[Peniel Etèmana](https://github.com/zpeniel09)|
| 17.04.2022 | 0.4 | Adição metas e Restrições de Arquitetura |[Peniel Etèmana](https://github.com/zpeniel09)|
| 18.04.2022 | 0.5 | Adição Visão de Casos de Uso |[Peniel Etèmana](https://github.com/zpeniel09)|


## Participantes

* [Peniel Etèmana](https://github.com/zpeniel09)

## 1- Introdução

&emsp;&emsp;O documento de arquitura de software fornece uma visão geral de arquitetura abrangente do sistema de software.

&emsp;&emsp;Esse documento serve como meio de comunicação entre o arquiteto de software e outros membros do equipe de projeto, com relação a decisões arquiteturalmente significativas tomadas sobre o projeto.

&emsp;&emsp;Nas linhas a seguir, estaremos falando um pouco mais sobre esse documento de arquitetura de software.

#### 1-1 Finalide

&emsp;&emsp;Este documento fornece uma visão arquitetural abrangente do sistema, usando diversas visões de arquitetura para representar diferentes aspectos do sistema. Ele pretende capturar e transmitir as decisões arquiteturas significativas que foram tomadas em relação ao sistema.

#### 1-3 Escopo

&emsp;&emsp;O Documento da Arquitetura de Software se aplica ao Sistema de Ki-Limpinho que será desenvolvido pela Integração do Contexto.Neste documento estaremos abordando os principais pontos desenvolvidos na arquitetura do projeto, a partir desse breve resumo de cada tópico é possível se orientar com relação a outros documentos da arquitetura desenvolvidos no projeto, onde é possível ter uma visão detalhada de cada tema.

&emsp;&emsp;Ki-Limpinho é uma aplicação que visa auxiliar no gerenciamento e comunicação com o cliente por parte do lava-jato, de modo que, durante o uso a frequência da execução de ações repetitivas por parte do gerente seja minimizada e o usuário possa facilmente solicitar serviços e também acompanha-los.


#### 1-4 Definições, Acrônimos e Abreviações

* RUP (Rational Unified Process)
* API (Aplication Programming Interface): Ela é um conjunto de definições e protocolos usado no desenvolvimento e na integração de software de aplicações, permitindo que um serviço interaja com outros produtos e serviços sem a necessidade de saber como eles foram implementados.
* GoF (Gang of Four)
* GRASP	(General Responsibility Assignment Software Patterns)
* DB (Database): Conhecido com Banco de Dados, local onde persistem os dados que devem ser salvos pela aplicação.

#### 1-5 Visão Geral

&emsp;&emsp;Esse documento de arquitetura contém os tópicos a seguir:
- [Introdução](#1--introdução)
- [Escopo](#1-3-escopo)
- [Representação Arquitetural](#2--representação-arquitetural)
- [Metas e Restrições de Arquitetura](#3--metas-e-restrições-de-arquitetura)
- [Visão dos Casos de Uso](#4--visão-de-casos-de-uso)
- Visão Lógica.
- Visão de Processos.
- Visão de Deploy.
- Visão de Implementação.
- Tamanho e Desempenho.
- Qualidade.
- [Referências](#referências)

## 2- Representação Arquitetural

&emsp;&emsp;A representação arquitetural serve para caracterizar a arquitetura de software de um sistema, possibilitando a:

- Identificação de componentes – o arquiteto identifica quais os principais elementos que tem funcionalidades bem definidas como, um componente de cadastro de (informações de) usuários e um componente de autenticação de usuário numa aplicação Web.
- Identificação de mecanismos de interação – a comunicação entre objetos por meio da troca de mensagens constitui uma forma através da qual os componentes de software interagem entre si.
- Identificação de propriedades – o arquiteto pode analisar as propriedades oferecidas por cada estilo baseado na organização dos componentes e nos mecanismos de interação, conforme discutido abaixo.

&emsp;&emsp;Das tecnologias:

* No nosso [frontend](https://github.com/UnBArqDsw2021-2/2021.2_g2_kilimpinho_frontend), foi utiliza o [TypeScript](https://en.wikipedia.org/wiki/TypeScript). É uma linguagem de programação de código aberto desenvolvida pela Microsoft. É um superconjunto sintático estrito de JavaScript e adiciona tipagem estática opcional à linguagem. 

* No [backend](https://github.com/UnBArqDsw2021-2/2021.2_G2_Ki-Limpinho_Backend) do nosso projeto, utilizamos as tecnologias [Node.js](https://en.wikipedia.org/wiki/Node.js) que é um software de código aberto, multiplataforma, baseado no interpretador V8 do Google e que permite a execução de códigos JavaScript fora de um navegador web; o [Express](https://en.wikipedia.org/wiki/Express.js) que é um framework para aplicativo da web do Node.js mínimo e flexível que fornece um conjunto robusto de recursos para aplicativos web e móvel. Ele é o principal bloco de construção de aplicações web com JavaScript e Node.JS; o [MongoDB](https://en.wikipedia.org/wiki/Mongoose_(MongoDB)) que é um software de banco de dados open source. Ele segue o modelo de banco de dados orientado a documentos, também chamado de bancos de dados NoSQL. É um dos bancos mais populares, possuindo uma comunidade ativa; o [Docker](https://en.wikipedia.org/wiki/Docker_(software)) que é uma tecnologia open source que permite aos desenvolvedores empacotar, entregar e executar aplicações em containers leves e autossuficientes. Contém uma comunidade que sempre está trabalhando para melhorar essa tecnologia. 

## 3- Metas e Restrições de Arquitetura

#### 3-1 Restrições

- O software deve ser desenvolvido nas tecnologias definidas;
- O software deve rodar nos navegadores: Web Firefox e Google Chrome;
- O ambiente de desenvolvimento do software deve funcionar tanto em Windows, Linux e MacOS;
- É preciso ter uma conexão com a internet para utilizar a aplicação;
- O escopo do projeto deve ser concluído até o final da disciplina.

#### 3-2 Metas

* Portabilidade – Deve ser possível utilizar a plataforma em qualquer navegador web.
* Usabilidade - O software deve possuir alta aprendibilidade e inteligibilidade, para que atenda aos requisitos elicitados no formulário criado pelo grupo;
* Manutenibilidade: O código e as documentações realizadas pelo grupo devem estar num nível de qualidade, seguindo os padrões de projeto e bibliografia, onde a sua manutenção seja fácil de ser realizada a qualquer momento que for desejado.

## 4- Visão de Casos de Uso.

&emsp;&emsp; A visão de casos de uso é documenta o que o sistema faz do ponto de vista do usuário. Em outras palavras, ela descreve as principais funcionalidades do sistema e a interação dessas funcionalidades com os usuários do mesmo sistema. Nesse diagrama não nos aprofundamos em detalhes técnicos que dizem como o sistema faz. 

&emsp;&emsp;Esse diagrama é composto basicamente por quatro partes que são:
- Cenário: Sequência de eventos que acontecem quando um usuário interage com o sistema.
- Ator: Usuário do sistema, ou melhor, um tipo de usuário.
- Use Case: É uma tarefa ou uma funcionalidade realizada pelo ator (usuário)
- Comunicação: é o que liga um ator com um caso de uso

&emsp;&emsp;Foram levantados alguns casos de usos nesse [documento de caso de uso](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/DiagramaCasoUso/), sendo assim, iremos falara um pouco mais sobre os casos de uso mais significativos.

- **[UC01 - Listar despesas](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/casosDeUso/UC01/)**
- **[UC02 - Registar despesas](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/casosDeUso/UC02/)**
- **[UC05 - Vizualizar serviços](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/casosDeUso/UC05/)**
- **[UC08 - Realizar cadastro](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/casosDeUso/UC08/)**
- **[UC09 - Realizar Logout](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/casosDeUso/UC09/)**
- **[UC11 – Realizar login](https://unbarqdsw2021-2.github.io/2021.2_G2_Ki-Limpinho/modelagem/diagramas/casosDeUso/UC11/)**


## Referências

> [1] **SERRANO, Milene.** Arquitetura e Desenho de Software. **AULA - ARQUITETURA & DAS – PARTE II.** Acesso em 14, Abril de 2022.

> [2] **Docker**. Disponível em: <https://stack.desenvolvedor.expert/appendix/docker/oquee.html>. Acesso em 17, Abril de 2022.

> [3] **Representação Arquitetural**. Disponível em: <https://www.devmedia.com.br/arquitetura-de-software-desenvolvimento-orientado-para-arquitetura/8033#:~:text=O%20estilo%20arquitetural%20considera%20o,todos%20os%20componentes%20do%20sistema.>. Acesso em 17, Abril de 2022.

> [4] **Visão de casos de uso**. Disponível em: <https://www.devmedia.com.br/o-que-e-uml-e-diagramas-de-caso-de-uso-introducao-pratica-a-uml/23408>. Acesso em 18, Abril de 2022.