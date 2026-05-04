# 2.4 Não há inovação acontecendo no Bitcoin.

> A criação de mil florestas está em uma única bolota.   
_Ralph Waldo Emerson_

Críticos frequentemente tentam afirmar que o Bitcoin é uma tecnologia 'antiga' ou 'morta' porque não altera o protocolo da camada base com a mesma frequência que blockchains concorrentes. Essa afirmação ignora tanto os motivos pelos quais as mudanças no Bitcoin são adotadas lentamente quanto a quantidade de inovação que ocorre para escalar a rede em camadas superiores, como a Lightning Network. Também ignora que muitas das nossas tecnologias mais flexíveis e duráveis também não escalam rapidamente na camada base.

Por exemplo, também não há inovação acontecendo no Protocolo de Controle de Transmissão (TCP), que é a base da internet. O TCP foi criado pela primeira vez em 1974. A última vez que o TCP foi atualizado foi em 1982. Ele faz o que precisa fazer. Não é perfeito, e há debates sobre se precisamos atualizar o IPv4 para suportar desenvolvimentos futuros da internet. No entanto, dizer que não houve inovação na internet desde 1982 seria uma afirmação notável. Toda essa inovação aconteceu 'sobre' o TCP, e não 'dentro' dele.

A grande maioria da inovação que está acontecendo não é 'dentro' do Bitcoin, mas 'sobre' o Bitcoin. Um dia, provavelmente não haverá mais inovação 'dentro' do Bitcoin, e isso deve ser um objetivo e não uma crítica, pois será um reflexo de quão fundamental ele se tornou ao apoiar a economia global, fornecendo as bases para um dinheiro sólido global, neutro e sem permissões. Dinheiro que é sólido tanto no sentido econômico, pois há uma oferta fixa e um registro imutável, quanto no sentido tecnológico, já que não muda e o que está rodando teve anos de funcionamento ininterrupto. O Bitcoin já atingiu 100% de disponibilidade nos últimos 10 anos.

No entanto, seria preocupante se não houvesse inovação acontecendo 'sobre' o Bitcoin. Vamos dar uma olhada nisso nos últimos 10 anos:



#### 'Dentro' do Bitcoin

O Segregated Witness (SegWit) foi implementado em 2017 para proteger contra a maleabilidade de transações e aumentar a capacidade dos blocos. O SegWit também foi um precursor necessário para que a Lightning Network e algumas sidechains funcionassem de forma eficiente.

O Taproot foi implementado em 2021 para permitir o agrupamento e validação de múltiplas assinaturas ao incorporar assinaturas Schnorr, introduzindo uma linguagem de script para permitir funcionalidades mais complexas e aumentando a privacidade e a resistência à censura das transações.



#### 'Sobre' o Bitcoin

##### Sidechain Liquid

A sidechain Liquid foi implementada em 2018. A Liquid, como outras sidechains, é um livro-razão de blockchain separado que está vinculado à blockchain principal do Bitcoin, de acordo com um conjunto predefinido de regras. Essas regras são flexíveis o suficiente para permitir que a cadeia Liquid desenvolva e incorpore melhorias de design e escalabilidade ao longo do tempo. No entanto, a ligação com a blockchain do Bitcoin garante que o limite total de 21 milhões de bitcoins seja consistente em ambas as cadeias.

O ativo na Liquid, L-BTC, é ancorado em duas vias ao bitcoin na cadeia principal. Existem compensações de custo, velocidade, privacidade e segurança que tornam o L-BTC ideal para algumas aplicações. Custo, velocidade e privacidade são todos melhorados com o L-BTC, à custa de confiar parcialmente nas organizações que compõem a Federação Liquid, que entre elas controlam um processo multisig de 11 de 15 para ancorar e desancorar L-BTC para bitcoin e vice-versa.

##### Lightning Network

A Lightning Network foi implementada em 2018. A Lightning foi projetada para ser uma rede de pagamentos peer-to-peer na forma de um grafo de nós conectados por canais; não é uma blockchain. O bitcoin é bloqueado por um operador de nó na blockchain principal para torná-lo disponível para uso na Lightning Network, garantindo que apenas bitcoin 'real' seja utilizado. Os nós podem então abrir canais de liquidez via contratos inteligentes multisig entre si. Os pagamentos encontram rotas pela rede da origem ao destino, otimizando o custo conforme a necessidade de liquidez suficiente na direção correta entre cada etapa do nó na rota. A Lightning Network melhora enormemente o custo, a velocidade e a privacidade em troca de uma perda de segurança (ou aumento da confiança necessária) e aumento da complexidade. No entanto, ela é destinada a pagamentos diários de alto volume e baixo valor, então essa é considerada uma troca muito razoável para seus milhões de transações diárias (fonte: River, 2023).

##### Mints de eCash Chaumiano

Fedimints podem ser vistos como uma Lightning Network limitada a uma comunidade. Eles são projetados para aproveitar a confiança inerente que existe dentro de certas comunidades (por exemplo, famílias, vilarejos, grupos de amigos) em troca de simplificar a complexidade e aumentar a privacidade para os usuários. São protocolos modulares e de código aberto para custodiar e transacionar bitcoin em um contexto comunitário. São interoperáveis com a própria Lightning Network.

**Cashu** é um token ao portador que pode ser armazenado em um dispositivo como um telefone celular; o design visa reproduzir os benefícios do dinheiro físico, mas em formato digital. O Cashu é um exemplo de eCash Chaumiano construído sobre o Bitcoin e aumenta a privacidade e a resistência à censura, além de reduzir a complexidade em troca da confiança no mint de eCash utilizado. Os mints Cashu emitem tokens de eCash, representando bitcoin, que podem ser gastos pelos usuários sem revelar sua identidade. O Cashu é interoperável com a Lightning Network.

Provavelmente haverá muitas outras aplicações de camada 2 construídas no futuro, com muitas aplicações de camada 3 sendo construídas sobre cada uma dessas.

Como exemplo do incrível número de aplicações sendo construídas sobre a Lightning, aqui está um trecho de um Relatório de Pesquisa da Lightning Network feito pela River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
