# 6 - Como Usar o Bitcoin

Duração: 90 minutos

Ideia Central: Usar o Bitcoin on-chain ensina aos alunos como funcionam, na prática, a posse, a autocustódia e a verificação, transformando teoria em ação financeira direta.

#### Objetivos de Aprendizagem

Ao final desta aula, os alunos deverão ser capazes de:

* Identificar formas comuns de adquirir e trocar bitcoin, incluindo métodos peer-to-peer e de corretoras centralizadas.
* Explicar a diferença entre carteiras autocustodiais e custodiais, e por que a autocustódia é importante no Bitcoin.
* Descrever a finalidade das chaves privadas, endereços públicos, frases-semente e interfaces de carteira.
* Comparar diferentes tipos de carteiras e avaliar seus prós e contras em termos de segurança, conveniência, privacidade e controle.
* Configurar uma carteira de Bitcoin no celular e explicar o processo básico de recuperação.
* Demonstrar como receber e enviar uma transação de bitcoin on-chain.

Aplicar o princípio "Não Confie, Verifique" na escolha da carteira, nas transações e no uso mais amplo do Bitcoin.

#### Ferramentas & Recursos

##### Recursos Visuais

* Capítulo 6 - Como Usar o Bitcoin

##### Biblioteca de Apoio

* Cartão de Referência de Vocabulário — Capítulo 6 — Termos: carteira, chave privada, endereço público, frase-semente, custodial, autocustodial, UTXO, taxa de transação
* Tabelas Comparativas & Folhas de Referência — Comparação de tipos de carteiras (custodial, mobile, hardware, papel)
* Explicações Técnicas & Explorações Profundas — Chaves públicas/privadas, modelo UTXO, confirmação de transação
* Exploração Profunda de Segurança de Chaves Privadas — Frases-semente, derivação de chaves, métodos de backup, vetores de ataque
* Guia de Anatomia da Transação — Exemplo passo a passo de como funciona uma transação de Bitcoin
* Checklist de Melhores Práticas de Segurança — Antes de começar, criar carteira, receber, enviar, prevenção de phishing

#### Atividades

* Transações na Prática
* Corrida de Revezamento Lightning
* Explorando o Mempool

#### Ensino Online

* Deixe claro desde o início se os alunos estão apenas assistindo a uma demonstração ou se vão configurar uma carteira por conta própria.
* Use capturas de tela grandes e legíveis para cada etapa da configuração da carteira.
* Pause após cada etapa e peça para os alunos confirmarem a compreensão no chat antes de continuar.
* Dê um aviso direto antes da seção sobre frase-semente e lembre os alunos de nunca compartilhar informações sensíveis online.

#### Preparação

* Baixe e teste um aplicativo de carteira móvel (Blue Wallet ou Muun); prepare capturas de tela das principais etapas de configuração.
* Prepare um guia de configuração da carteira (baixar → criar → backup da semente → receber) para referência.
* Garanta que a rede/WiFi esteja funcionando; tenha um endereço de demonstração e QR code prontos para mostrar.

#### Procedimento

Esta aula passa da teoria para a prática direta. Agora ela corresponde diretamente à estrutura do Diploma, de modo que aquisição, carteiras, configuração, transações e verificação aparecem sob os mesmos títulos principais do guia do aluno. Apoio extra ao ensino permanece inserido nessas seções.

##### 6.0 Introdução, 8 minutos

Comece conectando este capítulo ao anterior:

* Se o Bitcoin é dinheiro, como as pessoas realmente o obtêm e usam?
* O que significa realmente controlar seu bitcoin?
* Por que usar Bitcoin é diferente de usar um aplicativo bancário?

Deixe claro que este capítulo trata do uso prático. Os alunos não estão mais apenas aprendendo o que é Bitcoin, eles estão aprendendo como interagir diretamente com ele.

##### 6.1 Adquirindo e Trocando Bitcoin, 12 minutos

Explique que as pessoas podem adquirir bitcoin de diferentes formas, incluindo:

* receber pagamento em bitcoin
* minerar bitcoin
* trocar dinheiro fiduciário por bitcoin pessoalmente
* trocar dinheiro fiduciário por bitcoin online

Depois, foque nas duas principais formas de aquisição abordadas no capítulo:

* peer-to-peer, presencialmente
* peer-to-peer, online
* corretoras centralizadas

Deixe claros os prós e contras.

Para P2P presencial, enfatize a troca direta sem um banco ou intermediário, mas também mencione os riscos práticos de encontrar pessoas para negociações em dinheiro.

Para P2P online, explique o escrow (serviço de custódia) em termos simples, como uma forma de reduzir o risco da contraparte, permitindo ainda a troca direta entre pares.

Para corretoras centralizadas, deixe claro que elas são convenientes, mas exigem que os usuários confiem em uma empresa, geralmente compartilhem informações pessoais e deixem os fundos sob controle de terceiros até o saque. Este é um bom momento para reforçar que a conveniência geralmente vem com concessões em privacidade e soberania.

##### 6.2 Uma Introdução às Carteiras de Bitcoin, 35 minutos

**O que realmente é uma Carteira de Bitcoin**

Esclareça um equívoco comum imediatamente: o bitcoin não é armazenado dentro do aplicativo da carteira como dinheiro físico em uma bolsa.  
O bitcoin existe no registro mantido pela rede. O que o usuário controla é a capacidade de gastá-lo por meio das chaves privadas.

Depois explique as duas coisas que as pessoas geralmente querem dizer com "carteira":

* o sistema de chaves privadas, a partir do qual os endereços são gerados
* o aplicativo ou interface usado para interagir com a rede

Use a analogia do e-mail do capítulo, se for útil:

* endereço público = como um endereço de e-mail que você pode compartilhar
* chave privada = como uma senha que você deve proteger

Seja muito claro aqui: quem controla as chaves privadas controla o bitcoin. Esse é o conceito central que os alunos precisam entender.

**Carteiras de Autocustódia vs Carteiras de Custódia**

Esta é uma das partes mais importantes do capítulo.

Explique claramente a diferença:

* Carteira de autocustódia: o usuário controla as chaves privadas
* Carteira de custódia: um terceiro controla as chaves privadas em nome do usuário

Depois explique os prós e contras:

Autocustódia

* controle total sobre os fundos
* sem processo de aprovação
* proteção contra confisco arbitrário
* maior responsabilidade
* não há recuperação fácil se a frase-semente for perdida

Custódia

* recuperação e suporte mais fáceis
* mais simples para iniciantes
* mais exposto a congelamento de contas, ataques e controle de terceiros
* o usuário não detém realmente o bitcoin

Este é o momento certo para enfatizar a frase:

"Se não são suas chaves, não são suas moedas."

Os alunos devem sair desta seção entendendo não só o slogan, mas o que ele realmente significa na prática.

**Diferentes Tipos de Carteiras e Como Escolher Uma**

Apresente os tipos de carteiras abordados no capítulo:

* carteira online
* carteira móvel
* carteira de desktop
* carteira hardware
* carteira de papel

Não trate nenhuma como perfeita. Em vez disso, explique que cada uma envolve concessões entre:

* segurança
* privacidade
* conveniência
* compatibilidade
* taxas
* controle
* reputação

Também deixe claro que recomendamos prestar atenção se o software da carteira é de código aberto, pois ferramentas open-source podem ser revisadas, auditadas e mantidas pela comunidade. Isso se conecta diretamente ao princípio da verificação no Bitcoin.

##### 6.3 Configurando uma Carteira Bitcoin no Celular, 10 minutos

Guie os alunos pelo processo básico mostrado no capítulo:

* baixar a carteira
* criar uma nova carteira
* gerar e anotar a frase de recuperação
* confirmar a frase de recuperação
* adicionar segurança extra, se disponível
* abrir a carteira e encontrar a função de receber

Deixe o aviso sobre a seed phrase (frase-semente) muito explícito:

* se a frase-semente for perdida, o acesso aos fundos pode ser perdido
* se outra pessoa obtiver a frase-semente, ela pode pegar os fundos

Se os alunos estiverem fazendo isso na prática, o educador deve pausar em cada etapa e verificar se todos entenderam o que estão fazendo. Se a aula for mais conceitual, esta seção pode ser explicada como um passo a passo, em vez de ser realizada ao vivo. A opção de recuperação mostrada no capítulo também é útil para explicar que as carteiras podem ser restauradas se a frase-semente foi salva corretamente.

##### 6.4 Recebendo e Enviando Transações, 17 minutos

**Recebendo e Enviando Transações On-chain**

Agora explique como funcionam as transações on-chain.

Para receber bitcoin:

* abra a carteira
* toque em receber ou depositar
* copie o endereço, compartilhe o link ou mostre o QR code

Para enviar bitcoin:

* abra a carteira
* cole ou escaneie o endereço do destinatário
* insira o valor
* confira todos os detalhes
* transmita a transação
* aguarde a confirmação

Deixe estes pontos-chave claros:

* a transação transfere a propriedade, não moedas físicas
* as transações são irreversíveis
* os nós verificam a validade
* os mineradores incluem as transações nos blocos
* as taxas influenciam a prioridade de confirmação
* as transações on-chain geralmente são seguras, mas mais lentas e frequentemente mais caras do que as transações Lightning

O diagrama do fluxo de transação no capítulo é especialmente útil aqui, pois ajuda os alunos a visualizarem o caminho do pedido da carteira até a confirmação na rede.

**Transações na Prática e Exercício por Papéis**

Use a estrutura de exercício cooperativo do capítulo para reforçar o entendimento. Explique os quatro papéis envolvidos:

* remetente
* destinatário
* minerador
* operador de nó

Uma abordagem simples em sala de aula é atribuir papéis e percorrer uma transação passo a passo. Isso ajuda os alunos a verem que uma transação Bitcoin não é mágica, é um processo coordenado que envolve aprovação, verificação, inclusão em bloco e atualização do registro.

O objetivo aqui não é profundidade técnica. É ajudar os alunos a entenderem quem faz o quê em uma transação e por que a verificação é importante.

##### 6.5 Não Confie, Verifique, 8 minutos

Explique que isso se aplica a:

* carteiras
* corretoras
* aplicativos
* detalhes da transação
* afirmações sobre "lucros fáceis"
* projetos que fingem ser como o Bitcoin

Deixe claro que o Bitcoin exige que os usuários pensem criticamente, verifiquem o que estão usando e evitem confiar cegamente. Explique também por que ferramentas de código aberto são importantes nesse contexto: elas tornam possível a verificação independente.

###### Encerramento e Verificação de Compreensão

Encerre com algumas perguntas rápidas:

* Qual é a diferença entre uma carteira custodial e uma carteira de autocustódia?
* Por que a frase-semente é tão importante?
* O que acontece quando você envia uma transação on-chain?
* Por que as transações on-chain são mais lentas do que alguns outros pagamentos em Bitcoin?
* O que significa "Não confie, verifique" na prática?

#### Notas para Educadores

Este capítulo é altamente prático, então priorize clareza, segurança e repetição.

Os alunos não precisam dominar todos os tipos de carteira em uma única aula. Os principais objetivos são:

* compreender o básico sobre carteiras
* compreender a autocustódia
* aprender o fluxo básico de uma transação
* adotar uma mentalidade responsável de verificação

Tenha cuidado especial ao discutir frases-semente e a configuração da carteira. Os alunos devem sair entendendo que esses não são detalhes pequenos, mas sim a base da posse de Bitcoin.

Os recursos visuais e atividades mais úteis deste capítulo são:

* a comparação entre autocustódia e custódia
* a tabela de prós e contras dos tipos de carteira
* o exercício passo a passo de configuração de carteira
* o diagrama do fluxo de transação
* a atividade de transação baseada em papéis

##### O Que é Considerado Bom

* É importante que os alunos realmente configurem uma carteira ou assistam a uma demonstração cuidadosa, coloquem a frase-semente como peça central com "Estas 12 palavras SÃO o seu Bitcoin", testem cenários como "O que acontece se você perder o celular?" e pratiquem o reconhecimento de phishing.
* Os educadores devem ser guias práticos que já fizeram isso antes, serem conscientes sobre segurança sem paranoia e serem honestos sobre a curva de dificuldade e o aprendizado necessário.
* Os alunos sentem que aprenderam uma habilidade real que podem usar, entendem que a frase-semente é real e importante e não algo abstrato, sentem-se capazes de custodiar seu próprio Bitcoin e entendem que a descentralização exige responsabilidade pessoal.
* Os Resultados de Aprendizagem devem ser alcançados se os alunos conseguirem configurar uma carteira e entender a diferença entre chaves públicas e privadas, compreender os prós e contras entre carteiras custodiais e de autocustódia, explicar como funciona uma transação incluindo entradas, saídas e taxas, demonstrar consciência de segurança incluindo proteção da frase-semente e fazer perguntas críticas sobre posse e controle.

##### Gestão do Tempo

Se o tempo for curto, priorize:

* Compreender o básico sobre carteiras
* Compreender a autocustódia
* Aprender o fluxo básico de uma transação
* Adotar uma mentalidade responsável de verificação

Se houver tempo de sobra, dedique-se a:

* Tabela de comparação entre autocustódia e custódia
* Tabela de prós e contras dos tipos de carteira
* Exercício passo a passo de configuração de carteira com demonstração ao vivo
* Diagrama do fluxo de transação com cálculo de taxas
* Práticas avançadas de segurança e considerações sobre carteiras hardware

##### Se os Alunos Tiverem Dificuldade

* Frases-semente como "reais" → "Esta frase É o seu bitcoin; não existe atendimento ao cliente."
* Chaves públicas vs. privadas → Analogia com e-mail (endereço vs. senha).
* Por que é difícil → "Você controla; você é responsável." Reconheça o trade-off.
