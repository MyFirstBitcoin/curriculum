# 8.4 A Transação do Dia da Pizza

Até agora, este módulo concentrou-se em usar a natureza aberta do livro-razão do Bitcoin para compilar métricas úteis a partir de dados agregados de transações. No entanto, é possível usar dados do livro-razão e exploradores de blocos para examinar transações reais e rastrear o movimento de fundos dentro da rede.

Todo ano, no dia 22 de maio, a comunidade Bitcoin homenageia Laszlo Hanyecz, que se tornou a primeira pessoa registrada a usar bitcoin para comprar bens físicos. Em 18 de maio de 2010, Hanyecz anunciou em um fórum do Bitcointalk.org que estava procurando pizza e estava disposto a pagar em BTC. Ele ofereceu 10.000 BTC para quem estivesse disposto a realizar a transação. Ele esperou por vários dias, até que o estudante de 19 anos Jeremy Sturdivant aceitou e enviou duas pizzas grandes.

O **Dia da Pizza** pode ser visualizada por qualquer pessoa e possui o seguinte ID de transação:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Inserindo este ID de transação em [mempool.space](https://mempool.space) revela o seguinte:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Data e hora da transação: 22 de maio de 2010

Taxa de transação na rede: 99.000.000 sats (na época equivalia a menos de 1 centavo de dólar. Em maio de 2025, isso equivale a US$ 95.072,67)

Altura do Bloco: 57.043

Número de Confirmações: 838.645 (este é o número de blocos adicionados ao livro-razão após esta transação)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Número de Entradas da Transação: 131

Número de Saídas da Transação: 1

Clicando na chave pública de saída (terminando em `XaxFyQ`) que sabemos que pertencia a Jeremy Sturdivant, que recebeu 10.000 BTC por duas pizzas, revela o seguinte:

Este endereço atualmente possui um saldo de 0,00257879 BTC e parece ter participado de 14 transações, sendo a mais recente em 13 de dezembro de 2024.



#### 8.4.1 Atividade: Discussão em Grupo

1. Descreva os benefícios (por exemplo, auditoria, responsabilidade) ou riscos (por exemplo, preocupações com privacidade) para indivíduos ou empresas que utilizam um sistema de transações tão transparente e aberto.
1. Como esse tipo de transparência financeira pode afetar setores como caridade, compras governamentais, remessas ou aplicação da lei?
1. Os sistemas bancários tradicionais deveriam oferecer um nível semelhante de visibilidade? Eles serão forçados a isso pelo mercado?
