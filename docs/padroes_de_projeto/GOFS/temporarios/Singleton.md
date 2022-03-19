
|Data | Versão | Descrição | Autor(es)|
| :--: | :--: | :--: | :--: |
| 16.03.2022 | 0.1.1 | Adição do singleton | [Natanael Filho](https://github.com/fernandes-natanael) |
| 19.03.2022 | 0.1.2 | Revisão do documento | [Jonathan Jorge](https://github.com/Jonathan-Oliveira) |

## Singleton

&emsp;&emsp;Vemos que no Design Pattern o padrão Singleton possui uma peculiaridade, a qual seria a existência de um atributo estático  na classe que instância a própria classe, mas quais as vantagens para está pratica? Simplificando, classes públicas podem ser instâncias N vezes, logo é possível criar inúmeros objetos. Então, para aplicar o Singleton declaramos o construtor de uma classe como pública, e adicionamos uma variável estática, a qual limitará a criação de instâncias da classes.

&emsp;&emsp;Portanto, Singleton será usado quando a aplicação exigir a existência de uma única instância de uma classe, além disso, o acesso desta instância deverá ser através de um ponto bem conhecido.

&emsp;&emsp;Algumas vantagens da aplicação do Singleton:

- Acesso controlado a uma instância única.
- Menos variáveis globais para armazenar instâncias únicas.
- Permite um número variável de instâncias (alterando o padrão para controlar esse número).

&emsp;&emsp;Atualmente em nosso projeto esse padrão poderá ser aplicado na classe [Gerente](/DiagramaDeClasses). Para a aplicação é interessante exista apenas uma instância de gerente, pois assim evita-se a instância vários gerentes externos que não sejam o próprio gerente.

&emsp;&emsp;Segue um exemplo simplificado em Java de uma estrutura no padrão Singleton:

```java
class Gerente{
    protected Gerente instanceGerente;

    private Gerente() {}

    public static getInstanceGerente() {
        if (!instanceGerente) {
            this.instanceGerente = new Gerente();
        }
        return this.instanceGerente;
    }
}

```

## Referências

> [1] **Single Pattern**. Departamento de Informática, UFMA, Maranhão. Disponível em: <http://www.deinf.ufma.br/~vidal/singleton.pdf>. Acesso em 16, mar de 2022.