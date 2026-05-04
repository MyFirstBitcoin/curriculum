# 8 - Como o Bitcoin Funciona

Duração: 90 minutos

Ideia Central: A segurança do Bitcoin depende de ideias técnicas simples, mas poderosas, como chaves, assinaturas, hashing e UTXOs, que permitem a posse e a verificação sem uma autoridade central.

#### Objetivos de Aprendizagem

Ao final desta aula, os alunos deverão ser capazes de:

* Explicar como as chaves públicas e privadas ajudam a proteger a posse e as transações de Bitcoin.
* Descrever o que é uma assinatura digital e como ela prova que uma transação foi autorizada pelo verdadeiro proprietário.
* Explicar, em termos simples, o que significam criptografia, encriptação e decriptação no contexto do Bitcoin.
* Definir hashing e descrever por que as funções hash são importantes para a segurança e integridade dos dados do Bitcoin.
* Identificar propriedades básicas de uma função hash, como saída de comprimento fixo, comportamento unidirecional e sensibilidade a pequenas mudanças na entrada.
* Explicar o modelo UTXO e como o bitcoin é gasto, recebido e devolvido como troco através das saídas de transação.
* Descrever como os nós ajudam a evitar o duplo gasto verificando se uma saída já foi gasta.

#### Ferramentas e Recursos

##### Recursos Visuais

* Capítulo 8 - Como o Bitcoin Funciona

##### Biblioteca de Apoio

* Cartão de Referência de Vocabulário — Capítulo 8 — Termos: criptografia, hash, UTXO, assinatura digital, chave privada/pública, árvore de merkle, blockchain
* Bibliotecas de Equívocos — Capítulo 8 — Aborda: "frase-semente perdida pode ser recuperada", "chave privada = senha", "blockchain é anônima"
* Explicações Técnicas & Aprofundamentos — Funções hash, chaves públicas/privadas, modelo UTXO, segurança da Prova de Trabalho

#### Atividades

* Transações em Ação
* Explorando o Mempool

#### Ensino Online

* Use um quadro branco digital e desenhe cada conceito ao vivo em vez de depender apenas da explicação verbal.
* Ensine uma ideia técnica de cada vez e faça pausas frequentes para perguntas de verificação.
* Use recursos visuais para chaves, assinaturas, hashes e UTXOs para que os alunos possam acompanhar a estrutura.
* Mantenha o objetivo conceitual e evite aprofundar demais em matemática ou jargões.

#### Preparação

* Prepare e plastifique diagramas: pares de chaves públicas/privadas, assinaturas digitais, modelo UTXO, hashing (função unidirecional).
* Adicione aos favoritos um explorador de blockchain e uma calculadora de hash SHA-256; selecione 2-3 transações reais de Bitcoin para analisar passo a passo.
* Prepare anotações no quadro branco para explicar entradas, saídas e como as transações são confirmadas na blockchain.

#### Procedimento

Esta aula oferece aos alunos um primeiro contato com o lado técnico do Bitcoin sem pressupor conhecimento técnico prévio. O guia agora segue a mesma estrutura condensada do Diploma, com a criptografia agrupada sob um título e os UTXOs sob outro.

##### 8.0 Introdução, 8 minutos

Comece estabelecendo expectativas:

* O que torna o Bitcoin seguro se não há um banco central controlando?
* Como a rede pode saber se uma pessoa realmente possui o bitcoin que está tentando enviar?
* O que realmente acontece nos bastidores quando alguém faz uma transação de Bitcoin?

Deixe claro que este capítulo foca nas bases técnicas do Bitcoin, especialmente chaves, assinaturas, hashing e UTXOs. Reforce também que os alunos não precisam se tornar engenheiros para entender a lógica essencial. O próprio capítulo deixa isso claro ao comparar o Bitcoin à internet: muitas pessoas a usam todos os dias sem entender completamente todas as camadas por trás.

##### 8.1 Segurança através da Criptografia, 57 minutos

**Bitcoin como um Livro-razão Armazenado em Muitos Computadores**

Comece com a explicação simples do capítulo sobre a rede Bitcoin:

* Bitcoin é um registro de transações
* esse registro é armazenado em muitos computadores chamados nós
* o livro-razão é público e pseudônimo
* ele mostra endereços e histórico de transações, não detalhes de identidade pessoal

Esta seção ajuda os alunos a se conectarem com o que já sabem dos capítulos anteriores. O Bitcoin não se baseia em contas ocultas dentro de um banco. Ele se baseia em um livro-razão compartilhado que muitos participantes podem verificar. é especialmente útil aqui porque mostra usuários, carteiras e a rede Bitcoin mais ampla conectados ao livro-razão público.

**Chaves Públicas e Privadas**

Agora entre em criptografia.

Explique que cada usuário de Bitcoin possui:

* uma chave privada, que deve permanecer secreta
* uma chave pública, que pode ser compartilhada

Esclareça o propósito delas em termos simples:

* a chave privada comprova o controle e autoriza o gasto
* a chave pública ajuda os outros a verificar que a transação foi autorizada corretamente

Um ponto forte de ensino do capítulo é que o Bitcoin usa criptografia de chave pública/privada, e não o modelo antigo em que duas pessoas precisam primeiro compartilhar a mesma chave secreta. Isso é importante porque permite uma verificação segura sem obrigar os usuários a revelar o segredo que protege seus fundos.

Você pode explicar assim:

* a chave privada é como a prova secreta de que o bitcoin pertence a você
* a chave pública faz parte do que permite à rede verificar sua autorização
* quem controla a chave privada controla a capacidade de gastar o bitcoin

Tome cuidado aqui para não complicar demais a linguagem de criptografia. O ponto mais importante para os alunos é propriedade e autorização.

**Assinaturas Digitais e Autorização de Transações**

Agora explique o que acontece quando alguém envia bitcoin.

Use a sequência do capítulo:

* um usuário cria uma transação
* o remetente gera uma assinatura digital usando sua chave privada
* a transação é transmitida para a rede
* os nós verificam se a assinatura é válida
* uma vez verificada e confirmada, a propriedade é transferida no registro

Deixe claro que uma assinatura digital não é a mesma coisa que digitar um nome. É uma prova criptográfica de que o verdadeiro dono autorizou a transação. Esse é um dos mecanismos centrais que permite ao Bitcoin funcionar sem uma autoridade central aprovando transações manualmente. O diagrama é útil porque mostra visualmente a assinatura e a verificação, assim como o caminho da transação do remetente até a validação pela rede.

Uma boa frase para a aula é:

As transações de Bitcoin não são aprovadas porque um banco diz que sim. Elas são aceitas porque a rede pode verificar uma prova criptográfica válida.

**Hashing e Funções Unidirecionais**

Em seguida, explique o hashing.

Comece simples:

* uma função recebe uma entrada e produz uma saída
* uma função unidirecional é fácil de executar em uma direção, mas praticamente impossível de reverter
* uma função hash recebe dados de qualquer tamanho e transforma em uma saída de tamanho fixo chamada hash

Use uma das analogias do capítulo, a que parecer mais clara para seu público:

* a analogia do smoothie para funções unidirecionais
* a analogia da impressão digital para hashes
* a analogia da partitura musical para checar se algo mudou

A analogia da impressão digital provavelmente é a mais clara para a maioria das turmas:

* um hash é como uma impressão digital digital para dados
* se a entrada muda mesmo que um pouco, o hash muda completamente
* isso ajuda os computadores a checar a integridade e detectar adulterações

Depois explique por que o hashing é importante no Bitcoin:

* as transações são hasheadas
* a rede usa hashes para ajudar a verificar a integridade
* se uma transação for alterada, o hash muda
* isso ajuda a proteger o registro contra manipulação despercebida

Os visuais das páginas 7 a 10 são muito úteis aqui. O capítulo mostra tanto a ideia de saída de tamanho fixo quanto o princípio de "pequena mudança, resultado completamente diferente", que é um dos conceitos mais importantes para os alunos entenderem.

**Propriedades Básicas das Funções Hash**

Passe rapidamente pelas propriedades destacadas no capítulo, sem torná-las excessivamente acadêmicas:

* Determinística: a mesma entrada gera a mesma saída sempre
* Unidirecional / resistência à pré-imagem: você não pode realisticamente reverter o processo
* Sensível a mudanças: mesmo uma pequena alteração na entrada gera uma saída muito diferente
* Resistência a colisão: é extremamente difícil encontrar duas entradas diferentes com a mesma saída
* Rápida de verificar: a função é eficiente para executar e checar

Você não precisa que os alunos memorizem todos os termos, mas eles devem entender o ponto geral: o hashing dá ao Bitcoin uma forma confiável de identificar dados e detectar alterações.

##### 8.2 O Modelo UTXO, 25 minutos

**O Modelo UTXO**

Agora passe para a segunda parte principal do capítulo: UTXOs, ou Saídas de Transações Não Gastas.

Explique de forma simples usando a analogia do dinheiro em espécie do capítulo:

* o bitcoin não é acompanhado como um saldo de conta bancária apenas
* em vez disso, ele é composto por pedaços gastáveis chamados UTXOs
* quando você gasta bitcoin, você usa um ou mais UTXOs existentes como entradas
* novos UTXOs são então criados como saídas

Use o exemplo do capítulo:

* se você tem um UTXO de 10 BTC
* e você envia 6 BTC
* um novo UTXO de 6 BTC vai para o destinatário
* um novo UTXO de troco volta para você
* uma pequena parte é paga como taxa para o minerador

Isso ajuda os alunos a perceberem que o Bitcoin funciona mais como gastar dinheiro em espécie e receber troco do que simplesmente subtrair números de uma linha de conta. Os diagramas são especialmente eficazes aqui porque mostram visualmente um UTXO sendo dividido em saída para o destinatário, saída de troco e taxa.

Deixe dois pontos-chave explícitos:

* o saldo da sua carteira é a soma dos seus UTXOs
* quando você gasta, os UTXOs antigos são consumidos e novos são criados

**Prevenindo o Duplo Gasto**

Encerre o conteúdo explicando uma das implicações mais importantes do modelo UTXO.

Se alguém tentar gastar a mesma saída duas vezes, os nós rejeitam a segunda tentativa porque mantêm o registro e podem verificar se aquele UTXO já foi gasto. É assim que o Bitcoin previne o duplo gasto sem precisar de uma empresa central de pagamentos para gerenciar os registros. O exemplo é muito útil aqui porque mostra Alice combinando UTXOs, enviando fundos para Bob, recebendo troco e tendo a transação confirmada atualizando o registro em todos os nós.

Uma forma clara de dizer isso em sala é:

O Bitcoin previne o duplo gasto porque a rede acompanha quais saídas permanecem não gastas e quais já foram usadas.

###### Encerramento e Verificação de Compreensão

Encerre com algumas perguntas rápidas:

* Qual é a diferença entre uma chave pública e uma chave privada?
* O que uma assinatura digital comprova?
* Por que a função de hash é útil no Bitcoin?
* O que acontece se uma transação for alterada depois de ser hasheada?
* O que é um UTXO em termos simples?
* Como a rede impede que alguém gaste o mesmo bitcoin duas vezes?

#### Notas para Educadores

Este capítulo contém uma linguagem mais técnica do que os anteriores, então priorize clareza, analogias e repetição.

O objetivo não é transformar os alunos em desenvolvedores. O objetivo é ajudá-los a entender por que a segurança do Bitcoin funciona.

Os pontos mais importantes para priorizar, se o tempo for curto, são:

* chave privada vs chave pública
* assinaturas digitais
* o que o hash faz
* UTXOs como pedaços gastáveis de bitcoin
* como o duplo gasto é prevenido

Os visuais mais úteis deste capítulo são:

* o diagrama usuário-carteira-rede
* o visual da assinatura digital
* os exemplos de hash e diagramas de saída de comprimento fixo nas páginas 7 a 10
* os diagramas de UTXO nas páginas 10 a 12

##### O Que é um Bom Resultado

* É importante tratar a criptografia como uma base e não um mistério, usar muitos recursos visuais, evitar matemática profunda, conectar com capítulos anteriores e testar a compreensão com aplicações como "Se alguém altera uma transação, o que quebra?"
* Os educadores devem ser pacientes com alunos que têm dificuldades, pensar visualmente e desenhar tudo, ser honestos sobre o que os alunos não precisam entender, estar dispostos a dizer "Não sei, mas aqui está como descobriríamos", e permanecer encorajadores durante todo o processo.
* Os alunos entendem por que o Bitcoin não pode ser hackeado porque é protegido por matemática, respeitam o design elegante do sistema, sentem-se confortáveis com a complexidade sabendo que não precisam de todos os detalhes, ganham confiança para fazer perguntas sem julgamento e reconhecem que avançaram na compreensão de algo que a maioria das pessoas não entende.
* Os Resultados de Aprendizagem devem ser alcançados se os alunos conseguirem explicar o básico da criptografia como funções unidirecionais e assinaturas digitais sem matemática profunda, entender o modelo UTXO mostrando que você possui moedas e não contas, reconhecer o hash como a base da segurança do Bitcoin, entender a anatomia das transações incluindo assinaturas e confirmações, explicar por que o Bitcoin é imutável e fazer perguntas críticas sobre possíveis ataques ou vulnerabilidades.

##### Gestão do Tempo

Se o tempo for curto, priorize:

* Chave privada vs chave pública
* Assinaturas digitais
* O que o hashing faz
* UTXOs como partes gastáveis de bitcoin
* Como a dupla despesa é evitada

Se estiver adiantado, dedique tempo a:

* Diagrama usuário-carteira-rede e modelo visual de segurança
* Visualização da assinatura digital: processo criptográfico detalhado
* Árvores de Merkle e segurança da cadeia
* Vetores de ataque avançados e por que falham

##### Se os alunos tiverem dificuldade

* Criptografia como ameaça → "Você a usa diariamente; o Bitcoin usa da mesma forma."
* Hashing como conceito → Analogia da impressão digital; único, não pode ser alterado sem mudar o hash.
* Assinaturas digitais → "Prova autorização sem revelar a senha."
