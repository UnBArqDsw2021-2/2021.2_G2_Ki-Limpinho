# ✅ Termo de Abertura do Projeto

| Data       | Versão | Descrição      | Autor(es)                                            |
| ---------- | ------ | -------------- | ---------------------------------------------------- |
| 30/01/2022 | 0.1    | Versão inicial | Lucas Lima, Jonathan Jorge, Yuri Alves Bacarias      |
| 03/02/2022 | 0.2    | Versão inicial | Caio Martins, Lucas Lima, Jonathan Jorge, Yuri Alves |

## Sumário

- [✅ Termo de Abertura do Projeto](#-termo-de-abertura-do-projeto)
  - [Sumário](#sumário)
- [1 - Introdução](#1---introdução)
- [2 - Descrição do projeto](#2---descrição-do-projeto)
- [3 - Propósito e justificativa do projeto](#3---propósito-e-justificativa-do-projeto)
- [4 - Requisitos de alto nível](#4---requisitos-de-alto-nível)
- [5 - Restrições](#5---restrições)
- [6 - Riscos](#6---riscos)
- [7 - Estimativas de Custos](#7---estimativas-de-custos)
- [8 - Referências Bibliográficas](#8---referências-bibliográficas)

# 1 - Introdução

Esse documento possui o intuito de apresentar as principais características e traços iniciais do projeto **Lava-Jato**, ao final da leitura estará claro a visão inicial do projeto e seus principais pontos de desenvolvimento, e os stakeholders do mesmo.

# 2 - Descrição do projeto

Esse projeto foi proposto pela Milene Serrano. A proposta tem seu escopo reduzido com a ideia de ser desenvolvido em 15 semanas, o projeto **Lava-Jato** é uma página web dedicada a uma empresa que está com dificuldades de ampliar seu negócio devido a problemas de gestão. A plataforma funcionará fornecendo ao gerente/dono a possibilidade de visualizar o fluxo de caixa, serviços, clientes e agendamento de lavagem. Aos clientes a possibilidade de realizar seu cadastro na aplicação, visualizar os serviços disponíveis e seus respectivos preços e agendar um serviço.

# 3 - Propósito e justificativa do projeto

Com o aumento de clientes e serviços, tornou-se insustentável devido a falta de organização da empresa. Dito isso, é de extrema importância reorganizar a forma de gestão e a maneira mais eficaz encontrada foi a de criar este software para a organização dos clientes, serviços, agendas, financeiro e todas as etapas envolvidas nesse processo.

# 4 - Requisitos de alto nível

A plataforma será uma página web sendo possível o acesso a partir de computadores e celulares, o acesso será de forma gratuita. Os requisitos de alto nível são:

|           Nome            |                                                     Descrição                                                      |
| :-----------------------: | :----------------------------------------------------------------------------------------------------------------: |
|             -             |        Configurar a integração do site dentro dos frameworks escolhidos para o projeto. (a serem definidos)        |
|    Cadastro do cliente    |                Realizar cadastro do cliente com dados de comunicação, endereço e de identificação.                 |
|   Cadastro de serviços    |                      Realizar cadastro dos serviços com suas respectivas descrições e preços                       |
| Visualizar Fluxo de caixa |                                               Dashboard com entrada                                                |
|   Realizar agendamentos   |                      Permitir o agendamento de um serviço por parte do cliente e do gerente.                       |
|      Banco de Dados       | Permitir a comunicação entre o front e o banco de dados (a ser definido) para a criação de dashboards interativas. |

# 5 - Restrições

-   O prazo para entrega do projeto é (a ser definida)
-   O projeto deve ser construído pela equipe 02 do segundo semestre letivo de 2021 da matéria Arquitetura e Desenho de Software.

# 6 - Riscos

Nessa etapa é identificada o plano de risco do projeto. No gerenciamento de riscos é possível ter um certo controle sobre as incertezas que o projeto pode ter, além de medir o impacto.

| Impacto     | Descrição                              |
| ----------- | -------------------------------------- |
| Muito Baixo | Quase que imperceptível para o projeto |
| Baixo       | pouca influencia                       |
| Média       | influencia mas solucionável            |
| Alto        | Muita influencia no projeto            |
| Muito Alto  | influencia critica                     |

| probabilidade |
| ------------- |
| Muito Baixo   |
| Baixo         |
| Média         |
| Alta          |
| Muito Alta    |

| Risco                                           | Impacto    | probabilidade | prevenção                                                                                                         |
| ----------------------------------------------- | ---------- | ------------- | ----------------------------------------------------------------------------------------------------------------- |
| Aluno retira a disciplina                       | Alto       | Média         | manter o grupo sempre alinhado e contente                                                                         |
| Perda de prazo das entregas                     | Alto       | Baixa         | Manter o grupo coordenado e sempre alinhado com os prazos                                                         |
| Falta de comunicação na equipe                  | Alto       | Muito Baixa   | Manter um espaço de comunicação saudável                                                                          |
| Um dos membros ficar impossibilitado por doença | Alto       | Alta          | Reorganizar as tarefas de modo a não sobrecarregar os outros integrantes                                          |
| Equipe incapacitada tecnicamente                | Muito Alto | Baixa         | Escolha correta das tecnologias usadas abrangendo o conhecimento geral além de possibilidade de tempo para estudo |
| Bugs/Falha                                      | Alto       | Muito Alta    | Realizando testagem periodicamente                                                                                |
| Divergência de grade horária                    | Baixo      | Muito Alta    | Realização de heatmap, mantendo uma estratégia de distribuição de tarefas                                         |
| Sobrecarga de algum membro                      | Médio      | Média         | Reajuste de tarefas                                                                                               |
| Falta de monitoramento e controle               | Alto       | Média         | Elaboração de um cronograma com acompanhamento sistemático                                                        |

# 7 - Estimativas de Custos

Para realizar o cálculo de estima de custo do projeto foi utilizado a técnica COCOMO intermediário para classe de projetos semidestacados.

Levando em consideração a natureza da materia e o escopo do projeto a ser desenvolvido vemos como necessário o uso de um modelo mais avançado em relação ao COCOMO Básico, mas lidar com variáveis muito complexas como no COCOMO Detalhado se faz desnecessário. Com o método COCOMO Intermediário calcularemos o esforço e o custo de desenvolvimento considerando uma estimativa do tamanho do programa e um conjunto de direcionadores de custo. Dado as características do software que será desenvolvido, no caso uma aplicação web para facilitar e agilizar o trabalho de clientes e gerentes de lava jatos, o projeto se encaixa na classe de Semidestacado, pois ele exige certos requisitos rígidos, como confiabilidade nos dados cadastrados de clientes e seus carros. Além disso a equipe é composta por uma equipe heterogênea em quesitos como experiência com as tecnologias.

O projeto conta com uma complexidade moderada, mas a utilização de um framework contribuirá para reduzir o tempo de desenvolvimento e a quantidade de linhas de código. No frontend será utilizado React que possui uma organização por componentes e da suporte para uma grande reutilização de código. Para a construção do backend será utilizado NodeJS. A equipe de desenvolvimento estimou que o software a ser produzido deve possuir entre 4500 e 4000 linhas de código sem considerar as bibliotecas adicionais que serão utilizadas para facilitar o desenvolvimento.

Estimativa de Esforço:

$$
E = a*S^b*fae
$$

onde:
E: é o esforço aplicado (em pessoas-mês).
S: é o número (estimado) de linhas de código para o projeto (em milhares).
a: é um coeficiente fornecido pela tabela de Boehm(1981).
b: é um expoente fornecido pela tabela de Boehm(1981).
fae: é o Fator de Ajustamento do Esforço, onde é baseado na tabela de Boehm(1981) e a equipe se reuniu para definir os valores para a confeção do fae.

a = 3
b = 1.12
fae = 0.6765

S = 4500 LoC ou S = 4.5 KLoC temos:

$$
E = 3 *4.5^{1.12}* 0.6765
$$

$$
E = 10.94 pessoas/mês
$$

Para S = 4000 LoC ou S = 4 KLoC temos:

$$
E = 3 *4^{1.12}* 0.6765
$$

$$
E =  9.59   pessoas/mês
$$

Estimativa de Tempo:

$$
T = c *E^d
$$

onde:
E: é o esforço aplicado (em pessoas-mês).
T: é o tempo de desenvolvimento (em meses cronológicos).
c: é um coeficiente fornecido pela tabela de Boehm(1981).
d: é um expoente fornecido pela tabela de Boehm(1981).

Para E = 12.31 temos:

$$
T = 2.50*12.31 ^{0.35}
$$

$$
T = 6.02  meses
$$

Para E = 9.59 temos:

$$
T = 2.50* 9.59  ^{0.35}
$$

$$
T = 5.51  meses
$$

A tabela abaixo foi elaborada em equipe de acordo com a tabela de Bohem(1981) que possui os Multiplicadores de Esforço de Desenvolvimento de Software.

| Atributos do produto               |      |
| ---------------------------------- | ---- |
| Confiabilidade exigida do software | 1.00 |
| Tamanho do banco de dados          | 0.94 |
| Complexidade do produto            | 0.85 |

| Atributos do hardware                       |      |
| ------------------------------------------- | ---- |
| Restrição de tempo de execução              | 1.00 |
| Restrição de memoria                        | 1.00 |
| Volatilidade do ambiente de maquina virtual | 0.87 |
| Tempo para completar o ciclo                | 1.00 |

| Atributos do pessoal                       |      |
| ------------------------------------------ | ---- |
| Capacidade do analista                     | 1.00 |
| Experiencia em aplicações                  | 1.13 |
| Capacidade do programador                  | 1.00 |
| Experiencia em maquina virtual             | 1.10 |
| Experiencia com a linguagem de programação | 1.00 |

| Atributos de projeto                    |      |
| --------------------------------------- | ---- |
| Uso de praticas modernas de programação | 0.91 |
| Uso de ferramentas de software          | 0.91 |
| Cronograma exigido do desenvolvimento   | 1.04 |

# 8 - Referências Bibliográficas

EASYBOK. Termo de abertura de projeto. Brasil: Easyhome, 2019. Disponível em: <http://www.easybok.com.br/downloads/easyhome-tap/>
MELLER.Maristela.MODELOS PARA ESTIMAR CUSTOS DE SOFTWARE: ESTUDO COMPARATIVO COM SOFTWARES DE PEQUENO PORTE,2002. Disponível em: <https://repositorio.ufsc.br/xmlui/bitstream/handle/123456789/82351/184841.pdf?sequence=1&isAllowed=y>
