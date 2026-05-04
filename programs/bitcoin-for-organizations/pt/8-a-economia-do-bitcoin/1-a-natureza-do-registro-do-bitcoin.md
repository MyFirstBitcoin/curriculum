# 8.1 A Natureza do Registro do Bitcoin

O livro-razão de transações do Bitcoin (também chamado de timechain ou blockchain) é um registro público, com carimbo de data e hora, de todas as transações válidas que já ocorreram na rede. No sistema financeiro tradicional, as transações internas são visíveis apenas para participantes autorizados, como bancos, reguladores ou operadores de dados como SWIFT, BACS ou SEPA. O acesso aos dados de pagamento nesses sistemas tradicionais pode ser altamente restrito e caro.

Por outro lado, na rede Bitcoin, qualquer pessoa com conexão à internet pode visualizar todas as transações, desde os maiores valores até o Satoshi individual. Os participantes podem acompanhar o fornecimento total de bitcoin em tempo real, monitorar a atividade de endereços e carteiras, e visualizar recompensas de mineradores e comportamento das taxas. Embora a atividade visível no livro-razão esteja vinculada a endereços de chave pública e não a identidades individuais, é possível agregar grandes conjuntos de dados sobre o comportamento de gastos, permitindo que todos coletem e pesquisem a atividade econômica em tempo real. À medida que a rede cresce e se torna mais aceita como fonte de verdade econômica, podemos ver uma menor dependência de órgãos governamentais e provedores terceirizados para a produção de análises estatísticas e relatórios sobre comportamento de gastos.



#### 8.1.1 Nós e Exploradores de Blocos

Qualquer pessoa que deseje verificar independentemente o livro-razão do Bitcoin e acessar seus dados deve rodar um nó completo. O nó completo é frequentemente descrito como a forma mais fundamental de participar e verificar a economia do Bitcoin. Ele está disponível globalmente como software de código aberto que, ao ser executado, fará o download e validará todo o livro-razão do Bitcoin desde o ‘Bloco Gênese’, publicado em janeiro de 2009, até os dias atuais. Ele também contribui para a segurança da rede Bitcoin ao ajudar a verificar novas transações que estão sendo adicionadas ao livro-razão. Ao acessar o livro-razão do Bitcoin dessa forma, o nó completo serve como fonte de verdade para pesquisadores e auditores da rede. E, para os usuários de Bitcoin, o nó completo atua como um portal ‘autossoberano’ para as informações transacionais da economia do Bitcoin, pois aumenta a privacidade e a segurança ao eliminar a dependência de serviços de terceiros.

Enquanto os nós completos baixam os dados brutos, exploradores de blocos como mempool.space ou blockstream.info oferecem uma interface visual para pesquisar e interpretar a atividade do livro-razão. O explorador de blocos permite rastrear transações individuais e visualizar saldos e históricos de carteiras. Ele também mostra métricas de atividade dos mineradores, como recompensas de bloco e dados de taxas de transação.

Juntos, nós completos e exploradores de blocos são as ferramentas que tornam a transparência da rede Bitcoin utilizável.



#### 8.1.2 Atividade: Explorando o Livro-Razão do Bitcoin

1. Abra [mempool.space](https://mempool.space) e explore a página inicial.
  * Qual é a altura do bloco mais recente?
  * Qual é a taxa de transação atual (Baixa, Média e Alta Prioridade)?
  * Quantas transações estão aguardando no mempool para o próximo bloco?
1. Acesse o bloco mais recente no livro-razão.
  * Quantas transações foram incluídas?
  * Nomeie o minerador do bloco.
  * Qual foi a recompensa do bloco?
1. Acesse uma transação no bloco.
  * Quantas entradas e saídas a transação possui?
  * Qual é o valor da transação em BTC e USD?

Discuta as diferenças entre como o dinheiro circula no sistema tradicional e como uma empresa ou governo utiliza esse tipo de transparência.
