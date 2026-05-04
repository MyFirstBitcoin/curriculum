# 3.7 Bitcoin

Após muitos anos e tentativas fracassadas, os Cypherpunks, em sua maioria, já haviam começado a perder o interesse na ideia de uma moeda digital sem permissão, quando Adam Back recebeu um e-mail com um link para um rascunho de white paper chamado ‘dinheiro eletrônico sem terceira parte’ de uma pessoa anônima que se autodenominava Satoshi Nakamoto.

Para recapitular até este ponto, temos pelo menos as ideias de:

* Assinaturas criptográficas que poderiam fornecer um nível de privacidade e anonimato
* Conceito de uma moeda sem lastro (B-Money)
* Propostas (mas sem meios) para limitar a emissão de nova moeda
* Moedas digitais cuja propriedade era atribuída por chaves públicas (B-Money) e podiam ser transferidas por assinatura e reatribuídas com base no endereço do destinatário (RPOW e Hashcash)
* Todos os nós mantêm uma cópia de um livro-razão totalmente distribuído (B-Money) (descartado na época como impraticável)
* Protocolo de marcação temporal – usando hash de árvore de Merkle para fornecer uma cronologia matematicamente comprovável de eventos que é difícil de falsificar se todos os usuários mantiverem os mesmos registros
* Prova de trabalho para vincular esforço do mundo real ao sistema (mas usando o próprio hash como moeda)
* Redes totalmente descentralizadas onde todos os pares são iguais e podem entrar e sair da rede (BitTorrent)
* Conceito de vincular novos hashes a hashes anteriores (Bit Gold e marcação temporal)

O que faltava nesse momento incluía:

* Uma solução viável para resolver o problema dos ‘generais bizantinos’
* Um método para limitar a quantidade de dinheiro em circulação apesar das melhorias contínuas de hardware
* Esquema de incentivos para as pessoas participarem (problema do ovo e da galinha)

A outra grande diferença entre as tentativas recentes e o Bitcoin foi que Satoshi já vinha trabalhando no código há algum tempo, no verdadeiro espírito original dos ‘Cypherpunks escrevem código’, antes de anunciá-lo nas listas de discussão, ao contrário do Bit Gold e do B-Money, que eram mais conceituais.

Qual foi a inovação que diferenciou o Bitcoin das tentativas anteriores de dinheiro eletrônico?

A prova de trabalho seria usada como mecanismo de consenso e como forma de fornecer segurança e imutabilidade: Em vez de usar o hash como forma de dinheiro, ele seria usado por um novo processo conceitual chamado mineração, onde um nó agruparia um conjunto de transações, adicionaria um número aleatório e então aplicaria o hash ao ‘bloco’ de dados. Um bloco válido que atendesse ao requisito de hash seria então anunciado à rede. Esses blocos seriam ligados entre si usando o hash do bloco anterior em cada um, e a blockchain mais longa seria usada no caso de um desempate, onde diferentes nós validariam e anunciariam blocos diferentes ao mesmo tempo, criando divisões na cadeia. A prova de trabalho tornou-se o desempate distribuído para resolver o problema dos generais bizantinos.

Esses mineradores também receberam um incentivo para fornecer a CPU necessária para realizar a prova de trabalho, sendo alocados novos bitcoins para cada bloco. A quantidade de Bitcoin que recebem também está programada para diminuir aproximadamente a cada 4 anos até que todos os Bitcoins tenham sido criados, criando um limite rígido para o total de Bitcoin que jamais estará em circulação, de 21 milhões.

A ideia mais original foi a forma como ele resolveu a questão de quanto dinheiro é criado à medida que o hardware melhora e mais poder pode ser aplicado à rede. As marcações de tempo de um número definido de blocos (2016) seriam calculadas em média, e se estivessem sendo criados muito rapidamente, o hash necessário para criar um novo bloco seria tornado mais difícil; se muito lentamente, seria facilitado. Isso foi incorporado ao protocolo descentralizado que todos os nós executam e, portanto, qualquer minerador que o ignorasse gastaria energia para minerar um bloco sem benefício, pois seria rejeitado pelo restante da rede. Esse ajuste garante que a criação de novos blocos permaneça no cronograma planejado de emissão e fornece incentivos para que os mineradores ‘sigam as regras’.

####   
Resumo

Muitas das peças do quebra-cabeça do que é necessário para construir um sistema de dinheiro eletrônico descentralizado peer-to-peer baseado em princípios de moeda sólida já estavam no lugar antes de Satoshi lançar seu whitepaper e logo após o lançamento inicial do código.

> A natureza do Bitcoin é tal que, uma vez que a versão 0.1 foi lançada, o design central ficou gravado em pedra para o resto de sua existência  
_Satoshi Nakamoto_

Embora muitas ideias de melhorias (BIPs) tenham sido propostas e adotadas, o Bitcoin vem funcionando em segundo plano desde 2009 seguindo o protocolo projetado no lançamento inicial e com quase nenhuma interrupção. Todas as melhorias foram feitas mantendo a compatibilidade retroativa com todas as versões anteriores.



##### Notas

1. Para uma explicação do problema dos Generais Bizantinos - veja [https://pt.wikipedia.org/wiki/Falha_bizantina](https://en.wikipedia.org/wiki/Byzantine_fault)
