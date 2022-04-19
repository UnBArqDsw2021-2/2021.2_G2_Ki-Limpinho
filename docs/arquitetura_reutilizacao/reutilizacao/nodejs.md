# <center> Reutilização Node.JS

## Histórico de Versão<br>

|    Data    | Versão |       Descrição       |                      Autor(es)                       |
| :--------: | :----: | :-------------------: | :--------------------------------------------------: |
| 17.04.2022 |  0.1   | Abertura do documento |    [Nilvan Peres](https://github.com/NilvanPeres)    |
| 18.04.2022 |  0.2   |        Revisão        | [Yuri Alves Bacarias](https://github.com/yuriAlves5) |

## Participantes

-   [Nilvan Peres](https://github.com/NilvanPeres)

## Introdução

&emsp;&emsp;A reutilização de software é chamado de reutilização de código. Ela se baseia no uso de conceitos, produtos ou soluções previamente elaboradas ou adquiridas para criação de um novo software, visando melhorar significativamente a qualidade e a produtividade.[1]

&emsp;&emsp;Reusar um produto significa poder reusar partes de um sistema desenvolvido anteriormente como: especificações, módulos de um projeto, arquitetura e código fonte. A principal motivação para a reutilização está relacionada ao aumento dos níveis de qualidade e produtividade no desenvolvimento de software. Sendo assim, estaremos apresentando o conceito de reutilização do NodeJS.

## Resultados

&emsp;&emsp;O Node.JS pode ser definido como um ambiente de execução javascript, focado no server-side. Esssa ferramenta é muito utilizada por conta de sua escabilidade além de possuir uma arquitetura simples e flexível. Outro fator de destaque é que a execução Node.JS é feita de forma single-thread, isso permite que não haja preocupação com processos que não são necessários.

&emsp;&emsp; A reutilização do Node.JS ocorre de várias formas no projeto, como: reutilização de ferramentas e bibliotecas, por exemplo a variável [paramValidation](https://github.com/UnBArqDsw2021-2/2021.2_G2_Ki-Limpinho_Backend/blob/develop/server/user/user.route.js) que é responsável pela validação dos campos das requisições de acordo com as models das entidades, que é utilizada em lugares diferentes no código, a extensão do código ocorre de forma simples, pois para adicionar um novas restrições basta ir no arquivo [param-validation.js](https://github.com/UnBArqDsw2021-2/2021.2_G2_Ki-Limpinho_Backend/blob/develop/config/param-validation.js) e criar um novo objeto definindo quais são os parâmetros que serão validados daquele endpoint. No mesmo arquivo do user.route.js pode ser encontrado um exemplo middleware que pode ser utulizado em qualquer rota do projeto.

## Referências

> [1] **Reutilização de software**. Disponível em: <https://www.devmedia.com.br/reutilizacao-de-software-revista-engenharia-de-software-magazine-39/21956#:~:text=A%20reutiliza%C3%A7%C3%A3o%20de%20software%20se,a%20qualidade%20e%20a%20produtividade.>. Acesso em 17, abril de 2022.

> [2] **About Node.js**. Disponível em: <https://nodejs.org/en/about/>. Acesso em 17, abril de 2022.

> [3] **Animalesco**. Disponível em: <https://unbarqdsw2021-1.github.io/2021.1_G6_Curumim/arquitetura-reutilizacao/reutilizacao/#nodejs> . Acesso em 17, abril de 2022.
