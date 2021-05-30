# **Solicitação de Compra**

***```
Menu: Compras -> Solicitação de Compra
```***

---

A **==Solicitação de Compra==** é criada quando se tem a necessidade de comprar algo, mas não tem informação de fornecedor ou preço, apenas se tem o item que precisa, quantidade e data da entrega desejada. 

Na tela inicial da **==Solicitação de Compra==** é possível ver todas que já foram criadas e qual o **Status** de cada uma delas.

![Index Solicitação de Compras](../img/solicitacao_01.png)

!!! Legenda

	=== "Status"
		**:fontawesome-solid-circle:{ .laranja } - Aguardando envio**: Esse **Status** quer dizer que a **==Solicitação de Compra==** está aguardando para ser enviada à fila de integração com *SAP Business One*.

		**:fontawesome-solid-circle:{ .preto } - Aguardando integração**: Esse **Status** quer dizer que a **==Solicitação de Compra==** está na fila de integração com o *SAP Business One*.

		**:fontawesome-solid-circle:{ .azul_status } - Solicitação em Andamento**: Esse **Status** quer dizer que a **==Solicitação de Compra==** entrou no *SAP Business One* e está aguardando a criação de um Pedido de Compra a partir dessa **==Solicitação de Compra==**.

		**:fontawesome-solid-circle:{ .verde } - Solicitação Gerou pedido**: Esse **Status** quer dizer que foi criado um Pedido de Compra a partir dessa **==Solicitação de Compra==**.

		**:fontawesome-solid-circle:{ .vermelho } - Erro**: Esse **Status** quer dizer que o *SAP Business One* gerou algum erro, para saber qual é basta posicionar o cursor em cima do **Status**.

Para conseguir criar uma, basta clicar em **Novo** e na próxima tela é necessário informar quando precisa dos produtos e quais produtos/quantidades são necessários.

![Index Solicitação de Compras](../img/solicitacao_02.png)

Segue informações dos campos:

=== "Cabeçalho"

	*	**Data de Recebimento**: Informar a data necessária para recebimento do produto, essa data será replicada para todas as linhas.

=== "Linhas"

	 *	**Item**: Informar o item que deseja solicitar.
	 *	**Data de Recebimento**: Será informado a mesma data do cabeçalho, mas é possível realizar alterações por item (caso necessário).
	 *	**Quantidade**: Informar a quantidade necessária (lembrando da conversão de medida).
	 *	**Unidade de Medida**: Informar a unidade de medida (Conversão de Caixa 12 UN (CX12UN).
	 *	**Preço**: Se estiver com a configuração marcada, irá aparecer esse campo informando o custo do item.
	 *	**Em Estoque**: Se estiver com a configuração marcada, irá aparecer esse campo informando a quantidade desse item no estoque.
	 *	**Última sincronização**: Se estiver com a configuração marcada, irá aparecer quando foi feito a consulta do estoque no *SAP Business One*.
	 *	**Sub Total**: Cálculo entre Quantidade multiplicando pelo Preço Unitário.
	 *	**Ação**: Excluir a linha.


Para finalizar a **==Solicitação de Compra==** é possível informar uma **Observação** para detalhar alguma informação e depois disso basta clicar em **Salvar**.

![Index Solicitação de Compras](../img/solicitacao_03.png)

Pode acontecer de esquecer de preencher algum campo, com isso o B1Food irá apresentar uma mensagem de erro, segue exemplo:

![Index Solicitação de Compras](../img/solicitacao_13.png)

Caso a **==Solicitação de Compra==** estiver certo irá aparecer uma mensagem de **Registro adicionado com sucesso" e será necessário clicar no botão **Voltar** para ir à página inicial do **==Solicitação de Compra==**.

![Index Solicitação de Compras](../img/solicitacao_04.png)

Será listado a **==Solicitação de Compra==** que acabou de criar e com isso será listado 4 ações para essa **==Solicitação de Compra==**, segue abaixo explicativo de cada uma delas.

![Index Solicitação de Compras](../img/solicitacao_05.png)

=== ":fontawesome-solid-search:{ .search }"
	*	A ação **Visualizar** irá abrir a **==Solicitação de Compra==** para poder avaliar algum item, por exemplo. 
	![Index Solicitação de Compras](../img/solicitacao_06.png){ align=left }

=== ":fontawesome-solid-pen-square:{ .pen }"
	*	A ação **Editar** irá abrir a **==Solicitação de Compra==** para realizar alguma edição.
	![Index Solicitação de Compras](../img/solicitacao_07.png){ align=left }

=== ":fontawesome-solid-check-square:{ .check }"
	*	A ação **Enviar** irá enviar para o *SAP Business One* a criação dessa **==Solicitação de Compra==**.
	![Index Solicitação de Compras](../img/solicitacao_08.png){ align=left }

=== ":fontawesome-solid-window-close:{ .close }"
	*	A ação **Excluir** irá apagar a **==Solicitação de Compra==** criada.
	![Index Solicitação de Compras](../img/solicitacao_09.png){ align=left }

Se você enviou o **==Solicitação de Compra==**, **depende da configuração** do seu B1Food ele pode ter ido direto para integrar com o *SAP Business One* ou ele pode ter entrado na **aprovação**, pode ser que você que faça ela ou outro usuário, mas irei explicar como realizar essa aprovação.

![Index Solicitação de Compras](../img/solicitacao_10.png)

=== ":fontawesome-solid-thumbs-up:{ .aprovar }"
	*	A ação **Aprovar** irá enviar para o *SAP Business One* a criação dessa **==Solicitação de Compra==**.
	![Index Solicitação de Compras](../img/solicitacao_11.png){ align=left }

=== ":fontawesome-solid-thumbs-down:{ .rejeitar }"
	*	A ação **Rejeitar** será necessário informar o **Motivo** que rejeitou, para que o usuário que fez saiba e consiga realizar as devidas alterações para reenviar novamente.
	![Inventario](../img/solicitacao_12.png)

Caso a **==Solicitação de Compra==** for aprovado, ele irá entrar para fila de envio para o *SAP Business One*, durante esse processo o **Status** ficará :fontawesome-solid-circle:{ .preto }, caso der tudo certo o **Status** irá ficar :fontawesome-solid-circle:{ .azul_status } e se der algum erro ao integrar com o *SAP Business One* o **Status** irá ficar :fontawesome-solid-circle:{ .vermelho } e irá apresentar o erro.