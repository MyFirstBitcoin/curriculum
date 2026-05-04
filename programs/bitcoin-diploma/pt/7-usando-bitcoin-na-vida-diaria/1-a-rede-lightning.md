# 7.1 A Rede Lightning

A Lightning Network é um sistema de pagamentos que permite aos usuários enviar e receber bitcoin de forma rápida e barata. Ela funciona criando uma carteira compartilhada onde ambas as partes depositam parte de seus bitcoins. Assim, podem realizar transações ilimitadas entre si sem precisar registrar cada uma delas na blockchain principal. Dessa forma, evitam a necessidade de verificar e incluir cada transação em um bloco, tornando o processo mais rápido e econômico. As taxas mais baixas permitem que a Lightning Network seja usada para pequenos pagamentos, que nem sempre são viáveis na blockchain. Quando as partes decidem encerrar a colaboração, apenas o saldo final é registrado na blockchain.

Imagine um dia trabalhando em um café. Pretendendo ficar um tempo, você abre uma comanda e faz um pagamento antecipado, em vez de pagar por cada pedido. No final do dia, você e o dono do café conferem a comanda para acertar a conta. Se o seu depósito for maior do que você gastou, você recebe a diferença de volta; se gastou mais, paga o que ainda deve.

Esse esquema pode ser ampliado para incluir mais participantes. Por exemplo, em uma de suas visitas ao café, você leva um amigo que o atendente não conhece e, por isso, não pode abrir uma comanda. Você oferece ao seu amigo a sua própria comanda para cobrir as despesas dele, e combinam que ele irá te reembolsar depois. Agora imagine milhares de pessoas fazendo o mesmo ao mesmo tempo, permitindo que outros usem comandas já existentes para se conectar com ainda mais pessoas — é assim que a Lightning Network funciona!

Com a Lightning, você pode fazer pagamentos para qualquer pessoa na rede, não apenas para quem você compartilha uma comanda direta — desde que exista uma rota entre as duas partes. Seu pagamento pode percorrer a rede até chegar ao destino, mesmo que você não tenha um canal aberto diretamente com o destinatário.

Vamos dar uma olhada na diferença entre transações on-chain e off-chain.

##### Transações On-Chain

Essas são transações que acontecem diretamente na blockchain do Bitcoin. Elas levam cerca de 10 minutos para serem confirmadas, e as taxas dependem do tamanho da transação em bytes virtuais. São mais seguras, porém mais lentas, pois exigem o consenso da rede.

##### Transações na Lightning Network

Essas transações acontecem em uma rede separada construída sobre a blockchain do Bitcoin. Elas são liquidadas mais rapidamente e com taxas menores. São geralmente usadas quando fatores como velocidade e custo das transações são mais importantes. Comparadas às transações on-chain, são menos seguras.


|  | Rede Bitcoin | Lightning Network |
| --- | --- | --- |
| Definição | Uma rede digital descentralizada que utiliza criptografia para proteger transações financeiras. | Um protocolo de pagamento de segunda camada que opera sobre a blockchain do Bitcoin, permitindo transações mais rápidas e baratas. |
| Vantagens | Descentralizada e segura. Sem estornos ou fraudes. Pode ser usada de forma pseudônima. Aceitação global. | Transações mais rápidas e baratas. Maior escalabilidade. Transações off-chain não congestionam a blockchain. |
| Desvantagens | Transações lentas. Taxas altas para certos tipos de transações. Complexidade para iniciantes. | Pode exigir confiança nos operadores dos canais. Requer uma transação on-chain para abrir e fechar canais. |
