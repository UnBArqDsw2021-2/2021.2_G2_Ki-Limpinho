# <center> Prototype

### Histórico de versão<br>

| Data       | Versão | Descrição            | Autor(es)  |
| ---------- | ------ | -------------------- | ---------- |
| 16.03.2022 | 0.1    | Criação do documento | [Peniel Etèmana](https://github.com/zpeniel09) |

### Participantes

- Peniel Etèmana 

### Introdução

<p align="justify">&emsp;&emsp;
GoFs Criacionais são padrões que fornecem vários mecanismos de criação de objetos, que aumentam a flexibilidade e a reutilização do código existente. 

Permitem, nesse caso, usar mecanismos/recursos para facilitar tanto a incorporação de novos algoritmos para 
novos contextos quanto a seleção de qual algoritmo usar dado um contexto.

Entre os principais GoFs criacionais temos o Prototype,é um padrão de design criacional que permite copiar objetos existentes sem tornar seu código dependente de suas classes

</p>

### Metodologia

<p>
    O Prototype faz a criação de novos objetos, mas ao invés de criar objetos com valores não inicializados, ele cria objetos através da cópia dos valores de um protótipo. 
</p>

<p>
    Esse padrão nos permitirá copiar objetos existentes sem que essa parte do código tenha dependência em classes. Quando quisermos criar um objeto igual, não precisamos acionar essas classes, basta fazer a exata cópia do objeto já criado.
</p>