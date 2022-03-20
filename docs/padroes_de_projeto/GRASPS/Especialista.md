# <center> GRASP Especialista


### Histórico de versão<br>


| Data       | Versão | Descrição            | Autor(es)                    |
| ---------- | ------ | -------------------- | ---------------------------- |
| 19.03.2022 | 0.1    | Criação do documento | [Davi Matheus](https://github.com/DaviMatheus)<br>[Natanale Filho](https://github.com/fernandes-natanael) |
| 20.03.2022 | 0.2   | Adição da Metodologia [Davi Matheus](https://github.com/DaviMatheus) |


## Participantes

- [Davi Matheus](https://github.com/DaviMatheus)
- [Natanale Filho](https://github.com/fernandes-natanael)

## Introdução

<p align="justify">&emsp;&emsp;
    Especialista na informação ou apenas Expert ou Especialista é um dos princípios mais básicos dentro dos 9 GRASP’s existentes, em que é uma abordagem genérica que visa atribuir a responsabilidade de fazer ou conhecer algo, assim, basicamente o padrão de projeto Especialista se preocupa em atribuir responsabilidades para alguma entidade.
</p>

<p align="justify">&emsp;&emsp;
    Para essa atribuição é importante seguir um caminho objetivo em que primeiramente é interessante pensar em quais são as informações necessárias para se concluir uma tarefa obrigatória do sistema, após a identificação é preciso avaliar qual é a camada que concentra o maior conhecimento acerca da tarefa em específica. Com os módulos agora mapeados e levantados, aquele que possuir o maior conhecimento da tarefa é o forte candidato para especialista.
</p>


## Metodologia

<p align="justify">&emsp;&emsp;
A partir da definição do padrão, vamos fazer um exemplo analisando a API no backend do projeto do KI-limpinho em que a estrutura de arquivos da pasta pode ser visualizada na próxima imagem.
</p>



<p align='center'>
<img src='..\..\..\assets\img\grasp\especialista.jpeg'>
    <figcaption align='center'>
        <b>Figura 1: Estrutura de arquivos na camada Backend</b>
        <br>
        <small>Autor: Davi Matheus, 2022.</small>
    </figcaption>
</p>



Como evidenciado na imagem, existem arquivos node no padrão do templete do express no diretório e cada um deles possui uma responsabilidade específica. Estes são

- ```auth```, responsável pela a autenticação do projeto, controlando as rotas e os controllers.
- ```helpers```, responsável por ajudar e complementar algumas functios que o sistema percise;
- ```tests```, responsável pela implementação dos testes;
- ```user```, responsável por mapear  e implementar os endpoints e os metodos dos users, como as rotas as models os controlleres e etc;
