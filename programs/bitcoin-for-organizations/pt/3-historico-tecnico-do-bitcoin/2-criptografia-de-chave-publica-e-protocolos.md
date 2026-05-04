# 3.2 Criptografia de Chave Pública e Protocolos

A Internet hoje, e a maioria dos sistemas computacionais modernos, dependem da criptografia, um método de ocultar informações para que apenas o destinatário possa decodificá-las. As bases da criptografia usada para proteger o Bitcoin remontam aos anos 70.

A primeira questão a ser resolvida é – como enviar um segredo compartilhado por um meio não seguro.

Isso foi analisado pela primeira vez por Whitfield Diffie e Martin Hellman.

O problema: as duas partes – geralmente chamadas de Alice e Bob – querem compartilhar informações secretas por uma rede onde outros podem estar ouvindo. Para isso, eles criaram o processo de troca de chaves Diffie-Hellman.

Esse segredo compartilhado pode então ser usado como valor inicial para criar várias chaves simétricas para criptografar e descriptografar mensagens entre si sem compartilhar a chave abertamente.

Como a chave privada nunca precisa ser compartilhada, e chaves diferentes são usadas em cada extremidade para criptografar e descriptografar, isso é chamado de algoritmo de criptografia assimétrica.

Casos de uso:

* Alice assina uma mensagem com a chave pública de Bob – que é a única pessoa que pode descriptografá-la usando sua chave privada
* Alice assina uma mensagem com sua chave privada – ao descriptografar com sua chave pública, qualquer pessoa pode verificar que a mensagem foi enviada por Alice, sem saber sua chave privada
* Combinando essas duas abordagens com duas camadas de criptografia, uma mensagem pode ser enviada criptografada de modo que apenas Bob possa descriptografá-la, e ele pode então verificar que o remetente foi realmente Alice

Embora não tenha sido creditado no artigo, Ralph Merkle foi fundamental para ajudar a resolver o que até então era considerado um enigma insolúvel – como estabelecer ou restabelecer comunicação privada em uma rede aberta e potencialmente hostil.

Essa abordagem, sozinha, é suscetível a um ataque de força bruta, onde um atacante pode pegar os números compartilhados e eventualmente recriar uma chave compartilhada, dado tempo e recursos suficientes, então não é a solução completa por si só.

##### Protocolos para Criptossistemas de Chave Pública

Além de contribuir para o sistema de chave pública Diffie-Hellman descrito acima, **Ralph Merkle** continuou a contribuir nesse campo por muitos anos, e foi fundamental no desenvolvimento de alguns componentes-chave usados pelo Bitcoin.

Uma função hash criptográfica é um algoritmo matemático que recebe entradas de qualquer tamanho e processa cálculos complexos para retornar um valor hash em bits, que geralmente é representado por uma saída alfanumérica de comprimento fixo usando o formato hexadecimal.

* As entradas podem ter qualquer tamanho
* A saída é sempre de comprimento fixo e determinística (a mesma entrada gera o mesmo hash toda vez)
* É fácil de verificar, mas extremamente difícil reverter o processo para determinar a entrada
* Uma pequena modificação nos dados altera completamente as saídas

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/9d0f91fd34e6f66f0699b1e6626bd6d6a3e29ab5-515x331.svg)

Hashing é parte integrante do protocolo Bitcoin. O SHA-256, usado no Bitcoin, foi criado pela NSA e é um exemplo de algoritmo de hash criptográfico.

* Cada bloco na cadeia é hasheado para que os dados não possam ser alterados – garantindo a integridade do livro-razão distribuído
* O hash gerado precisa atender aos critérios de ‘Prova de trabalho’ para ser considerado um bloco válido
* Árvores de Merkle – ao empregar ramificações e hashes de hashes, as árvores de hash permitem a verificação de grandes conjuntos de dados com armazenamento mínimo
* Assinaturas e chaves baseadas em hash podem ser usadas para carteiras, endereços e autorização de transações

A verificação distribuída dos estados do blockchain e modelos de livro-razão apenas para acréscimo, resistentes à revisão, é possibilitada pelo hashing unidirecional. Funções hash fornecem o método confiável e determinístico para verificar eventos em livros-razão públicos como o Bitcoin na ausência de um modelo de confiança centralizado.

Essas novas capacidades no campo da criptografia eram esperadas por seus criadores para inaugurar uma nova onda de inovação nesse espaço.

##### Criptografia de curva elíptica

Uma dessas inovações posteriores veio na forma da criptografia de curva elíptica.

A criptografia de curva elíptica foi introduzida em 1985 por dois cientistas, N. Koblitz e V. Miller. Eles propuseram a ideia de usar pontos definidos por curvas elípticas em vez dos campos primos finitos, de modo que a suposição do problema do Logaritmo Discreto se mantenha, como é comumente usado no protocolo padrão de troca de chaves Diffie-Hellman. Os detalhes de como isso funciona estão além do escopo desta seção, mas, em alto nível, uma curva elíptica é o conjunto de pontos que satisfazem uma equação matemática específica.

A equação para uma curva elíptica se parece com:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Isso tem algumas propriedades úteis:

* Simetria horizontal. Qualquer ponto na curva pode ser refletido sobre o eixo x e permanecer na mesma curva.
* qualquer linha não vertical irá interceptar a curva em no máximo três pontos.
* Tamanhos de chave compactos são essenciais para o armazenamento e transmissão eficientes de chaves públicas no blockchain.

Essas propriedades podem ser usadas para criar pares de chaves de forma semelhante ao algoritmo Diffie-Hellman. O Bitcoin usa ECDSA, que é a sigla para Algoritmo de Assinatura Digital de Curva Elíptica. É um processo que usa uma curva elíptica e um campo finito para “assinar” dados de tal forma que terceiros possam verificar a autenticidade da assinatura enquanto o assinante mantém a capacidade exclusiva de criar a assinatura. No bitcoin, os dados assinados são a transação que transfere a propriedade.

A parte ‘finita’ é semelhante à abordagem ‘mod’ do Diffie-Hellman, onde o resultado da equação é dividido e o resto é usado para garantir que ele se encaixe em um intervalo de números.
