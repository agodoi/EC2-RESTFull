# O que é o NGINX?

Imagine que você é o gerente de uma loja de fast food muito popular, e há apenas uma pessoa na caixa registradora para lidar com todas as encomendas dos clientes. No início, quando a loja está calma, uma pessoa pode ser suficiente. No entanto, quando o horário do almoço chega e há muitos clientes chegando ao mesmo tempo, a fila se forma e o atendente fica sobrecarregado, resultando em atrasos no serviço.

Agora, vamos aplicar o conceito do Nginx nesta situação:

* Proxy Reverso (Atendente da loja): O Nginx age como um atendente dedicado que recebe as solicitações dos clientes. Ele verifica o que os clientes estão pedindo e decide a melhor maneira de lidar com cada solicitação.
  
* Balanceador de Carga (Atendentes adicionais): À medida que mais clientes chegam, o Nginx (o atendente dedicado) percebe que há muitas solicitações para um único atendente (servidor). Ele decide chamar mais atendentes (outros servidores) para ajudar a lidar com a carga aumentada. Ele distribui as solicitações de maneira equilibrada entre os atendentes para garantir que ninguém fique sobrecarregado.
  
* Cache HTTP (Balcão de retirada rápida): O Nginx também pode lembrar dos pedidos recentes dos clientes. Se um cliente pediu algo que está pronto e disponível (conteúdo em cache), o Nginx pode entregar imediatamente, sem a necessidade de pedir ao atendente (servidor de aplicação) para preparar o pedido novamente. Isso economiza tempo e recursos.
  
* Servidor Web (Cozinha): Além disso, o Nginx também pode ser configurado para lidar com a preparação de certos tipos de pedidos. Por exemplo, se um cliente pedir um hambúrguer especial que requer preparação rápida e simples (conteúdo estático), o Nginx pode prepará-lo diretamente e entregá-lo ao cliente, sem a necessidade de envolver os atendentes (servidores de aplicação).
