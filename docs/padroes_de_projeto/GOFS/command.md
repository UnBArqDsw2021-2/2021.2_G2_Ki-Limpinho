# <center> Design Sprint

### Histórico de versão<br>

| Data       | Versão | Descrição            | Autor(es)  |
| ---------- | ------ | -------------------- | ---------- |
| 15.03.2022 | 0.1    | Criação do documento | Lucas Melo |

### Participantes

- Lucas Melo

### Introdução

<p align="justify">&emsp;&emsp;
No pattern Command, uma operação é encapsulada como um objeto de comando e passada para o objeto invocador. O objeto invocador passa o comando para o objeto correspondente, que executa o comando.

O padrão de comando encapsula ações como objetos. Nesse padrão temos uma uma pilha de comandos sempre que um comando é executado e enviado para a mesma.

</p>

### Metodologia

<p align="justify">&emsp;&emsp; 
    O documento foi construido baseado na 
</p>

### Resultados

<p align="justify">&emsp;&emsp;
   
Um exemplo de aplicação do pattern command é em um componente Wizard, que apresenta várias páginas de configuração para uma única ação que acontece apenas quando o usuário clica no botão "Concluir" na última página. Nesses casos, uma maneira natural de separar o código da interface do usuário do código do aplicativo é implementar o assistente usando um objeto de comando.
</p>

<p align="justify">&emsp;&emsp;
Dessa forma, o objeto de comando é criado quando o componente Wizard é exibido pela primeira vez. Cada página do assistente armazena suas alterações de GUI no objeto de comando, para que o objeto seja preenchido à medida que o usuário progride.. Dessa forma, a classe de comando funcionará. [1]
</p>

<p align='center'>
    <img src='../../../assets/img/padroes/command-example.png'>
    <figcaption align='center'>
        <b>Exemplo código Wizard component - React</b>
        <br>
        <small>Autor: Lucas Melo, 2022.</small>
    </figcaption>
</p>

## Referências

> [1] WIKIPEDIA CONTRIBUTORS. Command pattern. Disponível em: <https://en.wikipedia.org/wiki/Command_pattern>. Acesso em: 15 mar. 2022.

> [2] AND, A. Learning Python Design Patterns - Second Edition. Disponível em: <https://www.oreilly.com/library/view/learning-python-design/9781785888038/ch07s04.html>. Acesso em: 16 mar. 2022.

‌
