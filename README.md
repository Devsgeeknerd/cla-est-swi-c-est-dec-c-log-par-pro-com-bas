<!-- Título -->
# Estrutura `switch()` — Teoria em C

***Conteúdo da Aula:***

Assim como vimos na estrutura `escolha-caso` no *Scratch*, nós temos o equivalente em **C**:

* Estamos falando do `switch()`.
* Esta estrutura permite verificar o valor de uma variável dentro de uma série de possíveis valores.

A variável na estrutura `switch()` deve ser de tipos simples, normalmente `char` ou `int`.

Depois de avaliar a expressão, o seu valor será comparado com as condições do case.

Se houver algum valor que satisfaça a condição, o comando referente a ela será executado.

Opcionalmente, podemos ter o bloco `default`.

Este bloco será executado quando o valor da variável a ser analisada pelo `switch()` não corresponde a nenhum dos casos detalhados.

Podemos afirmar que a sintaxe do `switch()` é a descrita abaixo:

```c
switch(<variável a ser analisada>) {
    case <1° valor possível>:
        // Comandos a serem realizados quando a variável tiver este valor.
        break;
    case <2° valor possível>:
        // Comandos a serem realizados quando a variável tiver este valor.
        break;
    //...
    case <n-ésimo valor possível>:
        // Comandos a serem realizados quando a variável tiver este valor.
        break;
    [default:
        // Comandos a serem realizados quando nenhum caso for executado.
        break;]
}
```

Vamos imaginar que o usuário deverá responder se ele é maior de idade para o nosso software:

* Caso ele pressione a tecla **“S”**, deveremos escrever a mensagem **“Usuário maior de idade”**;
* Se o usuário pressionar **“N”**, deveremos escrever a mensagem **“Usuário menor de idade”**.
* Caso nem as teclas **“S”** ou **“N”** sejam pressionadas, deveremos escrever a mensagem **“Opção inválida”**.
* Nós podemos implementar este algoritmo utilizando o `switch()`.

Ele ficaria da seguinte forma:

```c
char opcao;
printf("Usuário, você é maior de idade?");
scanf("%s", &opcao);
switch (opcao) {
    case ‘S’:
        printf("Usuário maior de idade");
        break;
    case ‘N’:
        printf("Usuário menor de idade");
        break;
    default:
        printf("Opção inválida");
        break;
}
```

Perceba que nós utilizamos um comando novo, o `break`.

Este comando é utilizado para informar que o bloco do que deve ser executado dentro de cada caso foi finalizado.

<!-- Informações -->
## &#8505; Informações

![Visitors](https://api.visitorbadge.io/api/visitors?path=Devsgeeknerd%2Fcla-est-swi-c-est-dec-c-log-par-pro-com-bas&label=Visitantes&labelColor=%23700070&labelStyle=none&countColor=%23000fff&style=plastic&color=%23ffffff "Total de Visitantes")
&nbsp;
![Followers](https://img.shields.io/github/followers/Devsgeeknerd?style=p&label=Seguidores&labelColor=800080&color=000fff "Total de Seguidores")
&nbsp;
![Watchers](https://img.shields.io/github/watchers/Devsgeeknerd/cla-est-swi-c-est-dec-c-log-par-pro-com-bas?style=p&label=Observadores&labelColor=800080&color=000fff "Total de Observadores")
&nbsp;
![Stars](https://img.shields.io/github/stars/Devsgeeknerd/cla-est-swi-c-est-dec-c-log-par-pro-com-bas?style=p&label=Estrelas&labelColor=800080&color=000fff "Total de Estrelas")
&nbsp;
![Forks](https://img.shields.io/github/forks/Devsgeeknerd/cla-est-swi-c-est-dec-c-log-par-pro-com-bas?style=p&label=Bifurcações&labelColor=800080&color=000fff "Total de Bifurcações")
&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/Devsgeeknerd/cla-est-swi-c-est-dec-c-log-par-pro-com-bas?style=p&label=Tamanho&labelColor=800080&color=000fff "Tamanho do Repositório")
&nbsp;
![License](https://img.shields.io/github/license/Devsgeeknerd/cla-est-swi-c-est-dec-c-log-par-pro-com-bas?style=p&label=Licença&labelColor=800080&color=000fff "Licença do Repositório")
