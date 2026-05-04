# 9.1 Nós e Mineradores de Bitcoin

Os nós do Bitcoin podem parecer algo técnico, mas são simplesmente softwares que mantêm uma cópia do blockchain do Bitcoin em um computador. O blockchain é um registro compartilhado de todas as transações de Bitcoin.

Quando você executa seu próprio nó, você mesmo verifica as transações de Bitcoin em vez de confiar em outra pessoa. Isso lhe dá mais independência e ajuda a manter a rede do Bitcoin descentralizada.

Você pode pensar em um nó do Bitcoin como um agente de trânsito digital com algumas funções importantes.

1. Ele mantém uma cópia do blockchain, que é o histórico de todas as transações de Bitcoin.
1. Os nós se conectam com outros nós ao redor do mundo e compartilham informações. Um exemplo é a lista de novas transações aguardando confirmação, chamada de mempool.
1. Os nós verificam se cada transação segue as regras do Bitcoin. Se uma transação for inválida, o nó a rejeita.

Os nós também ajudam novos nós a entrarem na rede compartilhando o blockchain com eles. No entanto, cada novo nó ainda verifica todas as regras de forma independente.

Qualquer pessoa pode rodar um nó instalando um software como o Bitcoin Core e baixando o blockchain. Depois de configurado, o nó continua recebendo novos blocos aproximadamente a cada 10 minutos e os verifica antes de adicioná-los à sua cópia do blockchain.

Rodar um nó ajuda a tornar a rede do Bitcoin mais segura e descentralizada, pois mais pessoas estão verificando o sistema de forma independente.

#### O que é um nó do Bitcoin?

> O objetivo da mineração não é a criação de novos bitcoin; isso é o sistema de incentivos. A mineração é o mecanismo pelo qual a segurança do Bitcoin é descentralizada.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Os mineradores coletam transações não confirmadas, formam um bloco e usam energia para encontrar uma chave que adiciona e protege o bloco.


Os mineradores competem para adicionar o próximo bloco de transações ao blockchain. Para isso, eles precisam encontrar um número especial que cria um hash de bloco válido. Você pode imaginar isso como procurar a chave certa entre bilhões de possibilidades. O primeiro minerador a encontrar o hash correto vence a corrida e ganha o direito de adicionar seu bloco ao blockchain.

Quando um minerador encontra um hash válido, ele compartilha seu bloco com a rede. Outros mineradores rapidamente verificam se a solução está correta. Se estiver, o bloco é adicionado ao blockchain, ajudando a manter o registro público do Bitcoin seguro.

Os mineradores ganham bitcoin de duas formas:

* **Recompensas de bloco:** Novos bitcoin são criados e dados ao minerador que adiciona com sucesso um bloco ao blockchain.
* **Taxas de transação:** Quando as pessoas enviam bitcoin, elas incluem uma pequena taxa. O minerador que adiciona o bloco recebe as taxas das transações incluídas naquele bloco.

#### Halvings do Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> As recompensas dos mineradores por completar um bloco são reduzidas pela metade a cada 210.000 blocos, aproximadamente a cada quatro anos.


O Bitcoin tem um fornecimento máximo fixo de 21.000.000 de bitcoin, mas nem todos foram criados quando o Bitcoin começou. Em vez disso, novos bitcoin são gradualmente introduzidos em circulação através da **mineração**.

Quando os mineradores adicionam com sucesso um novo bloco de transações à rede do Bitcoin, eles recebem uma **recompensa de bloco** em bitcoin. Nos primeiros dias do Bitcoin, essa recompensa era de 50 bitcoin por bloco. Essa recompensa incentivava as pessoas a usarem poder computacional e eletricidade para ajudar a proteger a rede.

A cada 210.000 blocos (aproximadamente a cada 4 anos), a recompensa de bloco é cortada pela metade. Esse evento é chamado de **halving**. O halving desacelera a criação de novos bitcoin e ajuda a garantir que o fornecimento total nunca ultrapasse 21 milhões. Com o tempo, isso torna o bitcoin cada vez mais escasso.


> **Definition – Oferta circulante**
>
> **Oferta circulante** refere-se à quantidade total disponível de uma moeda. No caso do Bitcoin, a oferta circulante total é o número de moedas que já foram mineradas e estão em circulação em determinado momento.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/0db11a2db83970e70220655682e7c17425c4415c-292x200.svg)


> **Definition – Cronograma de emissão do Bitcoin**
>
> O **cronograma de emissão do Bitcoin** é o plano pré-determinado e público para a liberação de novos bitcoin em circulação, projetado para manter a escassez do Bitcoin ao longo do tempo.


Após cada evento de halving, a recompensa em bitcoin que os mineradores recebem por adicionar um bloco é cortada pela metade. Isso reduz a taxa na qual novos bitcoins são criados.

Os mineradores ainda ganham taxas de transação das transações incluídas no bloco que mineram. Com o tempo, espera-se que essas taxas se tornem uma parte maior da renda dos mineradores.

Os halvings estão incorporados no protocolo do Bitcoin e acontecem automaticamente a cada quatro anos, aproximadamente. Por causa disso, o cronograma de emissão do Bitcoin é previsível e transparente.

A tabela mostra os próximos halvings, incluindo a data aproximada, o número do bloco em que ocorrem, a nova recompensa por bloco e a porcentagem do fornecimento total de bitcoin que já terá sido minerada.


| Evento | Data | Bloco | Recompensa | Minerado |
| --- | --- | --- | --- | --- |
| 5º Halving | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| 6º Halving | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| 7º Halving | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


À medida que mais bitcoin são minerados, a oferta em circulação continua aumentando até atingir o limite máximo de 21.000.000 de bitcoins, o que é esperado por volta do ano 2140. Como cada vez menos bitcoins novos são criados ao longo do tempo, se a demanda aumentar, o preço do Bitcoin pode subir. Isso também incentiva os mineradores a continuarem protegendo a rede ao contribuir com seu poder computacional.

#### O que é um hash de bloco válido no Bitcoin?

No Bitcoin, os mineradores competem para encontrar um código especial chamado **hash de bloco**. Esse código identifica um bloco de transações e permite que ele seja adicionado à blockchain.

Cada bloco contém informações sobre transações recentes e também inclui o hash do bloco anterior. Isso conecta todos os blocos, formando uma cadeia desde o primeiro bloco (o Bloco Gênese) até o mais recente.

Um hash funciona como uma **impressão digital** para os dados do bloco. Se qualquer informação no bloco for alterada, a impressão digital também mudará. Isso facilita para qualquer pessoa verificar que o histórico de transações da blockchain não foi alterado e ajuda a manter a rede segura.


> **Callout**
>
> Satoshi Nakamoto, o criador do Bitcoin, minerou o Bloco Gênese, que liberou um total de 50 bitcoin.


#### A Corrida para Minerar um Bloco

Os mineradores competem para encontrar um hash de bloco válido. O primeiro minerador a encontrar um recebe o direito de adicionar o novo bloco à blockchain e ganhar uma recompensa em bitcoin.

Para ser válido, o hash do bloco deve ser menor que um número definido pela rede chamado alvo de dificuldade. Como os hashes são aleatórios, os mineradores precisam tentar diferentes entradas até encontrar uma que funcione.

Se muitos mineradores estiverem competindo, os blocos seriam encontrados rápido demais. Se poucos mineradores estiverem participando, os blocos demorariam muito para serem encontrados. Para manter o sistema funcionando de forma estável, o Bitcoin ajusta automaticamente a dificuldade a cada 2.016 blocos (aproximadamente a cada duas semanas).

Esse ajuste garante que, em média, um novo bloco seja adicionado à blockchain a cada 10 minutos.


> **Definition – Definição de nível de dificuldade**
>
> O **nível de dificuldade** na mineração de Bitcoin mede o quão difícil é encontrar um hash de bloco válido. A rede ajusta essa dificuldade a cada 2.016 blocos (aproximadamente a cada duas semanas) para que novos blocos sejam adicionados à blockchain a cada 10 minutos, em média. Quanto maior a dificuldade, mais difícil é para os mineradores encontrarem um bloco válido.


Ao encontrar um hash de bloco válido, o minerador prova que realizou o trabalho necessário para adicionar um novo bloco à blockchain. Esse processo é chamado de **Prova de Trabalho** (PoW). É o mecanismo de segurança que permite ao Bitcoin confirmar transações e adicionar novos blocos à blockchain. O minerador que encontra o hash válido primeiro recebe uma recompensa em bitcoin, que inclui a recompensa do bloco e as taxas das transações incluídas nesse bloco.

A Prova de Trabalho (PoW) ajuda a manter o Bitcoin seguro, tornando extremamente caro para qualquer pessoa tentar trapacear ou assumir o controle da rede. Em vez disso, é muito mais lucrativo seguir as regras.

Os mineradores desempenham quatro funções principais:

1. **Coletar transações**: Os mineradores escolhem transações que foram enviadas para a rede e as colocam em um bloco candidato.
1. **Executar Prova de Trabalho**: Os mineradores competem para resolver um quebra-cabeça matemático difícil ao encontrar um hash de bloco válido.
1. **Transmitir o bloco**: O primeiro minerador a encontrar uma solução válida compartilha o novo bloco com a rede.
1. **Receber recompensas**: Se o bloco for válido, ele é adicionado à blockchain e o minerador recebe novos bitcoins criados, além das taxas de transação.

Muitos mineradores ao redor do mundo tentam criar o próximo bloco ao mesmo tempo. Quando um minerador encontra uma solução válida, a rede verifica o bloco. Se tudo estiver correto, ele é adicionado à blockchain. Outros blocos concorrentes são descartados. Esse processo mantém a rede em consenso e impede o duplo gasto.

* Mineradores são computadores que ajudam a manter e atualizar o registro do Bitcoin.
* Eles coletam transações e as agrupam em um bloco. Em seguida, processam os dados do bloco por meio de um algoritmo de hash para criar um código único chamado hash.
* Os mineradores repetem esse processo muitas vezes, buscando um hash que atenda às regras do Bitcoin. O primeiro minerador a encontrar um hash válido recebe novos bitcoins como recompensa, e seu bloco é adicionado à blockchain.
* O hash de cada bloco também o conecta ao bloco anterior. Se alguém tentasse alterar uma transação passada, os hashes não corresponderiam mais e a rede rejeitaria a cadeia alterada. É isso que mantém o registro do Bitcoin seguro.
