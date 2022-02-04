# <center> Product Backlog

### Histórico de Versão
|    Data    | Versão | Descrição            | Autor(es)       |
| :--------: | :----: | :------------------: | :-------------: |
| 30.01.2022 |  0.1   | Criação do documento e versão inicial | Henrique Melo |
| 30.01.2022 |  0.2   | Continuação do doumento e Criação Épico-2 | Davi Matheus|
| 30.01.2022 |  0.2   | Criação Épico-3 | Natanael Filho |
| 31.01.2022 |  0.3   | Criação Épicos 4,5,6,7 e adição de coluna tema | Nilvan Peres |
| 31.01.2022 |  0.4   | Adição dos tópicos introdução, metodologia, resultados e conclusão | Nilvan Peres |
| 03.02.2022 |  0.5   | Refatoração dos requisitos |Lucas Lima e Lucas Melo |

### Responsáveis pelo documento
- Nilvan Peres
- Davi Matheus
- Henrique

### Introdução

<p align="justify">&emsp;&emsp;
    O product backlog é uma das ferramentas essenciais da metologia Scrum, e consiste em uma lista priorizada, contendo todas as funcionalidades/comportamentos desejados para determinada aplicação. Vale ressaltar que, o product backlog está em constante mudanças, com o decorrer do desenvolvimento do projeto o entedimento vai prioridades são alteradas, novas demandas surgem, ou outros comportamentos podem ser descartados, é de suma importância ter o product backlog atualizado para ter uma organização mais otimizada sobre o projeto.[1]
</p>

### Metodologia
<p align="justify">&emsp;&emsp;
    O artefato foi desenvolvido ao longo da sprint 01 e 02, e deverá sofrer alterações ao longo do projeto. A lista de requisitos foram extraídas a partir das seguintes técnicas de elicitações:
    <ul>
        <li>Brainstorm</li>
        <li>Storytelling</li>
        <li>Introspecção</li>
    </ul>
</p>

<p align="justify">&emsp;&emsp;
    Foi determinado abordar os seguintes níveis de granularidade para backlog do projeto:
    <ul>
        <li>Tema</li>
        <li>Épicos</li>
        <li>Features</li>
        <li>História de usuário</li>
        <li>Critérios de aceitação</li>
    </ul>
</p>



### Resultados


<table>
    <thead style="background-color: lightblue">
        <tr>
            <th style="text-align:center">Tema</th>
            <th style="text-align:center">Épico</th>
            <th style="text-align:center">Feature</th>
            <th style="text-align:center">US</th>
            <th style="text-align:center">História de Usuário</th>
        </tr>
    </thead>
    <tbody >
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="17"><b>Lavagem de carro e outros serviços</b></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="5"><a href="./Epicos/EP01/" >Épico 01 - Cadastro e Autenticação de Cliente </a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="1">Cadastro</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US01/" >US01</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como novo usuário do sistema, desejo realizar cadastro no site do lava-jato para ter uma conta.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="3">Login</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US02/" >US02</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como um usuário do sistema, desejo realizar o login na aplicação do lava-jato para ter acesso à todas as funcionalidades.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US03/" >US03</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como um usuário do sistema, desejo visualizar minha senha, para que eu consiga confirmar se digitação está correta.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US04/" >US04</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente do sistema, desejo logar automaticamente quando marcar a opção de lembrar o login.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="1">Logout</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US05/" >US05</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente do sistema, desejo fazer logout da aplicação, para que ninguém acesse minha conta na mesma sessão.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="5"><a href="../Epicos/EP02/" >Épico 02 - Perfil do Usuário </a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Informação do Usuário</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US06/">US06</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo ter uma página de perfil, para que consiga acessar as minhas informações.</td>    
        </tr>
        </tr>
        <tr>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="2">Alterar dados de usuário</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US07/"  >US07</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo editar minhas informações de perfil, para que eu possa atualizar meus dados quando necessário.
        </td>
        </tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US08/"  >US08</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo deletar minha conta, para que todos meus registros sejam apagados.</td>
        </tr>
           <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Forma de Pagamento</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US09/">US09</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo escolher minha forma de pagamento, para que eu possa pagar da maneira que eu preferir.</td>    
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="7"><a href="../Epicos/EP03/" >Épico 03 - Gerenciamento de serviços </a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Agendar serviços</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US10/">US10</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"> Eu, como cliente, desejo agendar um serviço, para que eu possa ter meu carro lavado.</td>    
        </tr>
        </tr>
        <tr>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" >Cancelar serviços</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US11/"  >US11</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"> Eu, como cliente, desejo cancelar um serviço, para que eu possa desmarcar a ação caso eu esteja ocupado ou simplesmente não posso comparecer a data anteriormente agendada.
        </td>
        </tr>
           <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Remarcar um serviço</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US12/">US12</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo remarcar um serviço, para que eu possa obter a lavagem em uma data mais adequada a minha agenda.</td>    
        </tr>
        </tr>
           <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"rowspan="1" >Avaliar um  serviço</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US13/">US13</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo  fazer um comentário sobre determinado serviço para que eu possa deixar um feedback construtivo sobre a lavagem realizada.</td>    
        </tr>
         </tr>
           <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Verificação do serviço</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US14/">US14</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo verificar o status de um determinado serviço agendado/contratado para que eu possa ver de forma detalhada o percursso da lavagem.</td>                
        </tr>
        <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Indicação e sistema de fidelizacão</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US15/">US15</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente, desejo recomendar a aplicação para amigos, para que eu possa receber descontos e brindes.</td>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan=16><b>Gerenciamento do lava jato.</b></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="6"><a href="../Epicos/EP04/" >Épico 04 -  Cadastro e Autenticação de Gerente </a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Cadastro</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US16/" >US16</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"> Eu, como gerente do lava-jato, desejo cadastrar uma conta no site do lava-jato para poder usar a aplicação.</td>
        </tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="4">Login</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US17/" >US17</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"> Eu, como um gerente do sistema, desejo realizar o login na aplicação do lava-jato para ter acesso as funcionalidades que estão disponíveis para mim.</td>
        <tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US18/" >US18</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como um gerente do sistema, desejo login automático quando marco a opção de lembrar login.</td>
        </tr>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US19/" >US19</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como um gerente do sistema, desejo visualizar minha senha para saber se não há erros de digitação.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="1">Logout</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US20/" >US20</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como cliente do sistema, desejo fazer logout, quando desejar sair da aplicação.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="2"><a href="../Epicos/EP05/" >Épico 05 -  Gerenciamento de conta de Gerente </a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="2">Editar conta de gerente</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US21/" >US21</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do lava-jato desejo modificar as minhas informações pessoas registradas na aplicação.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US22/" >US22</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do lava-jato desejo modificar as minhas informações pessoas registradas na aplicação.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="3"><a href="../Epicos/EP06/" >Épico 06 -  Dashboards</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="3">Visualização de dados</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US23/" >US23</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do lava-jato, desejo visualizar um dashboard com a quantidade de serviços contratados/cancelados, para ter mais controle sobre quantidade de serviços prestados</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US24/" >US24</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"> Eu, como gerente do lava-jato desejo visualizar um gráfico com o lucro bruto líquido.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US25/" >US25</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do lava-jato, desejo visualizar um dashboard com o gasto mensal, para análise do negócio.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="2"><a href="../Epicos/EP07/" >Épico 07 -  Sistema de fidelização</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="1">Cupons</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US26/" >US26</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do sistema, desejo cadastrar cupons de descontos, para os clientes conseguirem aplica-los no serviço desejado.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="1">Recompensas</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US27/" >US27</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do sistema, desejo determinar recompensas a partir da quantidade de serviços contratados pelo mesmo cliente, para que os clientes ganhem brindes ou serviços gratuitos.</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="2"><a href="../Epicos/EP08/" >Épico 08 -  Fluxo de caixa</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);" rowspan="2">Despesas</td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US28/" >US28</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do sistema desejo registrar despesas fixas e variáveis(mês).</td>
        </tr>
        <tr>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);"><a href="../User-Stories/US29/" >US29</a></td>
            <td style="vertical-align: middle;text-align:center;border: 0.5px solid rgba(0,0,0,0.2);">Eu, como gerente do sistema desejo listar despesas fixas e variáveis(mês), para ter controle sobre lucro líquido e o fluxo de caixa.</td>
        </tr>
    </tbody>
</table>

### Conclusão

<p align="justify">&emsp;&emsp;
    Apesar do product backlog ser uma lista ordenada e priorizada com todos os requisitos, acredito que o documento está com mais requisitos do que deveria devido ao tempo que será disponibilizado. Entretanto, foi realizado uma matriz de esforço-ganho para determinar quais são os épicos que devem permancer no product backlog até o final da entrega, os épicos mais agregarão valor para o projeto são: E01, E03, E04, E06 E08.
</p>

## Referências

> [1] - Product Backlog. Disponível em : https://www.atlassian.com/agile/scrum/backlogs. Acesso em: 02 de fev. de 2022.

> [2] - Animalesco - Product Backlog. Disponível em: https://unbarqdsw2021-1.github.io/2021.1_G01_Animalesco_docs/#/pages/backlog-do-produto?id=_4-requisitos-funcionais. ACesso em: 02 de fev. de 2022

> [3] - What is product backlog. Disponível em: https://www.scrum.org/resources/what-is-a-product-backlog. Acesso em: 02 de fev. de 2022.

> [4] - Curumim - Prodcut backlog. Disponível em : https://unbarqdsw2021-1.github.io/2021.1_G6_Curumim/product-backlog/. Acesso em: 02 de fev. de 2022.