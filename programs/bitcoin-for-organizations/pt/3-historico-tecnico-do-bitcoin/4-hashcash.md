# 3.4 Hashcash

O Hashcash foi criado por Adam Back, outro dos primeiros inovadores nesse espaço. Adam tinha um forte interesse em mercados livres e privacidade na internet, e encontrou a lista de discussão dos Cypherpunks, na qual entrou e se tornou um participante ativo.

Ele estava muito interessado em dinheiro digital e fez algumas sugestões de como o grupo poderia potencialmente trabalhar mais de perto com Chaum no DigiCash, mas essas ideias não avançaram. Então, ele voltou sua atenção para outro problema emergente – o spam de e-mails. Ele e o restante dos Cypherpunks queriam encontrar uma solução para o problema do spam, onde era trivial para spammers criar e enviar milhares de e-mails que congestionavam as redes. Sua solução inovadora foi baseada em hashing – a capacidade, com a criptografia, de transformar qualquer dado em uma sequência única e aleatória de comprimento específico, criando o equivalente a um ‘selo’ digital que precisava ser adicionado ao e-mail para que fosse considerado válido e transmitido pela rede. Um custo trivial para um e-mail genuíno, mas proibitivo para um spammer.

A principal inovação que o Hashcash criou foi vincular recursos do mundo real – poder computacional – a uma rede digital. Enquanto os recursos digitais até então podiam ser replicados sem limites, o número de ‘hashcash’ criados era limitado por quanta energia as pessoas estavam dispostas a investir nisso.

Embora a solução atendesse a alguns dos critérios que Adam acreditava serem necessários em um sistema de dinheiro digital; era anônima, resiliente e sem necessidade de confiança, cada hashcash não era reutilizável e não era verdadeiramente escasso. Ele sugeriu outras formas de abordar essas questões usando terceiros externos.

##### BitGold

Nick Szabo desenvolveu o conceito de Hashcash e prova de trabalho para propor uma solução alternativa, que descreveu em uma lista de discussão um ano após a publicação do Hashcash, em 1998.

Embora estivesse se aproximando de uma solução, essa proposta ainda apresentava vários desafios.

* Quem administraria o Registro de propriedade dos hashes e como poderiam ser confiáveis?
* O hashing geralmente ficaria mais barato com o tempo, um desafio também para o HashCash.

Como os hashes vinculados seriam carimbados com data e hora, ele propôs algum tipo de rastreamento histórico da dificuldade do hashing na época; um hash mais antigo exigiria mais custos de processamento do que um mais recente, já que os custos diminuíram. Infelizmente, isso significava que os hashes não seriam ‘fungíveis’, ou seja, de valor igual, considerado um atributo fundamental do dinheiro digital. Para ajudar a resolver isso, Nick sugeriu algum tipo de ‘banco livre’ funcionando sobre o BitGold, que poderia agregar diferentes grupos de hashes que teriam o mesmo valor.

##### B-Money

Logo após a proposta do Bit Gold, Wei Dai propôs uma solução semelhante. Ele já havia desenvolvido várias outras ferramentas para os Cypherpunks e tinha suas próprias ideias sobre dinheiro digital.

Sua proposta se assemelhava ao Bit Gold no sentido de usar assinaturas digitais para transferir dinheiro, e os registros das transações seriam armazenados em um livro-razão, contendo chaves públicas e a quantidade de unidades de moeda atribuídas a cada uma. Assim como no Bit-Gold, terceiros confiáveis eram considerados falhas de segurança, e acreditava-se que um sistema de dinheiro eletrônico não deveria depender de uma única entidade para rastrear saldos, transações ou para evitar o gasto duplo.

Wei-Dai propôs várias soluções para essas questões, uma das quais era que, em vez de uma entidade central manter o livro-razão, TODOS os nós manteriam uma cópia. Se todos os usuários verificassem seu próprio livro-razão e a validade de cada transação, enquanto todos os nós permanecessem atualizados, os livros-razão deveriam permanecer sincronizados em toda a rede. Esse sistema altamente distribuído seria difícil de corromper.

Wei Dai reconheceu que isso não resolvia o problema dos generais bizantinos (1), pois os nós poderiam facilmente perder a sincronização ou simplesmente mentir. Ele sugeriu métodos alternativos, como ter um subconjunto de servidores ‘confiáveis’ que mantivessem o livro-razão e criar incentivos financeiros para manter esses servidores honestos.

Para a política monetária, ele propôs atrelar o poder de compra do B-Money a algum tipo de índice de preços ao consumidor externo. Ele queria que a mesma quantidade de B-Money pudesse comprar uma fração igual do índice ao longo do tempo, proporcionando alguma estabilidade de preços. Assim, qualquer pessoa poderia gerar novas unidades de moeda fornecendo um hash válido, mas a dificuldade de gerar um hash poderia mudar ao longo do tempo com base nos custos de CPU e no índice de preços, de modo que cada unidade seria ‘imutável’.
