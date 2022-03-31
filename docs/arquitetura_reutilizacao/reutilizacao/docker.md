# <center> Reutilização Docker

## Histórico de Versão<br>

|Data | Versão | Descrição | Autor(es)|
| :-:|:-:|:-:|:-: |
| 30.03.2022 | 0.1 | Abertura do documento |[Peniel Etèmana](https://github.com/zpeniel09)|
| 30.03.2022 | 0.2 | Adição de Introdução  |[Peniel Etèmana](https://github.com/zpeniel09)|
| 30.03.2022 | 0.3 | Adição da Metodologia e Resultados  |[Peniel Etèmana](https://github.com/zpeniel09)|
| 30.03.2022 | 0.4 | Finalização do documento com as referências   |[Peniel Etèmana](https://github.com/zpeniel09)|


## Participantes
* [Peniel Etèmana](https://github.com/zpeniel09)

## Introdução

&emsp;&emsp;A reutilização de software é chamado de reutilização de código. Ela se baseia no uso de conceitos, produtos ou soluções previamente elaboradas ou adquiridas para criação de um novo software, visando melhorar significativamente a qualidade e a produtividade. 

&emsp;&emsp;Reusar um produto significa poder reusar partes de um sistema desenvolvido anteriormente como: especificações, módulos de um projeto, arquitetura e código fonte. A principal motivação para a reutilização está relacionada ao aumento dos níveis de qualidade e produtividade no desenvolvimento de software. Sendo assim, estaremos apresentando o conceito de reutilização do Docker.

## Metodologia

&emsp;&emsp;Backend de armazenamento é a parte da solução do Docker que cuida do gerenciamento dos dados. No Docker temos várias possibilidades de backend de armazenamento e à reutilização de software nesse documento foi utilizado o docker no backend a fim de torna mais eficiente o fluxo do nosso projeto.

## Resultados

&emsp;&emsp;O Docker é uma plataforma aberta, criada com o objetivo de facilitar o desenvolvimento, a implantação e a execução de aplicações em ambientes isolados. Foi desenhada especialmente para disponibilizar uma aplicação da forma mais rápida possível. O uso dele permite de gerenciar a infraestrutura da aplicação, isso agilizará o processo de criação, manutenção e modificação do serviço.

&emsp;&emsp;No [backend](https://github.com/UnBArqDsw2021-2/2021.2_G2_Ki-Limpinho_Backend) do nosso projeto, foi configurado um Docker com a versão alpine do Node.js. Essas configurações podem ser melhor visualizadas a partir do Dockerfile do back-end.

&emsp;&emsp;Foi feito o uso do Docker Compose que age, basicamente, como o orquestrador de containers do Docker, organizando e gerenciando as instâncias do Docker utilizadas na aplicação. As configurações do Docker Compose podem ser acessadas pelos documentos: docker-compose.yml do [backend](https://github.com/UnBArqDsw2021-2/2021.2_G2_Ki-Limpinho_Backend). Falando em reutilização de software, o Docker possui uma quantidade significativa de Hot Spots e alguns pontuais Frozen Spots.

* Hot-Spots: são partes específicas de sistemas individuais, projetadas para serem genéricos e adaptáveis.
    * Imagem Docker;
    * Dependências;
    * Comandos;
    * Networking
    * Variáveis de ambiente.

* Frozen-Spots: definem a arquitetura geral do sistema e seus componentes básicos, permanecem fixos em todas as instanciações.
    * Sistema de arquivos,
    * Arquivos necessário.

<p align='center'>
  <img src='https://i.ibb.co/5xfgnks/dockerfile.png'>
  <figcaption align='center'>
        <b>
            <a href='https://i.ibb.co/5xfgnks/dockerfile.png'>
               Figura 1: Dockerfile Backend
            </a>
        </b>   
      <br>
        <small>Autor: <a href='https://github.com/zpeniel09'>Peniel Etèmana</a>, 2022.</small>
  </figcaption>
</p>

<p align='center'>
  <img src='https://i.ibb.co/FW6Kf1z/docker-Compose-File.png'>
  <figcaption align='center'>
        <b>
            <a href="https://i.ibb.co/FW6Kf1z/docker-Compose-File.png">
               Figura 2: Docker Compose Backend
            </a>
        </b>   
      <br>
        <small>Autor: <a href='https://github.com/zpeniel09'>Peniel Etèmana</a>, 2022.</small>
  </figcaption>
</p>

## Referências
> [1] **Reutilização de software**. Disponível em: <https://www.devmedia.com.br/reutilizacao-de-software-revista-engenharia-de-software-magazine-39/21956#:~:text=A%20reutiliza%C3%A7%C3%A3o%20de%20software%20se,a%20qualidade%20e%20a%20produtividade.>. Acesso em 30, março de 2022.

> [2] **Install Docker Compose**. Disponível em: <https://docs.docker.com/compose/install/>. Acesso em 30, março de 2022.

> [3] DOCKER. **Overview of Docker Compose**. Disponível em: <https://docs.docker.com/compose/>. Acesso em 30, março de 2022.

> [4] **Docker**. Disponível em: <https://stack.desenvolvedor.expert/appendix/docker/oquee.html>. Acesso em 30, março de 2022.