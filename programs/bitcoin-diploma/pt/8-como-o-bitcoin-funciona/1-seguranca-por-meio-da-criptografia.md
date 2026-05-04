# 8.1 Segurança por meio da Criptografia

> O que o Bitcoin nos oferece é uma promessa rígida: o programa será executado exatamente como especificado.  
_Andreas M. Antonopoulos_

#### Criptografia de Chave Pública/Privada


> **Definition – Definição de Criptografia**
>
> **Criptografia** é a prática de transformar informações em um segredo que só as pessoas certas podem ler.


* **Criptografia** é o processo de transformar informações em uma forma codificada para que apenas alguém com a chave correta possa lê-las.
* **Descriptografia** é o processo de transformar essa informação codificada de volta em algo legível.

Na criptografia tradicional, duas pessoas que querem se comunicar de forma privada precisam primeiro compartilhar a mesma chave secreta, semelhante a uma senha compartilhada. Uma pessoa usa essa chave para criptografar a mensagem antes de enviá-la, e a outra pessoa usa a mesma chave para descriptografar e ler.

O problema desse sistema é que ambas as pessoas já precisam compartilhar a chave secreta. Se outra pessoa tiver acesso a essa chave, poderá ler qualquer mensagem interceptada.

O Bitcoin resolve esse problema usando uma abordagem diferente chamada criptografia de chave pública, onde os usuários não precisam compartilhar chaves secretas antecipadamente.

A criptografia de chave pública/privada resolve o problema do compartilhamento de segredos. Em vez de compartilhar uma senha, cada pessoa tem duas chaves: uma chave pública e uma chave privada.

* A **chave pública** pode ser compartilhada com qualquer pessoa.
* A **chave privada** deve sempre ser mantida em segredo.

Se João quiser enviar algo para Ariel, ele pode usar a chave pública de Ariel. Somente Ariel pode desbloquear usando sua chave privada. Mesmo que alguém intercepte a mensagem, não poderá lê-la ou usá-la sem a chave privada.

No Bitcoin, esse sistema é usado para criar assinaturas digitais. Uma assinatura digital prova que o dono de uma chave privada aprovou uma transação, semelhante a assinar seu nome em um documento. É isso que permite que as transações de Bitcoin sejam seguras e verificáveis sem confiar em terceiros.

As transações de Bitcoin envolvem a transferência de propriedade de bitcoin de um endereço para outro.

A criptografia é usada para garantir que apenas o verdadeiro detentor do bitcoin tenha autoridade para enviar seu dinheiro para outra pessoa. Isso garante que sua propriedade esteja protegida contra agentes mal-intencionados.

Como uma medida adicional de proteção, cada transação de Bitcoin recebe automaticamente uma assinatura digital ÚNICA. Essa assinatura digital única é alimentada por uma tecnologia à prova de adulteração que ajuda a rede a verificar que o verdadeiro dono do bitcoin, e não outra pessoa, foi quem enviou.


> **Info**
>
> Cada usuário possui duas chaves: uma **chave privada**, que é **mantida em segredo**, e uma **chave pública** que pode ser **compartilhada com outros**. A **chave privada** serve como uma forma de identificação e prova de propriedade, confirmando: “Este endereço me pertence e eu tenho controle sobre ele.”


###### Como Funciona uma Transação de Bitcoin

1. **Criando a Transação**: Um usuário inicia uma transação de Bitcoin especificando detalhes como o endereço do destinatário e a quantidade de bitcoin a ser enviada.
1. **Geração da Assinatura Digital**: O remetente gera uma **assinatura digital** única usando sua **chave privada**. Essa assinatura é um código único que verifica a autenticidade da transação.
1. **Transmissão da Transação**: A transação assinada é transmitida para a rede Bitcoin, indicando a intenção de transferir a propriedade do bitcoin do remetente para o destinatário.
1. **Verificação na Rede**: Os nós da rede Bitcoin recebem a transação e usam a **chave pública** para verificar a autenticidade da assinatura da transação. Ao mesmo tempo, eles usam a **chave pública** para verificar a **assinatura digital**.
1. **Confirmação na rede Bitcoin**: Se a verificação for bem-sucedida, a transação será adicionada ao registro, que serve como um histórico seguro e transparente de todas as transações. Uma vez confirmada, a posse do bitcoin é oficialmente transferida do remetente para o destinatário.


> **Callout – Resumo**
>
> A **assinatura digital**, criada com a **chave privada** do remetente, prova que a transação foi autorizada pelo dono do bitcoin. A rede Bitcoin pode então verificar essa prova e registrar a transação.


#### Explicação sobre Hashing

Por favor, não se intimide com os termos técnicos e conceitos matemáticos a seguir. Sabemos que nem todo mundo gosta de matemática, mas você pode se surpreender e perceber que até as ideias mais complexas podem ser compreendidas com um pouco de esforço.


> **Definition – Definição de função**
>
> Uma **função** é como uma máquina que recebe uma informação e a transforma em algo novo. A informação que você fornece para a função é a **entrada**. A nova informação que a função cria é a **saída**. As funções ajudam os computadores a realizar tarefas e resolver problemas.


##### O que é uma função?

Uma função é um conjunto de instruções que recebe uma entrada e produz uma saída. Você pode pensar nela como uma receita: você segue os passos com certos ingredientes e sempre chega a um resultado previsível.

No Bitcoin, funções são usadas para processar e verificar transações. Quando alguém envia bitcoin, funções criptográficas ajudam a checar se a transação é válida, confirmar se o remetente tem saldo suficiente e atualizar os saldos no registro do Bitcoin. Uma vez verificada e adicionada a um bloco, a transação se torna parte do registro permanente na blockchain.

##### O que é uma função unidirecional?

Uma função unidirecional é um tipo especial de função que é fácil de calcular em uma direção, mas extremamente difícil de reverter. Por exemplo, bater ingredientes para fazer um smoothie é fácil, mas você não consegue separar o smoothie de volta nos ingredientes originais.

A segurança do Bitcoin depende de funções unidirecionais. Elas são usadas na criptografia de chave pública e privada, permitindo que as pessoas compartilhem uma chave pública enquanto mantêm sua chave privada em segredo. Mesmo que a chave pública seja visível, é impossível derivar a chave privada a partir dela. Isso é o que torna as transações de Bitcoin seguras.

##### O que é uma função hash?

Uma **função hash** é como uma máquina de códigos secretos. Ela recebe uma mensagem e a transforma em um código.

###### Como o Hashing Funciona nas Transações de Bitcoin

No Bitcoin, toda transação é transformada em um hash antes de ser adicionada à blockchain. Um hash é uma impressão digital única da transação. Se alguém tentar alterar até mesmo uma pequena parte da transação, o hash mudará completamente. Isso facilita para a rede detectar qualquer tentativa de adulteração.

###### O Papel do Hashing na Segurança do Bitcoin

O hashing ajuda a proteger a rede Bitcoin tornando as transações fáceis de verificar e impossíveis de modificar silenciosamente. Como cada transação tem seu próprio hash único, a rede pode detectar rapidamente se algo foi alterado.

Uma função hash recebe dados e os converte em uma sequência fixa de números e letras chamada hash. A mesma entrada sempre produzirá o mesmo hash, mas até mesmo uma pequena alteração na entrada criará um resultado completamente diferente. Essa propriedade permite que os computadores verifiquem se os dados não foram alterados.


> **Definition – Definição de Hashing**
>
> **Hashing** é como criar uma impressão digital para dados digitais. É o processo de pegar uma mensagem digital e transformá-la em um código de comprimento fixo, que serve como um identificador único. Assim como uma impressão digital pode identificar uma pessoa, um hash pode identificar uma mensagem digital.


A **saída**, ou hash, tem sempre o mesmo comprimento, não importa o tamanho da informação original. O Bitcoin utiliza alguns tipos específicos de função hash chamados **SHA-256** e **RIPEMD160**.

Veja alguns exemplos abaixo:

* Hash SHA256 da string **olá mundo**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hash SHA256 da string **olá mundo.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Perceba que uma pequena alteração na entrada muda completamente a saída quando comparada à primeira
* Hash SHA256 do arquivo iso para download **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Esta entrada é um arquivo enorme, mas a saída ainda tem o mesmo comprimento fixo

Você também pode pensar em hashing como uma partitura musical que captura a essência de uma peça de música. Assim como uma partitura é uma representação única de uma melodia, um valor de hash é uma representação única de um dado.

Ao comparar a partitura de uma música com a performance real, um músico pode determinar se a execução está correta. Da mesma forma, ao comparar o valor de hash dos dados recebidos com o valor de hash original, é possível saber se os dados foram alterados durante a transmissão.

Assim como uma pequena diferença em uma apresentação musical pode fazer com que ela soe diferente, até mesmo a menor alteração nos dados originais resultará em um valor de hash diferente. Isso faz do hashing uma ferramenta poderosa para garantir a integridade e autenticidade de uma transação de Bitcoin.

O processo de codificação da **chave pública** por meio do hashing é usado para melhorar a segurança das informações, convertendo-as em um formato de comprimento fixo e ilegível. O Bitcoin utiliza os algoritmos SHA-256 e RIPEMD160 para gerar endereços públicos. O resultado serve como um identificador único para a **chave pública** e ajuda a garantir a integridade e a segurança das transações armazenadas no livro-razão. Ao criptografar as informações dessa forma, torna-se mais difícil para pessoas não autorizadas acessarem e manipularem os dados.

##### Propriedades de uma função de hash

* **Determinística**: Os mesmos ingredientes sempre produzem o mesmo smoothie. Da mesma forma, os mesmos dados sempre produzirão o mesmo hash.
* **Resistência à pré-imagem**: Se você só tem o smoothie, não consegue descobrir exatamente quais frutas foram usadas. Da mesma forma, se você só tem o hash, não consegue determinar os dados originais.
* **Efeito avalanche**: Alterar até mesmo uma pequena parte dos ingredientes cria um smoothie completamente diferente. No hashing, uma mudança muito pequena nos dados produz um hash totalmente diferente.
* **Resistência a colisões**: É extremamente difícil encontrar dois conjuntos diferentes de ingredientes que produzam exatamente o mesmo smoothie. Da mesma forma, é extremamente improvável que dois dados diferentes produzam o mesmo hash.
* **Rápida para verificar**: Fazer o smoothie é rápido, e é fácil conferir que o resultado é um smoothie. Funções de hash são rápidas de calcular e fáceis de verificar por qualquer pessoa.

#### Atividade: Gere um Hash SHA 256

https://tools.keycdn.com/sha256-online-generator

Curioso para saber como o hashing funciona? Escaneie o código QR para gerar instantaneamente um hash SHA256 de qualquer palavra, frase ou entrada que você escolher. Funções de hash são como impressões digitais digitais: são unidirecionais, ou seja, uma vez que algo é hasheado, não pode ser revertido. Experimente e veja por si mesmo!
