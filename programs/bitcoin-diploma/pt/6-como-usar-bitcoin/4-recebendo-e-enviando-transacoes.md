# 6.4 Recebendo e Enviando Transações

Uma transação de Bitcoin é uma transferência de propriedade de bitcoin para um novo proprietário. Note que não são as moedas em si que são transferidas, mas sim a propriedade delas: em outras palavras, o direito de gastá-las. Toda vez que uma transação é aceita em um bloco, todos os nós da rede atualizam sua cópia local do livro-razão público para refletir a mudança de propriedade. Nesse sentido, uma transação de Bitcoin se assemelha mais a uma transação imobiliária (ou de outro bem) do que a uma transação em dinheiro.

Para "enviar" bitcoin, o remetente assina uma mensagem com sua chave privada, sinalizando para a rede que o legítimo proprietário do bitcoin transferiu sua propriedade para o destinatário.

O bitcoin agora estará vinculado ao endereço do destinatário, dando a ele a propriedade do bitcoin, de modo que somente o novo proprietário poderá gastá-lo usando sua chave privada.

Novas transações de Bitcoin são iniciadas por carteiras ao redor do mundo, mas não existe um processador de pagamentos central. Em vez disso, os mineradores competem para registrar as transações no livro-razão.

Vamos supor que João deve 0,5 BTC para Mariana e está pronto para pagar a dívida. Ambos possuem carteiras digitais.

1. Mariana compartilha seu endereço com João.
1. João usa o software de sua carteira para criar a transação, que inclui o endereço de Mariana, o valor a ser transferido (0,5 BTC) e uma taxa para o minerador. Taxas mais altas aumentam a probabilidade de um minerador incluir a transação no próximo bloco.
1. Após assinar a transação, ela é transmitida para a rede, onde é verificada pelos nós. Eles verificam se João possui fundos suficientes e se é o legítimo proprietário das moedas que pretende gastar. Caso não seja, a transação é rejeitada imediatamente.
1. Uma vez que a transação é verificada, os mineradores escolhem se vão adicioná-la ao próximo bloco, geralmente com base na taxa selecionada. Assim que a transação entra em um bloco, ela é adicionada à blockchain e os fundos são transferidos para o endereço de Mariana.
1. A propriedade foi transferida para Mariana. Agora ela pode usar sua chave privada para gastar os fundos.

_É importante notar que, uma vez que a transação é concluída, ela não pode ser revertida._


> **Note – Como Funciona uma Transação de Bitcoin**
>
> 1. Alguém solicita uma transação
> 1. Transação transmitida para computadores P2P (nós)
> 1. Mineradores verificam a transação
> 1. Transações combinadas para formar um bloco de dados
> 1. Novo bloco adicionado à blockchain existente
> 1. A transação está concluída



> **Note – Recebendo Transações de Bitcoin**
>
> Para receber bitcoin, você precisará fornecer ao remetente um endereço público de Bitcoin. Este é um conjunto único de letras e números que representa sua carteira e é usado para identificá-la na rede Bitcoin.
>
> Você pode encontrar seu endereço público abrindo sua carteira de Bitcoin e procurando uma opção para “Receber” ou “Depositar” bitcoin.
>
> Você pode então compartilhar seu endereço de Bitcoin de várias formas:
>
> 1. **Copiar e colar o endereço**: Você pode copiar o endereço selecionando-o e pressionando "Copiar", depois colar em um e-mail ou mensagem.
> 1. **Compartilhar um link para sua carteira de Bitcoin**: Algumas carteiras de Bitcoin permitem criar um link para sua carteira que pode ser compartilhado com o remetente. Ele pode então clicar no link para acessar sua carteira e enviar bitcoin.
> 1. **Compartilhar um código QR**: Se o remetente tiver um smartphone com um aplicativo de carteira de Bitcoin instalado, ele pode escanear o código QR para obter seu endereço de Bitcoin.


Assim que o remetente tiver seu endereço, ele pode lhe enviar bitcoin inserindo seu endereço e o valor que deseja enviar. O bitcoin é então enviado da carteira dele para a sua.

A transação é confirmada pela Rede Bitcoin e normalmente leva cerca de 10 minutos. Para maior segurança, recomenda-se aguardar duas confirmações, o que leva cerca de 20 minutos.


> **Note – Enviando Transações de Bitcoin**
>
> Para enviar bitcoin, você precisará de algumas coisas: uma carteira de Bitcoin, o endereço público do destinatário e o valor de bitcoin que deseja enviar.
>
> 1. Abra sua carteira de Bitcoin.
> 1. Vá até o botão “Enviar” e cole o endereço do destinatário no campo "Para". Alternativamente, você também pode escanear o código QR se o destinatário fornecer um.
> 1. Digite o valor de bitcoin que deseja enviar no campo “Valor”.
> 1. Confira o endereço do destinatário e o valor a ser enviado. Lembre-se: as transações são irreversíveis!
> 1. Antes de clicar em “Confirmar e Enviar”, recomendamos que você confira os detalhes da transação mais uma vez para garantir que está enviando o valor correto de bitcoin para o endereço correto.
> 1. Transmita a transação e aguarde a confirmação da rede.
>
> Agora você sabe como avaliar, selecionar e configurar uma carteira de Bitcoin de autocustódia. Enviar e receber bitcoin na rede Bitcoin são chamados de transações “on-chain”. Isso porque as transações ocorrem na rede principal do Bitcoin e são registradas na blockchain.
>
> Transações on-chain são a forma mais segura de transacionar com bitcoin devido à verificação descentralizada fornecida pela rede.
>
> No entanto, transações on-chain são mais lentas e podem ser significativamente mais caras do que outras opções (que discutiremos no Módulo 7) devido à taxa do minerador.


#### Atividade: Transações em Ação

https://qr.myfirstbitcoin.org/transactions.pdf

**Este é um exercício cooperativo que simplifica os papéis básicos das pessoas envolvidas em uma transação de Bitcoin.**

###### Pontos-Chave

1. Existem quatro tipos de participantes em toda transação de bitcoin: o remetente, o destinatário, os mineradores e os operadores de nós.
1. O remetente deve aprovar (assinar criptograficamente) o **valor de bitcoin** a ser enviado E o **endereço específico** para o qual enviar.
1. O destinatário deve fornecer um(a) **endereço válido** ao remetente E verificar se a transação foi confirmada com sucesso na blockchain.
1. Os mineradores garantem que todos os critérios sejam válidos antes de adicionar as transações aos próximos blocos.
1. Os operadores de nós verificam se os blocos minerados são válidos antes de atualizar sua versão da blockchain (o livro-razão).

###### Dica para o estudante

Revezem entre os quatro papéis para experimentar o que cada participante faz.
