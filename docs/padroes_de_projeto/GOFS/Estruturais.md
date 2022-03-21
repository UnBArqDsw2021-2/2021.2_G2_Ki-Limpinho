## Proxy


<p align="justify">&emsp;&emsp;
O  padrão Estrutural  Proxy  permite a encapsulação de um objeto através de um outro caso ele possui a mesma interface, de forma que o segundo objeto, conhecido como “Proxy”, controla o acesso ao primeiro, que é o objeto real,assim sendo, o proxy é algo que fica no meio do caminho entre a chamada do objeto e o próprio objeto.
</p>


<p align='center'>
    <img src='..\..\..\assets\img\grasp\proxy.jpeg'>
    <figcaption align='center'>
        <b>
            <a href='..\..\..\assets\img\grasp\proxy.jpeg'>
               Figura 1. Diagrama do padrão Proxy
            </a>
        </b>
        <br>
        <small>Fonte:<a href='https://www.devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066'>DevMedia Padrão GOF-Proxy</a></small>
    </figcaption>
</p>

<p align="justify">&emsp;&emsp;
    <li><b>Vantagens:</b> </li>
        <ol>
            <li>Permite deixar transparente o local (endereço) do objeto real. O cliente não precisa conhecer se o objeto é remoto ou não, este tipo de proxy é conhecido como Remote Proxy. [1] </li>
            <li>Útil para realizar otimizações, como cache de objetos.</li>
            <li>Pode ser implementado rotinas de logs e controle de acesso (segurança). Este tipo de proxy é conhecido como Virtual Proxy.</li>
</p>


## Referências

> [1] Conheça o Pattern Proxy - GoF (Gang of Four) Disponível em : <https://www.devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066>. Acesso em 20, mar de 2022.