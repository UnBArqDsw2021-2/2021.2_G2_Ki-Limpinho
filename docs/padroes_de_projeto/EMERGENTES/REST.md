# <center> Design Sprint

## Histórico de Versão<br>

|Data | Versão | Descrição | Autor(es)|
| :-:|:-:|:-:|:-: |
| 18.03.2022 | 0.1 | Criação do documento | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |

## Participantes

* [Jonathan Jorge](https://github.com/Jonathan-Oliveira)

## Introdução

<p align="justify">&emsp;&emsp;

REST é um acrônimo de Representational State Transfer, que significa Transferência de Estado Representacional. O REST fornece um conjunto de restrições arquitetônicas que, quando aplicadas como um todo, enfatizam a escalabilidade das interações dos componentes, a generalidade das interfaces, a implantação independente dos componentes e os componentes intermediários para reduzir a latência da interação, reforçar a segurança e encapsular sistemas legados (FIELDING; TAYLOR, 2000).
</p>

## Metodologia

<p align="justify">&emsp;&emsp;
Foi realizado uma pesquisa bibliográfica sobre o assunto, para conceituar e para aplicação do REST no projeto foi utilizado a linguagem javascript com o framework react para o front e nodejs para o back.
</p>

## Resultados

### REST

#### Client-Server

<p align="justify">&emsp;&emsp;
O cliente-servidor trata sobre a separação de responsabilidades entre o cliente e o servidor, ou seja, o cliente é responsável pela interface do usuário (User interface) e o servidor é responsável por armazenar os dados no bando de dados. Com isso, permite que os componentes evoluam independentemente, aumentando sua flexibilidade e escalabilidade.
</p>

#### Stateless

<p align="justify">&emsp;&emsp;
Essa restrição implica que a comunicação deve ser naturalmente sem estado, ou seja, cada solicitação que o cliente faz para o servidor deve conter todas as informações necessárias para que o servidor entenda o que é pedido e não pode aproveitar de nenhum contexto armazenado no servidor. O estado da sessão é, portanto, mantido completamente no cliente. O lado negativo é que pode diminuir o desempenho da rede aumentando os dados repetitivos enviados em uma série de solicitações, pois esses dados não podem ser deixados no servidor em um contexto compartilhado, porém a próxima restrição é apresentada justamente para resolver essa questão.
</p>

#### Cache

<p align="justify">&emsp;&emsp;
Para melhorar a eficiência da rede, a restrição de cache exige que os dados em uma resposta a uma solicitação seja rotulados, explicitamente ou implicitamente, como armazenáveis em cache ou não armazenáveis em cache. Se uma resposta puder ser armazenada em cache, um cache do cliente terá o direito de reutilizar os dados da reposta para novas solicitações posteriores, sem necessidade de consultar o servidor. A grande vantagem dessa restrição é que ela têm o potencial de abolir parcialmente ou completamente algumas interações, melhorando a eficiência, a escalabilidade e reduzindo a latência média de uma série de interações. A desvantagem é que os dados armazenados em cache pode divergir dos dados que seriam solicitados diretamente do servidor, o que pode causar problemas de conflito de dados.
</p>

#### Uniform Interface

<p align="justify">&emsp;&emsp;
A interface uniforme é a interoperabilidade entre os componentes cliente e servidor, ou seja, o cliente e servidor compartilham da mesma interface. Para isso foi definido quatros restrições de interface: identificação de recursos; manipulação de recursos por meio de representações; mensagens autodescritivas; e, componentes HATEOAS, ou seja, hipermídia como motor do estado da aplicação.
</p>

#### Layered System

<p align="justify">&emsp;&emsp;
A restrição de sistema em camadas implica que uma arquitetura seja composta de camadas hierárquicas restringindo o comportamento do componente de modo que cada componente possa "ver" além da camada imediata com a qual está interagindo, ou seja, o cliente não deve conectar-se diretamente ao servidor da aplicação, porém uma camada de balanceamento de carga deverá ser acionada para essa responsabilidade. Caso ocorra mudanças em uma delas, as demais não serão impactadas.
</p>

#### Code on demand (opcional)  

<p align="justify">&emsp;&emsp;
O Código sob demanda é a única restrição opcional no REST. Permite aos clientes melhorar a sua flexibilidade porque de fato é o servidor que decide como certas coisas serão feitas. Por exemplo, com o código sob demanda, um cliente pode descarregar um javascript, uma applet java ou mesmo uma aplicação flash a fim de encriptar a comunicação para que os servidores não estejam conscientes de quaisquer rotinas/chaves de encriptação utilizadas neste processo.
</p>
<p align="justify">&emsp;&emsp;
No entanto, a utilização de Code on demand (COD) reduz a visibilidade, razão pela qual esta restrição é opcional. Além disso, nem todas as API necessitam deste tipo de flexibilidade.
</p>

#### REST e HTTP

<p align="justify">&emsp;&emsp;
No REST, a manipulação dos recursos disponibilizados para o cliente é feita por métodos do protocolo HTTP, os quais indica diferentes tipos de operações que o cliente pode realizar para manipulas os dados por requisições para cada contrato disponibilizado. Comumente, os métodos HTTP são utilizados para operações CRUD ( Create, Read, Update e Delete). 
</p>
<p align="justify">&emsp;&emsp;
Cada resposta que uma aplicação REST retorna, é enviado um código definindo o status da requisição e o conteúdo da resposta, a seguir há uma lista com os códigos de status mais utilizados, para visualizar uma lista completa com os códigos de status, clique no link <a href='https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status'>aqui</a>.
</p>
- 200 (OK), requisição atendida com sucesso;
- 201 (CREATED), objeto ou recurso criado com sucesso;
- 204 (NO CONTENT), objeto ou recurso deletado com sucesso;
- 400 (BAD REQUEST), ocorreu algum erro na requisição (podem existir inúmeras causas);
- 404 (NOT FOUND), rota ou coleção não encontrada;
- 500 (INTERNAL SERVER ERROR), ocorreu algum erro no servidor.

<p align="justify">&emsp;&emsp;
Segue uma lista de métodos HTTP com suas respectivas operações :
</p>

- POST: O método POST é utilizado para submeter uma entidade a um recurso específico, frequentemente causando uma mudança no estado do recurso ou efeitos colaterais no servidor.
- GET: O método GET solicita a representação de um recurso específico. Requisições utilizando o método GET devem retornar apenas dados.
- PATCH: O método PATCH é utilizado para aplicar modificações parciais em um recurso.
- PUT: O método PUT substitui todas as atuais representações do recurso de destino pela carga de dados da requisição.
- DELETE: O método DELETE remove um recurso específico.

<p align="justify">&emsp;&emsp;
Usualmente usa-se o método PUT para atualizar parte de um recurso ao invés do PATCH.
</p>

### Aplicação

<p align="justify">&emsp;&emsp;
Segue um exemplo da aplicação do REST no Back-end do Ki-limpinho, feita com Node.Js, onde pode ser visualizado a disponibilização dos principais métodos HTTP utilizados para manipulação de dados do usuário.
</p>

```javascript
const express = require('express');
const validate = require('express-validation');
const paramValidation = require('../../config/param-validation');
const userCtrl = require('./user.controller');

const router = express.Router(); // eslint-disable-line new-cap

router.route('/')
  /** GET /api/users - Get list of users */
  .get(userCtrl.list)

  /** POST /api/users - Create new user */
  .post(validate(paramValidation.createUser), userCtrl.create);

router.route('/:userId')
  /** GET /api/users/:userId - Get user */
  .get(userCtrl.get)

  /** PUT /api/users/:userId - Update user */
  .put(validate(paramValidation.updateUser), userCtrl.update)

  /** DELETE /api/users/:userId - Delete user */
  .delete(userCtrl.remove);

/** Load user when API with userId route parameter is hit */
router.param('userId', userCtrl.load);

module.exports = router;
```

## Conclusão

 Com esse documento podemos ter uma visão geral sobre o REST e como ele é aplicado no backend do  projeto. Evidenciando sua importância para a aplicação.

## Referências

> [1] NOLETO, Cairo. API REST: o que é e como montar uma API sem complicação?. [S. l.], 4 jan. 2022. Disponível em: <https://blog.betrybe.com/desenvolvimento-web/api-rest-tudo-sobre/>. Acesso em: 18 mar. 2022.

> [2] FIELDING, R. T.; TAYLOR, R. N. Architectural Styles and the Design of Network-Based
Software Architectures. Tese (Doutorado), 2000. AAI9980887.

> [3] REST: Conceito e fundamentos. Disponível em: <https://www.alura.com.br/artigos/rest-conceito-e-fundamentos> Acesso em: 18 mar. 2022.

> [4] MDN contributors. Métodos de requisição HTTP. 14 jul. de 2021. Disponível em: <https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Methods> Acesso em: 18 mar. 2022

> [5] Introdução a web services RESTful. Disponível em: <https://www.devmedia.com.br/introducao-a-web-services-wwwrestful/37387> Acesso em: 18 mar. 2022.

> [6] Backend Ki-limpinho. Disponível em: <https://github.com/UnBArqDsw2021-2/2021.2_G2_Ki-Limpinho_Backend/blob/main/server/user/user.route.js> Acesso em: 18 mar. 2022.