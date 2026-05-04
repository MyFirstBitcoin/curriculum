# 7.4 Enviando e Recebendo Transações Lightning

Com uma carteira Lightning, usar Bitcoin é rápido, barato e privado, tornando as transações entre duas pessoas fáceis. Você pode enviar e receber bitcoin rapidamente para coisas do dia a dia, como comprar um café.

Vamos ver alguns exemplos da Lightning Network em ação.

###### Exemplo 1

Tanto Marcia quanto Eve têm 5 unidades de moeda. Marcia quer enviar 2 unidades para Eve. O pagamento passa por Jeff, que ajuda a encaminhar o pagamento pela Lightning Network. Após a conclusão do pagamento, Eve fica com 7 unidades e Marcia com 3.

Jeff ajuda a rotear o pagamento, mas ele não pode roubar os fundos. A Lightning Network usa criptografia para garantir que apenas o destinatário pretendido possa receber o pagamento. Jeff simplesmente ajuda o pagamento a passar pela rede.

Isso mostra uma vantagem chave da Lightning Network: as pessoas podem enviar pagamentos rapidamente sem precisar confiar em intermediários como bancos.

Operadores de nós como Jeff também podem ganhar pequenas taxas por ajudar a rotear pagamentos. Ao fazer isso, eles ajudam a rede a permanecer descentralizada e eficiente.

Comparado às transações normais de Bitcoin:

* **Transações on-chain** acontecem diretamente na blockchain do Bitcoin. Elas são muito seguras, mas podem ser mais lentas e caras.
* **Transações Lightning** acontecem off-chain e permitem que os pagamentos sejam feitos muito mais rápido e a um custo muito menor.

Por isso, a Lightning é útil para pagamentos pequenos e do dia a dia, enquanto as transações on-chain geralmente são usadas para transferências maiores ou armazenamento de longo prazo.

###### Exemplo 2

Mina adora comer fora e costuma parar em seu café local favorito. Com tantas opções de pagamento diferentes disponíveis, ela não tem certeza de qual é a melhor escolha. Felizmente, ela aprendeu um pouco sobre Bitcoin e a Lightning Network. Depois de analisar suas opções, Mina percebe que usar o método de pagamento Lightning é a melhor opção.

Mina quer comprar um café, mas pagar com uma transação normal de Bitcoin pode, às vezes, demorar e exigir taxas mais altas. Em vez disso, ela decide usar a Lightning Network.

A Lightning Network permite que as pessoas enviem bitcoin instantaneamente e com taxas muito baixas. Isso a torna ideal para pequenas compras do dia a dia, como café.

Para começar a usar a Lightning, Mina baixa uma carteira Lightning em seu celular. Em seguida, ela envia um pouco de bitcoin de sua carteira Bitcoin normal para sua carteira Lightning. Esta etapa usa uma transação normal de Bitcoin na blockchain. Uma vez que os fundos estão em sua carteira Lightning, eles podem ser usados na Lightning Network.

Agora Mina pode pagar o café instantaneamente usando a Lightning. O pagamento acontece fora da blockchain principal do Bitcoin, por isso é muito mais rápido e barato do que uma transação on-chain normal.


| Benefícios | Lightning Network | Sistema Bancário Tradicional |
| --- | --- | --- |
| Velocidade | Rápido | Lento |
| Transparência | Transparente | Opaco |
| Segurança | Seguro | Vulnerável |
| Taxas de transação | Baixas | Altas |
| Inclusão financeira | Alta | Limitada |
| Escalabilidade | Alta | Baixa |
| Privacidade | Alta | Moderada |
| Interoperabilidade | Alta | Baixa |
| Conformidade legal | Moderada | Alta |
| Custo-benefício | Alta | Moderada |


Transações on-chain acontecem diretamente na blockchain do Bitcoin e podem levar mais tempo e ter taxas mais altas. Transações Lightning acontecem off-chain, permitindo pagamentos rápidos e de baixo custo, ainda utilizando bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Capacidade de 65.000 transações por segundo. | Capacidade de 7 transações por segundo. | Capacidade de milhões de transações por segundo. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Este é um mapa de toda a Lightning Network. Graças a milhares de operadores de nós Lightning, você pode enviar sats para qualquer usuário com uma carteira Bitcoin Lightning, onde quer que ele esteja no mundo. O pagamento chegará em poucos segundos e custará apenas alguns centavos.**Veja por si mesmo!**

#### Atividade: Corrida de Revezamento Lightning

https://qr.myfirstbitcoin.org/lightning.pdf

**Este é um exercício prático onde os alunos enviam e recebem sats reais usando a Lightning Network.**

###### Pontos-chave

1. Usar uma carteira Lightning aumentará sua confiança para receber e enviar sats reais.
1. Preste atenção às unidades. Algumas carteiras permitem que os usuários enviem bitcoin OU sats (1/100.000.000 de um bitcoin).
1. Pagamentos via Lightning às vezes podem ficar presos no roteamento, especialmente para valores maiores. Embora seja possível, esse tipo de experiência está se tornando menos comum à medida que a rede amadurece.

###### Dica para o estudante

Verifique com seu instrutor se e como as taxas atuais de transação on-chain do Bitcoin vão impactar a carteira Lightning específica que você usa.
