# <center> GRASP Especialista


### Histórico de versão<br>


| Data       | Versão | Descrição            | Autor(es)                    |
| ---------- | ------ | -------------------- | ---------------------------- |
| 19.03.2022 | 0.1    | Criação do documento | [Davi Matheus](https://github.com/DaviMatheus)<br>[Natanale Filho](https://github.com/fernandes-natanael) |
| 20.03.2022 | 0.2   | Adição da Metodologia | [Davi Matheus](https://github.com/DaviMatheus) |
| 20.03.2022 | 0.2   | Correção e melhorias do documento | [Natanale Filho](https://github.com/fernandes-natanael) |


## Participantes

- [Davi Matheus](https://github.com/DaviMatheus)
- [Natanale Filho](https://github.com/fernandes-natanael)

## Introdução

&emsp;&emsp;Especialista na informação, ou apenas Expert, é um dos princípios básicos dentre os 9 GRASP’s existentes, em que visa uma abordagem genérica que atribui a responsabilidade de fazer ou conhecer algo, assim, basicamente o padrão de projeto Especialista se preocupa em atribuir responsabilidades para entidade do projeto.

&emsp;&emsp;Primeiramente, para esta atribuição é importante seguir um caminho objetivo onde  defini-se quais são as informações necessárias para se concluir uma tarefa obrigatória do sistema. Após a identificação é preciso avaliar qual é a camada que concentra o maior conhecimento acerca da tarefa em específica. Ao fim, com os módulos mapeados e levantados, aquele que possuir o maior conhecimento da tarefa é o forte candidato para especialista.


### Aplicação

&emsp;&emsp;A partir da definição do padrão, trazemos como exemplo analisado a API do Backend do projeto Ki-Limpinho.


<center>
<img src='..\..\..\assets\img\grasp\especialista.jpeg'>
    <figcaption align='center'>
        <b>Figura 1: Estrutura de arquivos na camada Backend</b>
        <br>
        <small>Autor: Davi Matheus, 2022.</small>
    </figcaption>
</center>



Na figura anterior, vemos que o projeto é feito em node.js e evidenciamos que os especialistas são separados em diretórios, onde cada um possuem arquivos característicos para as suas respectivas funções, sendo elas:

- ```auth```, responsável pela a autenticação do projeto, controlando as rotas e os controllers.
- ```helpers```, responsável por ajudar e complementar algumas functios que o sistema percise;
- ```tests```, responsável pela implementação dos testes;
- ```user```, responsável por mapear  e implementar os endpoints e os metodos dos users, como as rotas as models os controlleres e etc;
