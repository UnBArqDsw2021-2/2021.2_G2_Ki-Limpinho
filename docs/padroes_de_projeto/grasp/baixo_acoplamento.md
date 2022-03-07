# <center> `GRASP's` Baixo Acoplamento

### Histórico de Versão
|    Data    | Versão | Descrição            | Autor(es)       |
| :--------: | :----: | :------------------: | :-------------: |
| 07/03/2022 |  0.1   | Criação do Documento | Henrique Melo e Lucas Lima |
| 07/03/2022 |  0.2   | Criação da Introdução | Henrique Melo e Lucas Lima |
| 07/03/2022 |  0.3   | Baixo acoplamento | Henrique Melo e Lucas Lima |


<div align="justify">

## Introdução

GRASP é um acrônimo para **General Responsability Assignment Software Patterns**, que em tradução livre significa **Padrões de Software para Atribuições Gerais de Responsabilidades**. Para a compreensão dos GRASP's, é primeiro necessário a contextualização da abordagem em mais alto nível, esta chamada de **Responsability-Driven-Development**, ou simplesmente **RDD**, que em tradução livre significa **Projeto Guiado por Responsabilidades**.

Larman define que o **RDD** é uma maneira de pensar em projetos de Orientação a Objetos que inclui a abstração de comportamentos entre os diferentes módulos do sistema. O *RDD* é baseado em duas grandes camadas de abstração, a camada de *conhecer*, relacionada com instâncias e comunicações internas do código, e a camada de *fazer*, relacionada com os comportamentos e métodos implementados pelos diferentes módulos. A partir do **RDD**, tem-se que os GRASP's são um conjunto pragmático de princípios básicos que fornecem um referencial sólido para a programação orientada a objetos. [1]

Desta forma, é válido afirmar que os GRASP's buscam oferecer um guia bem estruturado para soluções de software que se baseiam no paradigma da Orientação a Objetos. Como consequência direta da utilização dos padrões dentro de um projeto de software, tem-se a produção de uma base de código robusta e que apresenta um enorme fator de adaptabilidade diante de novas necessidades de projeto, de negócio ou, simplesmente, futuras mudanças planejadas para o código. Um código que segue as diretrizes propostas pelos GRASP's apresenta uma ótima organização entre os diferentes módulos; uma fácil manutenção e, por fim; uma boa capacidade de compreensão por diferentes desenvolvedores. [2]

Os GRASP são descritos pelos seguintes tópicos:

- GRASP Criador;
- GRASP Especialista;
- GRASP da Alta Coesão;
- GRASP do Baixo Acoplamento;
- GRASP Controlador;
- GRASP do Polimorfismo;
- GRASP da Invenção Pura;
- GRASP da Indireção;
- e, por fim, GRASP de Variações Protegidas.

Neste documento, será abordado o tópico **Baixo Acoplamento**.


## Baixo Acoplamento

### Definição

Para definir o princípio do Baixo Acoplamento, antes é preciso definir em termos palpáveis o que é acoplamento: Larman define o acoplamento como uma métrica para mensurar o quão fortemente conectado se encontra o estado de um código específico, isto é, o quão dependente a camada de *conhecer* está entre os diversos componentes do sistema [1]. A partir disso, o princípio do baixo acoplamento fornece a visão necessária para a decisão da melhor forma de implementação que satisfaça:

- a menor dependência entre as classes;
- menor impacto por mudanças em classes existentes;
- maior potencial de reutilização de código.

### Utilização

Ao utilizarmos os padrões já estabelecidos por uma REST API usando express, mongoose em NodeJS(ES6), já estamos utilizando as práticas de Baixo acoplamento, visto que cada um dos arquivos tem sua própria responsabilidade e seus próprios métodos definidos. Desta forma, a própria ferramenta já proporciona um nível adequado de conexão entre os componentes do código e também de modularização e reutilização do código.

## Conclusão

Após todo o conteúdo explicitado neste documento, é possível evidenciar a importância dos padrões de projeto GRASP dentro da construção da base de código do projeto, isto é, é capaz de se identificar quais são as atribuições e responsabilidades de cada um dos componentes presentes no código.

## Bibliografia

- [1] Larman, C. 2005. Applying UML and Patterns – An Introduction to Object-Oriented Analysis and Design and Iterative Development 3rd ed. New Jersey.

- [2] Desenvolvimento com qualidade com GRASP. **DevMedia**. Disponível em <https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704> (Último acesso em 07/03/2022).

- [3] SERRANO, Milene. Arquitetura e Desenho de Software AULA – GRASP – PARTE I. 36 slides <https://aprender3.unb.br/pluginfile.php/897140/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP%20BASE%20Parte%20I%20-%20Profa.%20Milene.pdf> (Último acesso em 07/03/2022).

- [4] SERRANO, Milene. Arquitetura e Desenho de Software AULA – GRASP_A - COMPLEMENTAR – PARTE I. 66 slides https://aprender3.unb.br/pluginfile.php/897140/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP_A%20-%20Profa.%20Milene%20-%20Complementar.pdf> (Último acesso em 07/03/2022).

</div>