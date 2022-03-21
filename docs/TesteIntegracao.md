# <center> Testes de Integração

### Histórico de versão<br>

| Data       | Versão | Descrição            | Autor(es)                    |
| ---------- | ------ | -------------------- | ---------------------------- |
| 20.03.2022 | 0.1 | Criação do documento | [Natanale Filho](https://github.com/fernandes-natanael) |
| 21.03.2022 | 0.2 | Revisão do documento | [Davi Matheus](https://github.com/DaviMatheus)  |

## Participantes

* [Natanael Filho](https://github.com/fernandes-natanael)

## Introdução

&emsp;&emsp;O teste de integração é a fase do teste de software em que módulos são combinados e testados em grupo. Geralmente, sucede à construção dos testes unitários, o que irá variar a partir do contexto do projeto [1]. Basicamente, neles ocorrem as validações dos módulos produzidos anteriormente para o projeto, formando assim um plano de testes num sistema  integrado e preparado para o teste de sistema.

&emsp;&emsp;Além disso, testes de integração se encaixam nos testes de caixa branca, os quais são criados e executados pela equipe de desenvolvimento, requerendo conhecimento da arquitetura interna do projeto. Outro fator é que os testes de integração são importantes, já que agregam valor aos requisitos funcionais do projeto, pois verificam sua integridade, desempenho e confiabilidade, abrindo marguem para o descobrimento e correção de erros de interface entre os componentes do sistema [1].

## Metodologia

&emsp;&emsp;Para a elaboração dos testes de integração da equipe Ki-limpinho, fizemos o uso do Java 11, juntamente do Maven 4.0.0, o qual auxilia na construção das dependências necessárias para os testes funcionarem, como o Framework principal para a elaboração de testes de integração, chamado Rest Assured. Embora comumente os testes de integração sejam feitos após os testes unitários, não há problemas em desenvolverem eles primeiros, na realidade isto se adéqua  ao contexto de cada projeto.

&emsp;&emsp;Rest Assured é um framework utilizado para validar REST API e seus serviços, de modo que independe da linguagem a qual a aplicação e feita [3]. Utilizando o exemplo da Ki-limpinho, feita em Node.JS, temos que o Rest Assured verifica se as requisições e responses com conteúdo do tipo JSON confirmam com o esperado pelo sistema, desse modo, validam se a troca de informações e as requisições http estão ocorrendo de forma correta.

## Resultados

### Tabelas

<div style="position: relative; width: 100%; height: 0; padding-top: 100.0000%;
 padding-bottom: 48px; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
 border-radius: 8px; will-change: transform;">
  <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
    src="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAE7lLlPzFE&#x2F;view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
  </iframe>
</div>

<center>
<a href="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAE7lLlPzFE&#x2F;view?utm_content=DAE7lLlPzFE&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" target="_blank" rel="noopener"> <strong>Figura 1: Tabelas verdades para os testes de integração.</strong>
</a></center>
<center>Autor:  <a href='https://github.com/fernandes-natanael'>Natanel Filho</a>, 2022.</center>

## Referências

> [1] Testes de integração na prática. **Devmedia**. Disponível em: <https://www.devmedia.com.br/teste-de-integracao-na-pratica/31877#1>. Acesso em 20, mar de 2022.

> [2] Códigos de status de respostas HTTP. **Mozzila Developer**. Disponível em: <https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status>. Acesso em 20, mar de 2022.


> [3] **Rest Assured**. Disponível em: <https://rest-assured.io/>. Acesso em 20, mar de 2022.


