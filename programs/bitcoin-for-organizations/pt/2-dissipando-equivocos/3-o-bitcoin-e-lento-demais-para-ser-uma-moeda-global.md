# 2.3 O Bitcoin é lento demais para ser uma moeda global.

> Visionários veem um futuro de trabalhadores em home office, bibliotecas interativas e salas de aula multimídia. Falam sobre reuniões municipais eletrônicas e comunidades virtuais... A verdade é que nenhum banco de dados online substituirá seu jornal diário, nenhum CD-ROM pode ocupar o lugar de um professor competente e nenhuma rede de computadores mudará a forma como o governo funciona.  
_Clifford Stroll_

17 anos depois, a Newsweek encerrou sua publicação impressa e passou a estar disponível exclusivamente online. Imagine estar vivo em 1974, quando o Protocolo de Controle de Transmissão (TCP) foi criado pela primeira vez.

Ninguém previu o smartphone, com todos os seus aplicativos, na palma da sua mão. Ninguém imaginou o sistema de navegação por satélite no seu carro.

A internet não surgiu de uma vez só, mas sim gradualmente, como uma evolução de protocolos e camadas. Essas evoluções se basearam no TCP, mas principalmente não o alteraram.

> Portanto, ao pensar na transição para as plataformas de comunicação do futuro, vejo que a beleza dos protocolos da Internet está na separação das camadas entre serviço e tecnologia.  
_Michael K Powell_



##### Compare a evolução do Bitcoin com a da internet

O TCP foi necessário, mas não suficiente para o surgimento de todo o resto na internet. A evolução do Bitcoin parece seguir um caminho semelhante. Sistemas abertos parecem ser mais resilientes e bem-sucedidos quando desenvolvidos em camadas, embora possa haver muito tempo decorrido entre a colocação dos blocos iniciais e a adoção em larga escala. Soluções tudo-em-um não parecem ser tão eficazes em sistemas abertos quanto aquelas construídas em camadas sobre protocolos. Assim como ninguém precisou reconstruir a internet porque filmes não podiam ser transmitidos usando TCP, é provável que o mesmo aconteça com o Bitcoin.

Já existem vários protocolos de camada 2 sobre o Bitcoin, e há muitos aplicativos construídos sobre esses protocolos de camada 2 (veja a seção 201.4 para mais detalhes sobre eles).

Em vez de focar no que o bitcoin e a rede Bitcoin não conseguem fazer hoje, pense no que já pode ser feito atualmente e compare isso com o que era possível há 10 anos. Faça esse exercício com a internet de 1985 a 1995 e depois veja o quanto a internet evoluiu nos 30 anos seguintes e as aplicações que se tornaram possíveis. Use esse insight para projetar o Bitcoin para frente e imaginar como ele pode ser em apenas mais 10 anos, ou 30, se sua imaginação alcançar tão longe.



##### Compare o Bitcoin com o sistema monetário global existente

A afirmação central de que o Bitcoin é muito lento para ser dinheiro global é, sem dúvida, verdadeira se estivermos restritos à camada base do Bitcoin. Também é verdade que a camada base dos nossos sistemas monetários atuais é muito lenta para ser dinheiro global, se uma restrição semelhante significasse que não existisse infraestrutura de pagamentos construída sobre ela por bancos privados e serviços de pagamento como Visa e Mastercard. Nosso sistema atual é construído em camadas, então podemos esperar que o futuro seja semelhante. Alguns compromissos de design, como entre confiança, velocidade e custo, podem ser traduzidos entre sistemas que entregam as mesmas soluções, embora sejam construídos para movimentar diferentes tokens de valor.

Algumas das camadas 2 já existentes no Bitcoin abordam diretamente a questão da velocidade, por exemplo, Liquid e a Lightning Network (veja a seção 201.4 para mais detalhes). Liquid é mais rápida e barata que a blockchain do Bitcoin, e a Lightning Network é ainda mais rápida e barata que a Liquid. Uma proliferação de camadas 2, cada uma com diferentes compromissos, é esperada e saudável.

Provavelmente haverá mais camadas 2 e 3 e uma explosão de aplicativos utilizando essas camadas, assim como aconteceu com a evolução da internet.



##### Motivação

Quando essa crítica é levantada, vale a pena considerar se o crítico tem outras motivações. Por exemplo, eles têm um projeto de blockchain novo ou diferente? Isso pode ser análogo a tentar vender um Protocolo de Controle de Transmissão melhor.

O Trilema da Escalabilidade, ou Blockchain, foi levantado pela primeira vez por Vitalik Buterin em 2017. Ele diz que sempre há um compromisso no design de blockchain entre as propriedades de Descentralização, Segurança e Escalabilidade. Qualquer um que levante a crítica de que o Bitcoin é muito lento e que tem uma solução mais rápida em uma blockchain de camada 1 estará sacrificando alguma segurança ou descentralização para conseguir isso. Embora tal compromisso para uma blockchain projetada para outros usos possa fazer sentido, a ordem de prioridade para um dinheiro global deve ser:


> **Light**
>
> * **Descentralização**
>   * Torna possível remover partes confiáveis
> * **Segurança**
>   * Inibe que agentes mal-intencionados adulterem transações ou o livro-razão
> * **Escalabilidade**
>   * Permite que o sistema escale economicamente em usuários e velocidade


As duas primeiras características criam o ambiente para emissão sem emissores, pagamentos sem intermediários e custódia sem gestores.

O Bitcoin faz o compromisso correto entre as três características de design de blockchain, dado que seu caso de uso alvo é como dinheiro global, e mitiga os compromissos de escalabilidade e velocidade usando camadas.

> Satoshi descobriu como proteger a integridade do dinheiro digital sem partes confiáveis – não são necessários emissores, intermediários ou gestores.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
