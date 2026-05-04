# 9.3 Como Funcionam as Transações

Agora que você entende as chaves públicas e privadas, assim como os papéis dos nós e dos mineradores, veja como funciona uma transação de Bitcoin do início ao fim.

1. André quer enviar bitcoin para Gustavo. Ele cria uma transação com o endereço de Gustavo, o valor a ser enviado e uma taxa.
1. André assina a transação com sua chave privada para provar a propriedade.
1. Ele transmite a transação para a rede Bitcoin.
1. Os nós a recebem e verificam se ela segue as regras, incluindo a verificação da assinatura e se André possui bitcoin suficiente.
1. Se for válida, a transação é compartilhada pela rede e adicionada ao mempool, onde as transações pendentes aguardam.
1. Os mineradores escolhem transações do mempool e as incluem em um bloco que tentam minerar.
1. Quando um minerador minera um bloco com sucesso, ele é compartilhado com a rede e verificado por outros nós.
1. Se for válido, o bloco é adicionado ao blockchain. Gustavo recebe o bitcoin.
1. À medida que mais blocos são adicionados, a transação recebe confirmações, tornando-a mais segura.

Uma vez incluída em um bloco, a transação está confirmada. André não pode gastar aquele bitcoin novamente, e Gustavo pode gastar o que recebeu em uma nova transação.


> **Note**
>
> Transação e taxa selecionadas → Assinada pela carteira e enviada → Distribuída pelos nós → Minerador adiciona a transação ao bloco modelo → Minerador vence a prova de trabalho → Novo bloco é validado → Novo bloco é distribuído pelos nós


###### Recursos


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
