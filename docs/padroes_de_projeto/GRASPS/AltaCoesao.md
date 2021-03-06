# <center> Alta Coesão

### Histórico de versão

| Data       | Versão | Descrição                        | Autor(es)                   |
| ---------- | ------ | -------------------------------- | --------------------------- |
| 11.03.2022 | 0.1    | Criação do documento             | [Caio Martins](https://github.com/linktocaio) <br>[Yuri Alves](https://github.com/yuriAlves5) |
| 11.03.2022 | 0.2    | Adição da introdução padronizada | [Caio Martins](https://github.com/linktocaio) <br>[Yuri Alves](https://github.com/yuriAlves5) |
| 11.03.2022 | 0.3    | Adição da definição              | [Caio Martins](https://github.com/linktocaio) <br>[Yuri Alves](https://github.com/yuriAlves5) |
| 11.03.2022 | 0.4    | Adição da utilização              | [Caio Martins](https://github.com/linktocaio) <br>[Yuri Alves](https://github.com/yuriAlves5) |
| 11.03.2022 | 0.5    | Adição da conclusão              | [Caio Martins](https://github.com/linktocaio) <br>[Yuri Alves](https://github.com/yuriAlves5) |
| 13.03.2022 | 0.6    | Revisão do documento             | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |
| 15/03/2022 |  0.4   | Padronização Parágrafos | [Nilvan Peres](https://github.com/NilvanPeres) |


### Participantes

* [Caio Martins](https://github.com/linktocaio)
* [Yuri Alves](https://github.com/yuriAlves5)

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

Neste documento, será abordado o tópico **Alta Coesão**.

### Alta Coesão

### Definição

&emsp;&emsp; Alta coesão é um principio avaliativo que prega a divisão de responsabilidades entre as classe. Isso é, uma classe coesa é aquela que lhe foi delegada apenas as suas responsabilidades que estão fortemente relacionadas e altamente focadas. Classes com baixa coesão frequentemente são de difícil compreensão, difíceis de se reutilizar, manter ou alterar.

### Utilização

&emsp;&emsp; Utilização da alta coesão deve estar presente durante todo o projeto para garantir que cada classe possua um única responsabilidade, dessa forma deixando-a entendível, reutilizável e enxuta. Dessa maneira tornando as interfaces de comunicação mais claras, enquanto deixa as classes mais legíveis e amigáveis a expansões e alterações mantendo a complexidade gerenciável.

## Conclusão

&emsp;&emsp; Com o presente documento é possível demonstrar a importância dos padrões de projeto GRASP dentro da construção da base do código, isto é, ser capaz de se identificar quais são as atribuições e responsabilidades de cada um dos componentes presentes.

## Referências

> [1] Larman, C. 2005. Applying UML and Patterns – An Introduction to Object-Oriented Analysis and Design and Iterative Development 3rd ed. New Jersey.

> [2] Desenvolvimento com qualidade com GRASP. **DevMedia**. Disponível em: <https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704> (Último acesso em 11/03/2022).

> [3] SERRANO, Milene. Arquitetura e Desenho de Software AULA – GRASP – PARTE I. 36 slides. Disponível em: <https://aprender3.unb.br/pluginfile.php/897140/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP%20BASE%20Parte%20I%20-%20Profa.%20Milene.pdf> (Último acesso em 11/03/2022).

> [4] SERRANO, Milene. Arquitetura e Desenho de Software AULA – GRASP_A - COMPLEMENTAR – PARTE I. 66 slides. Disponível em: <https://aprender3.unb.br/pluginfile.php/897140/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP_A%20-%20Profa.%20Milene%20-%20Complementar.pdf> (Último acesso em 11/03/2022).
