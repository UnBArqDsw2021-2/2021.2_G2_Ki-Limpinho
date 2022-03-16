# <center> Controlador

### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| :- | :- |:- | :- |
| 13.03.2022 | 0.1 | Criação do documento              | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |
| 15.03.2022 | 0.2 | Adição no documento               | [Peniel Etèmana](https://github.com/zpeniel09)         |
| 15.03.2022 | 1.0 | Adição dos resultados e conclusão | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) e [Peniel Etèmana](https://github.com/zpeniel09)    |
| 16.03.2022 | 1.0 | Revisão do documento |[Nilvan Peres Costa](https://github.com/NilvanPeres) |

### Participantes

* [Jonathan Jorge](https://github.com/Jonathan-Oliveira)
* [Peniel Etèmana](https://github.com/zpeniel09)

## Introdução

<p align="justify">&emsp;&emsp;No desenvolvimento de um software, é de suma importância a utilização de padrões de projeto. São esses padrões de projeto que definem os princípios e soluções que serão utilizados na criação desse software. GRASP(General Responsibility Assignment Software Patterns) padrões são diretrizes que atribuem responsabilidade a classes e objetos em projetos orientados a objetos.
</p>
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

## Referências

> [1] BOAS, Leandro Vilas. Padrões GRASP - Padrões de Atribuir Responsabilidades. Disponível em: <https://medium.com/@leandrovboas/padr%C3%B5es-grasp-padr%C3%B5es-de-atribuir-responsabilidades-1ae4351eb204>. Acesso em 15, de Março de 2022.

> [2] Universidade Federal de Uberlândia. Padrões GRASP. Disponível em: <http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf>. Acesso em 15, de Março de 2022.

> [3] SERRANO, Milene. Aula - GRASP - PARTE I.

> [4] Controller – Padrões GRASP . Disponível em: <https://www.ramonsilva.net/post/controller-padr%C3%B5es-grasp>. Acesso em 15, de Março de 2022.
