# **Conciliação de CardService**

***```
Menu: Conciliação -> Conciliação de CardService
```***

---

Esse módulo de **==Conciliação de CardService==** é para clientes que **contrataram integração com CardService** e será utilizado quando existe algum dia que o **estabelecimento não abriu**, com isso é necessário informar o B1Food para habilitar integração de CardService para poder enviar para o SAP Business as vendas e recebimentos de cartões daquele dia.

![Index Conciliacao](../img/conciliacao_cardservice01.png)

Primeiramente é necessário ter a certeza que o dia não teve vendas (pois é um processo sem volta), para ter uma certeza melhor podemos identificar no monitoramento se o dia está em **branco**

![Index Conciliacao](../img/conciliacao_cardservice02.png)

Após essa certeza, basta procurar o dia que deseja habilitar essa conciliação e clicar em **Habilitar integração**

![Index Conciliacao](../img/conciliacao_cardservice03.png)

O B1Food irá te perguntar se tem certeza (só por precaução), e para seguir com o processo é necessário selecionar **Sim**

![Index Conciliacao](../img/conciliacao_cardservice04.png)

Caso der certo, irá apresentar uma mensagem de **Sucesso**

![Index Conciliacao](../img/conciliacao_cardservice05.png)

Após essa **habilitação da integração** o dia já entra na fila da integração para importar as **vendas de cartões** e **recebimento de cartões**

![Index Conciliacao](../img/conciliacao_cardservice06.png)