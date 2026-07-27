# 6.1 A Descoberta da Escassez Digital

> Com o Bitcoin, um novo tipo de commodity foi descoberto... um tipo de commodity digital, gerada por computadores e em parte feita para computadores. A humanidade tem um histórico de invenções significativas. Nos livros de história que serão escritos no futuro, o Bitcoin será listado como uma delas.  
_Prof. Dr. Philipp Sander_



#### 6.1.0 Escassez na Economia

No âmbito da economia, é bem compreendido que a escassez é um princípio fundamental que impulsiona o valor. Bens e serviços que apresentam demanda significativa tornam-se mais valiosos se a oferta for limitada a ponto de a demanda não poder ser facilmente atendida. Além disso, a escassez estimula a competição e é um fator determinante na descoberta de preços no mercado. Em um mercado de competição livre, justa e aberta, os preços devem se estabilizar no ponto em que a oferta e a demanda se encontram.

Recursos que apresentam demanda significativa podem ser considerados mais valiosos se forem finitos ou mais difíceis de adquirir. Isso pode estimular uma demanda ainda maior por esse recurso, à medida que os participantes do mercado competem para garantir acesso a ele. Essa dinâmica pode ser observada com recursos naturais como metais preciosos, petróleo ou os chamados 'soft commodities', como alimentos. A escassez, portanto, fundamenta a tomada de decisões econômicas, a alocação de recursos e o custo de oportunidade. Em um mundo de recursos ilimitados, tudo seria igualmente acessível e de valor muito baixo. Em contraste, a escassez confere valor e promove o comércio, o investimento e a inovação, pois obriga as sociedades a gerenciar recursos limitados de forma eficaz.



#### 6.1.1 O Desafio da Escassez Digital

O desafio em torno da escassez digital reside na facilidade com que a informação digital pode ser copiada e distribuída. A informação digital é inerentemente mais difícil de proteger do que a informação física porque, ao contrário dos bens físicos - alguns dos

quais possuem escassez natural devido a restrições materiais - itens digitais como arquivos de música, documentos ou imagens podem ser duplicados infinitamente a praticamente nenhum custo.

Tradicionalmente, a replicabilidade dos dados digitais significava que esses ativos não podiam ter um valor econômico semelhante ao dos ativos físicos, pois lhes faltava qualquer forma de escassez aplicável. Para o dinheiro digital, isso é particularmente problemático e é caracterizado como o problema do 'gasto duplo', onde uma única unidade digital (por exemplo, um token ou moeda) poderia ser copiada e gasta várias vezes, desvalorizando-a. Se for possível gastar uma moeda digital duas vezes, ela perde valor por se tornar indistinguível de fundos falsificados ou fraudulentos.

Tradicionalmente, instituições financeiras centralizadas como bancos mitigam esse risco mantendo um livro-razão que verifica cada transação e deduz os saldos de acordo, garantindo que, uma vez que o dinheiro é gasto, não possa ser reutilizado pelo mesmo titular da conta. No entanto, essa abordagem exige uma autoridade central confiável ou 'oráculo' para gerenciar e verificar as transações, o que impõe dependência e um ponto único de controle. Ter um oráculo centralizado de informações deixa os ativos digitais vulneráveis à manipulação e censura.

Para um sistema descentralizado e com confiança minimizada como o Bitcoin, onde não existe uma autoridade central para supervisionar as transações, prevenir o gasto duplo é um desafio monumental. Sem um mecanismo para garantir a unicidade de cada transação, o Bitcoin estaria aberto à exploração, tornando-o impraticável como reserva de valor e meio de troca confiável. O Bitcoin resolve o problema do gasto duplo por meio de um livro-razão descentralizado, onde as transações são confirmadas por milhares de participantes da rede simultaneamente. Esse mecanismo permite que o Bitcoin mantenha um registro imutável de cada transação, garantindo que cada moeda só possa ser gasta uma vez.

Essa solução gera escassez digital sem depender de controle centralizado. O Bitcoin introduz a primeira solução bem-sucedida para a escassez digital, abrindo caminho para um ecossistema de ativos digitais escassos e com confiança minimizada, de uma forma antes considerada impossível.



#### 6.1.2 Aplicando a Escassez Digital com o Bitcoin

> Propomos uma solução para o problema do gasto duplo usando um servidor de carimbo de data/hora distribuído peer-to-peer para gerar prova computacional da ordem cronológica das transações. O sistema é seguro enquanto nós honestos controlarem coletivamente mais poder de CPU do que qualquer grupo cooperativo de nós atacantes.  
_Satoshi Nakamoto_

Satoshi Nakamoto criou o Bitcoin como uma solução de engenharia para os problemas associados ao dinheiro fiduciário. No entanto, essa solução exigiu que Satoshi descobrisse uma forma de impor escassez digital absoluta. Para isso, Satoshi desenvolveu um protocolo de comunicação de código aberto que roda em uma rede descentralizada de computadores ou nós. Cada um desses nós mantém uma cópia localmente verificável de um livro-razão imutável, o chamado blockchain ou timechain. O protocolo Bitcoin define as regras e a rede descentralizada verifica as transações de forma independente, seguindo as mesmas regras sem exigir uma autoridade central.

A escassez do Bitcoin contribui para seu papel como reserva de valor. Assim como o ouro, o Bitcoin é valioso não apenas por sua oferta limitada, mas também pelo esforço necessário para 'minerar' ou produzir novas moedas. A mineração de Bitcoin (o processo que mantém o livro-razão e emite novas moedas) é um processo caro e intensivo em energia, que espelha o ato físico de extrair minerais da terra. Essa 'prova de trabalho' digital impõe uma restrição de produção que alinha o Bitcoin com commodities tangíveis, conferindo-lhe propriedades de durabilidade e verificabilidade que os bens digitais tradicionais não possuem. A dificuldade embutida e a taxa decrescente de emissão de novas moedas por meio dos 'halvings' periódicos criam uma estrutura econômica em que a oferta de Bitcoin se torna cada vez mais escassa ao longo do tempo, aumentando seu apelo como reserva de valor de longo prazo.

##### Como a escassez digital é aplicada?

A solução do Bitcoin para o problema do gasto duplo está em seu uso de um livro-razão descentralizado e publicamente visível. O livro-razão do Bitcoin pode ser visto como um banco de dados imutável que registra cada transação em uma cadeia sequencial de lotes com carimbo de data/hora, chamados blocos. Cada bloco é estritamente cronológico e contém transações que foram verificadas e aceitas pelos participantes da rede. Cada bloco está conectado ao anterior, criando um registro permanente que é distribuído por milhares de nós ao redor do mundo. Ao armazenar e compartilhar esse livro-razão em uma rede descentralizada, o Bitcoin elimina a necessidade de uma autoridade central para confirmar transações. Quando uma transação de Bitcoin ocorre, os nós da rede a validam de forma independente, garantindo que cada moeda seja gasta apenas uma vez. Esse livro-razão compartilhado também torna extremamente difícil para atacantes invadirem a rede ou alterarem transações passadas, pois qualquer alteração exigiria aprovação da maioria dos participantes da rede.

O mecanismo de Prova de Trabalho (PoW) do Bitcoin reforça ainda mais sua proteção contra o gasto duplo ao exigir que os mineradores resolvam um problema criptográfico para terem permissão de validar novas transações e criar um novo bloco. Esse processo, conhecido como mineração, demanda poder computacional e adiciona um nível de dificuldade e custo para alterar o livro-razão. Cada bloco adicionado ao livro-razão deve conter um vínculo criptográfico com o bloco anterior, o que solidifica a integridade da cadeia e impede adulterações.

O papel de um nó é armazenar a cópia mais atual do livro-razão, que contém todo o histórico de transações. Os nós mantêm os mineradores 'honestos', pois verificam se não ocorreu gasto duplo e, principalmente, se todas as moedas foram criadas de acordo com o cronograma de emissão do Bitcoin. Qualquer usuário de Bitcoin pode rodar um nó e verificar a posse de suas moedas sem precisar confiar em terceiros. Não há necessidade de autoridades para resolver disputas no Bitcoin porque qualquer transação incluída em um bloco é objetivamente válida.

##### Como um atacante poderia controlar a rede Bitcoin?

Se um atacante quisesse alterar uma transação passada para ter sucesso em um ataque de gasto duplo, ele precisaria refazer a Prova de Trabalho para aquele bloco e todos os blocos subsequentes, competindo contra o poder computacional combinado de toda a rede. Esse mecanismo de segurança garante que, se alguém tentar um gasto duplo, precisaria controlar mais de 50% do poder de mineração da rede para ter sucesso. Isso é conhecido como ataque de 51%.

Nos primeiros anos do Bitcoin, quando era possível que participantes individuais criassem ou minerassem novos blocos usando hardware de computação geralmente disponível, era pelo menos teoricamente possível implantar poder computacional suficiente para realizar um ataque de 51%. Hoje, o poder computacional combinado da rede de Prova de Trabalho supera 700 ExaHash/s. Isso significa que, em conjunto, os computadores de mineração estão calculando mais de 700 quintilhões de hashes (cálculos criptográficos) por segundo. Chegamos a um ponto em que o imenso custo e a coordenação necessários para reescrever o livro-razão e realizar um ataque de 51% tornam o gasto duplo inviável na prática.

##### Confirmações e Reorganizações

Outra camada de proteção (que às vezes é negligenciada) vem do processo de confirmação de transações do Bitcoin. Quando uma transação é transmitida pela primeira vez, ela é considerada não confirmada e coletada no 'mempool' enquanto aguarda inclusão em um bloco e validação pelos mineradores. Uma vez que a transação é adicionada a um bloco, ela é considerada 'confirmada'. Cada bloco adicionado depois disso é contado como uma confirmação adicional para a transação. Embora uma transação seja considerada oficial após uma única confirmação, ela não é considerada final até que mais confirmações sejam adicionadas.

Para segurança total, os usuários de Bitcoin geralmente aguardam múltiplas confirmações (tipicamente seis), pois cada bloco adicional adicionado ao blockchain reforça ainda mais a segurança da transação, reduzindo drasticamente a probabilidade de uma tentativa de gasto duplo bem-sucedida. Esse processo de confirmação estabelece uma janela de tempo durante a qual as transações são finalizadas.

##### Por que esperar por seis confirmações?

Os usuários de Bitcoin aguardam mais confirmações porque é possível que o bloco mais recente de transações seja removido da cadeia de blocos, caso ele não faça mais parte da cadeia mais longa. É importante notar que a mineração é uma competição entre grandes pools de poder computacional. Portanto, é possível que dois mineradores concorrentes encontrem uma solução criptográfica válida e blocos separados sejam adicionados à cadeia quase ao mesmo tempo. Se isso acontecer, a cadeia é essencialmente dividida. Os mineradores continuarão tentando adicionar blocos a cada ramo da cadeia. No entanto, assim que o próximo bloco for minerado, a cadeia mais longa1 (definida como a cadeia que possui a maior prova de trabalho investida) é a que prevalece e o bloco na cadeia mais curta é 'órfão' e se torna inválido. Todas as transações no bloco órfão retornam ao mempool para inclusão em um bloco válido posterior. Esse processo é chamado de reorganização ou, simplesmente, 'reorg'.

Um agente malicioso, tentando um gasto duplo, deve controlar a rede por tempo suficiente para 'reorganizar' a cadeia. Como vimos acima, obter controle total exige uma quantidade enorme de poder computacional, mas e se uma grande operação de mineração - que hipoteticamente controla pouco mais de um terço de todo o poder computacional da rede - tentar um gasto duplo de moedas?

Vamos analisar um exemplo:

Vamos supor, por exemplo, que o poder total de mineração da rede Bitcoin seja de 550 ExaHash/s. A Rogue Inc, que controla 200 ExaHash/s, faz uma grande compra de imóveis e pretende pagar em Bitcoin. No entanto, a Rogue também planeja tentar um duplo gasto das mesmas moedas. O vendedor informa à Rogue que aguardará seis confirmações antes de entregar as escrituras do imóvel. Para realizar um ataque de duplo gasto, a Rogue deve construir um ramo alternativo na cadeia em segredo, minerando uma cadeia mais longa contendo a transação de duplo gasto. Assim que o vendedor visualizar seis confirmações contendo sua transação e entregar o ativo, a Rogue deve então publicar todos os blocos que minerou em um novo ramo, tornando-o a cadeia mais longa. Quão possível é isso?

A qualquer momento, a probabilidade de a Rogue minerar o próximo bloco é 200/550 = 0,36. Mesmo que a Rogue seja o maior pool de mineração, a probabilidade de os mineradores honestos encontrarem o próximo bloco é 1 - 0,36 = 0,64. Os blocos devem ser minerados muito mais rapidamente na cadeia honesta. Mas suponha que a Rogue tenha sorte, mine um bloco e o mantenha em segredo. Ela então tenta minerar outro nesse ramo secreto. No entanto, a cadeia honesta então minera um bloco e fica à frente ao minerar outro, antes que a Rogue mine seu segundo bloco.

A Rogue então desiste. Por quê?


| Blocos para alcançar | 1% | 10% | 36% (Rogue) | 51% |
| --- | --- | --- | --- | --- |
| 1 | 0,010101 | 0,111111 | 0,562500 | 1,0 |
| 2 | 0,010102 | 0,012346 | 0,316406 | 1,0 |
| 3 | 1,0e-06 | 0,001372 | 0,177919 | 1,0 |
| 4 | 1,0e-08 | 0,000152 | 0,100113 | 1,0 |
| 5 | 1,0e-10 | 0,000017 | 0,056314 | 1,0 |
| 6 | 1,0e-12 | 1,9e-06 | 0,031676 | 1,0 |


**Fonte**: Baseado em uma tabela do livro Grokking Bitcoin de Kalle Rosenbaum

A Rogue percebe que não tem poder de hash suficiente para realizar o duplo gasto, apesar de controlar 36% do poder de hash do Bitcoin. Para ter sucesso, ela precisaria minerar mais quatro blocos para ultrapassar a cadeia honesta. Apesar de seu vasto poder computacional e de controlar 36% da rede, as chances de sucesso da Rogue são de apenas 0,100113.


> **Dark – A Teoria dos Jogos Entra em Cena**
>
> As chances de sucesso da Rogue são péssimas, mas ainda pioram. A cada minuto que continua tentando, a Rogue consome uma enorme quantidade de eletricidade. Tudo isso terá sido em vão. Além disso, para cada bloco que ela deixa de minerar honestamente, a Rogue perde a recompensa do bloco, atualmente 3,125 moedas por bloco, avaliadas em mais de US$ 300 mil atualmente.
>
> A principal razão para o fracasso da Rogue foi que o vendedor do imóvel exigiu seis confirmações. Quanto mais confirmações forem necessárias, mais difícil será para mineradores desonestos construírem cadeias alternativas de blocos. De fato, para uma transação muito grande, o vendedor pode exigir ainda mais confirmações. Por exemplo, dez confirmações (que devem levar cerca de 100 minutos) reduziriam as chances de sucesso da Rogue para apenas 0,003.
>
> Dessa forma, a teoria dos jogos em torno da mineração garante que todos sejam incentivados a agir honestamente e não desperdiçar recursos computacionais ou abrir mão das recompensas dos blocos. Além disso, é do interesse de todos os mineradores que a rede Bitcoin seja segura e confiável. Isso garante que seu enorme investimento em poder computacional esteja protegido. Se a rede for atacada com sucesso, o valor de mercado das moedas cairá drasticamente, pois a confiança na rede será abalada.




#### 6.1.3 A Centralização da Mineração é uma Ameaça?

Como visto na tabela acima, a centralização da mineração pode representar uma ameaça potencial à proteção contra duplo gasto do Bitcoin, pois aumenta a probabilidade de um ataque de 51% – um cenário em que um único minerador ou grupo de mineradores controla mais da metade do poder computacional da rede. Se isso acontecesse, a entidade controladora poderia, teoricamente, alterar transações recentes ou tentar um duplo gasto reescrevendo o livro-razão, permitindo gastar as mesmas moedas mais de uma vez.

Tal situação compromete a integridade da rede Bitcoin ao conceder influência desproporcional sobre a validação de transações a poucos atores. No entanto, embora teoricamente possível, executar um ataque de 51% ainda seria altamente complexo e caro, exigindo imensos recursos computacionais, eletricidade e coordenação, o que provavelmente superaria os possíveis benefícios de tentar um duplo gasto.

Existem salvaguardas que ajudam a limitar os riscos da centralização da mineração. Os pools de mineração, por exemplo, permitem que mineradores menores combinem recursos e compartilhem as recompensas dos blocos, reduzindo a dominância de qualquer entidade única. Embora isso seja uma forma útil para pequenos mineradores participarem da rede, existe o risco de que a entidade controladora do pool possa agir de má-fé e tentar atacar a rede. No entanto, a transparência do livro-razão do Bitcoin também significa que qualquer concentração de poder de mineração é visível, alertando a comunidade para riscos potenciais e permitindo a adoção de contramedidas. Os mineradores estão muito cientes de que qualquer ataque à rede Bitcoin pode prejudicar seriamente sua proposta de valor, sendo assim muito simples para pequenos mineradores mudarem para um novo pool para evitar que seu poder de mineração seja usado de forma nefasta. Embora o risco não seja zero, a natureza aberta e distribuída do ecossistema do Bitcoin, combinada com o alto custo de um ataque, faz com que a centralização da mineração seja mais uma ameaça teórica do que iminente, já que manter tal controle por períodos prolongados seria financeiramente inviável para qualquer atacante.



#### 6.1.4 O Impacto Mais Amplo da Escassez Digital

O Bitcoin transformou a forma como pensamos sobre escassez no mundo digital. Como os bens digitais – como softwares, arquivos de música, e-books e conteúdos online – possuem características que os diferenciam dos bens físicos, eles podem ser reproduzidos a um custo insignificante e compartilhados instantaneamente. Diferentemente dos itens físicos, que estão sujeitos a restrições materiais como custos de produção e limitações de armazenamento, os bens digitais existem como dados que podem ser duplicados infinitamente sem qualquer degradação na qualidade. Isso significa que, enquanto os bens físicos são inerentemente escassos devido a essas restrições materiais, os bens digitais tradicionalmente têm sido abundantes, sem mecanismos embutidos para limitar sua oferta.

É importante notar que os bens digitais são não-rivais. Isso significa que o consumo de um bem digital por uma pessoa não diminui a disponibilidade desse bem para outras pessoas. Por exemplo, quando uma música é baixada, ela pode ser copiada e distribuída um número ilimitado de vezes sem perder utilidade. Historicamente, essa abundância representa um desafio para a criação de valor, já que o modelo econômico tradicional de oferta e demanda se distorce quando a oferta é, pelo menos teoricamente, ilimitada. Em resposta a isso, a gestão de direitos digitais (DRM) e outras medidas de escassez artificial tentaram restringir o acesso. No entanto, esses mecanismos podem ser contornados e transferem a confiança para autoridades centralizadas. A inovação do Bitcoin está em como ele resolve esse problema de forma nativa, tornando-se o primeiro ativo digital a incorporar escassez por meio de tecnologia descentralizada, sem depender dessas limitações tradicionais.

O Bitcoin desempenha um papel transformador ao estabelecer a escassez digital, introduzindo um protocolo que impõe uma oferta finita. Um limite de 21 milhões de moedas está codificado no protocolo e esse limite não pode ser alterado sem o consenso da rede, ou seja, de todos os milhares de participantes espalhados globalmente que executam nós do Bitcoin. Dessa forma, o Bitcoin criou um ativo que imita a natureza finita de commodities físicas, como o ouro, enquanto existe inteiramente no mundo digital. O limite de oferta é fundamental para a proposta de valor do Bitcoin e é sustentado por uma combinação de criptografia, mecanismos de consenso e código aberto e transparente. Isso garante que todos os participantes da rede sigam as mesmas regras, além de serem motivados pelo principal incentivo econômico de garantir que a oferta de moedas seja absolutamente e comprovadamente finita.

Ao resolver o problema do duplo gasto, o Bitcoin previne a inflação ou duplicação do ativo, um desafio que atormentou experimentos anteriores de dinheiro digital. No Bitcoin, nenhuma autoridade única controla a oferta, tornando-o imune à manipulação centralizada do tipo visto no sistema monetário fiduciário, como impressão arbitrária de moeda ou desvalorização. Essa inovação permite que o Bitcoin funcione como reserva de valor e proteção contra a inflação, possibilitando que ele ocupe uma posição única semelhante ao 'ouro digital' – um recurso digital escasso com valor verificável.



#### 6.1.5 Conclusão

Em conclusão, está se tornando cada vez mais compreendido que a inovação do Bitcoin em relação à escassez digital redefiniu o conceito de dinheiro. No entanto, às vezes é negligenciado que o Bitcoin também transformou o cenário digital ao resolver o antigo problema de criar escassez em um mundo digital inerentemente abundante. O Bitcoin introduziu efetivamente uma nova categoria de ativo digital que reflete as qualidades das commodities físicas.

Essa inovação demonstra que um sistema descentralizado pode estabelecer escassez, imutabilidade e valor independentemente de qualquer autoridade central. Além disso, pode ter usos além do dinheiro, já que inspirou todo um campo de pesquisa e desenvolvimento em torno dessa tecnologia.

Olhando para o futuro, o modelo de escassez digital do Bitcoin está moldando o futuro do dinheiro e do armazenamento de valor. À medida que as preocupações com a inflação e as questões sobre a gestão da moeda fiduciária se tornam mais reconhecidas, a oferta fixa do Bitcoin o torna cada vez mais atraente como proteção contra a instabilidade financeira tradicional.

Em última análise, a descoberta da escassez digital pelo Bitcoin pode marcar o início de uma mudança de paradigma, onde ativos digitais com escassez reconhecida e confiança verificável ganham reconhecimento como componentes valiosos da economia moderna, estabelecendo uma base para o futuro das finanças descentralizadas e da propriedade digital. Isso tem implicações significativas para o campo da economia – o Bitcoin forneceu o modelo de como escassez e valor podem existir em forma digital.

> Além da escassez digital, o Bitcoin é também o primeiro exemplo de escassez absoluta, sendo a única commodity líquida (digital ou física) com uma quantidade fixa definida que não pode ser aumentada de forma alguma. Até a invenção do Bitcoin, a escassez sempre foi relativa, nunca absoluta.  
_Saifedean Ammous_



###### Notas

1. A cadeia mais longa é aceita pelos nós do Bitcoin como a versão mais válida do livro-razão, pois é definida como a cadeia que exigiu mais esforço (ou maior prova de trabalho) para ser construída. Mais informações aqui: [https://learnmeabitcoin.com/technical/blockchain/longest-chain/](https://learnmeabitcoin.com/technical/blockchain/longest-chain/)
