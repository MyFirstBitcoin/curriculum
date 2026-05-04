# 8.2 Métricas para Análise do Livro-Razão

Como a transparência do Bitcoin é diferente dos sistemas financeiros tradicionais — onde grande parte do fluxo monetário ocorre a portas fechadas em instituições — isso dá origem a um campo rico de análises on-chain, onde dados em nível de rede se tornam uma lente para entender o comportamento dos usuários, fluxos monetários e tendências de longo prazo. Essas métricas podem ajudar a responder perguntas específicas, como o quão ativamente a rede está sendo usada, se as moedas estão sendo acumuladas ou vendidas, e se a rede está se tornando mais segura.

Compreender essas métricas é útil não apenas para usuários de Bitcoin, mas também para pesquisadores ou formuladores de políticas que buscam insights sobre esse sistema financeiro singularmente transparente.

Esta seção contém algumas métricas comumente usadas para analisar a atividade do Bitcoin agrupadas em subcategorias. Não é uma lista abrangente. Visite [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) para uma lista mais completa e descrições.



#### 8.2.1 Métricas de Endereços

As métricas de endereços são úteis para monitorar ao longo do tempo, pois indicam o nível de atividade na rede Bitcoin. Por exemplo, à medida que o Bitcoin é mais adotado, o número de endereços ativos aumenta. Podemos examinar isso mais a fundo ao destilar o número de endereços que possuem uma quantidade mínima especificada de Bitcoin, digamos 0,1 BTC, por um determinado período, como um ano. Embora isso forneça uma visão da adoção do Bitcoin ao longo do tempo, é imperfeito, já que um indivíduo pode possuir vários endereços de Bitcoin. Por outro lado, corretoras ou ETFs podem aparecer como entidades únicas ao manter fundos para um grande número de pessoas.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Endereços HODLando Bitcoin > X BTC por Ano. Fonte: Bitcoin Magazine Pro._

Ao comparar endereços com o preço de mercado atual do BTC, é possível visualizar a porcentagem de todos os endereços de Bitcoin que estão em lucro. Isso nos permite acompanhar o sentimento do mercado, pois podemos ver qual proporção do mercado está mantendo BTC com lucro ou prejuízo.

Por exemplo, o **Percentual de Lucro Não Realizado** no gráfico abaixo mostra a proporção de todos os endereços do livro-razão com lucro não realizado, medido em dólares americanos. Observe que, como o gráfico abaixo foi feito próximo ao recorde histórico do Bitcoin, a porcentagem de endereços mostrando lucro não realizado está próxima de cem por cento. Também podemos ver que períodos prolongados de Percentual de Lucro Não Realizado abaixo de um desvio padrão da média são incomuns. Portanto, uma queda abaixo dessa linha pode sugerir um bom ponto de entrada para compradores.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Percentual de Lucro Não Realizado. Fonte: checkonchain.com_



#### 8.2.2 Indicadores On-Chain

Os indicadores on-chain são úteis porque oferecem uma visão do comportamento da rede, além do que apenas preço e métricas de endereço podem mostrar. Eles ajudam analistas a entender as ações e o sentimento de diferentes tipos de participantes, como detentores de longo prazo versus traders de curto prazo, acompanhando como as moedas estão sendo mantidas, movimentadas ou avaliadas ao longo do tempo. Esses indicadores aproveitam a natureza transparente do livro-razão para revelar dinâmicas de mercado ocultas, como acumulação, distribuição ou até mesmo convicção dos investidores. Isso os torna particularmente úteis para identificar tendências estruturais, avaliar se o mercado está superaquecido ou subvalorizado e antecipar pontos de virada em um ciclo de mercado.

Por exemplo, ao examinar o valor das posses de BTC desde a última vez que foram transacionadas, podemos deduzir se o mercado está ou não sob estresse (como pode ocorrer durante um grande fundo de ciclo). Essa métrica é conhecida como **Preço Realizado** e nos dá um 'custo médio' de todo o BTC em circulação. Se o preço de mercado cair abaixo do Preço Realizado, isso mostra que, em média, a maioria dos endereços está com prejuízo não realizado.

Ao agrupar ainda mais os dados do livro-razão em faixas etárias, podemos mostrar como a quantidade de BTC se move entre endereços ao longo do tempo, o que cria padrões em ondas em um gráfico conhecidos como **Ondas HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Ondas HODL do Bitcoin. Fonte: Bitcoin Magazine Pro._

As Ondas HODL mostram o que detentores de longo, médio e curto prazo estão fazendo com seus BTC. Por exemplo, no gráfico acima, os detentores de curto prazo são mostrados em vermelho e laranja e podemos ver picos de atividade quando esse grupo corre para comprar próximo aos topos de mercado. Por outro lado, vemos que detentores de muito longo prazo (em roxo e azul) estão aumentando constantemente sua participação na rede, indicando alta convicção entre esses grupos. O gráfico é imperfeito, pois algumas moedas podem se mover de endereços antigos para novos sob controle do mesmo usuário. No entanto, ele fornece uma visão interessante da convicção dos detentores de longo prazo.

Outra forma de examinar o 'dinheiro inteligente' dos detentores de longo prazo é analisar o **Coin Days Destroyed** (CDD). O conceito de 'Coin Days' é o número de BTC multiplicado pelos dias desde a última movimentação das moedas. Por exemplo, 5 BTC que não se moveram por 100 dias acumularam 500 coin days e 10 BTC que não se moveram por 10 dias acumularam 100 coin days. Dessa forma, damos peso extra às moedas mantidas por mais tempo. Quando essas moedas são movimentadas, esses coin days são 'destruídos'. Esse indicador mostra aumentos em CDD em momentos de movimentos significativos de preço, o que fornece aos analistas uma maneira de separar a atividade rotineira do mercado de mudanças significativas no sentimento dos detentores de longo prazo.

Outra métrica que pode ajudar a identificar se o mercado está subvalorizando ou supervalorizando o BTC é o Market-Value to Realised Value ou **MVRV**. Ela é calculada simplesmente como a razão entre o Valor de Mercado (número de BTC em circulação multiplicado pelo preço de mercado) dividido pelo Valor Realizado (a soma de todo o BTC desde a última movimentação). Um MVRV alto sugere que mais moedas estão em lucro (frequentemente visto próximo aos topos de mercado) e um MVRV baixo indica que muitas moedas estão sendo mantidas com prejuízo (visto próximo aos fundos de mercado).



#### 8.2.3 Métricas de Mineração

As métricas de mineração são úteis para entender a segurança, os incentivos econômicos e a saúde geral da rede Bitcoin. Métricas como hashrate, receita dos mineradores, dificuldade e proporção de taxas revelam quanta potência computacional está protegendo o blockchain e quão bem os mineradores estão sendo recompensados por suas atividades.

O **Hashrate** da rede Bitcoin é talvez o indicador mais citado da saúde da rede e da força da segurança. Como o processo de mineração protege a rede e confirma que as transações no livro-razão são válidas, quanto maior o nível de poder computacional (ou de hashing), mais difícil seria para um agente malicioso dominar e atacar a rede.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate do Bitcoin. Fonte: Bitcoin Magazine Pro._

O gráfico acima mostra que, em maio de 2025, o poder computacional total da rede está em torno de 900 TeraHash/s (900 trilhões de cálculos criptográficos de 'hash' por segundo). Se o hashrate está subindo, isso mostra que a rede está se tornando mais segura, o que é tranquilizador para os usuários.

O Puell Multiple (criado por David Puell) observa o ciclo de mercado sob a perspectiva dos mineradores e sua receita. A métrica é calculada dividindo a emissão diária de BTC (em USD) pela média móvel de 365 dias do valor da emissão diária. A métrica ajuda a identificar períodos de estresse ou alívio para os mineradores. Historicamente, um múltiplo acima de 3 precedeu uma queda no valor de mercado do BTC, pois indica que os mineradores estão altamente lucrativos. Um valor abaixo de 0,5 indica estresse e historicamente sinalizou fundos de mercado para o valor do BTC.
