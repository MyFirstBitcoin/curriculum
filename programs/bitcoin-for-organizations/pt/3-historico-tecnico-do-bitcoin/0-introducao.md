# 3.0 Introdução

> **Dark – Resumo do White Paper do Bitcoin**
>
> **Uma versão puramente peer-to-peer de dinheiro eletrônico** permitiria que pagamentos online fossem enviados diretamente de uma parte para outra sem passar por uma instituição financeira. **Assinaturas digitais fornecem parte da solução**, mas os principais benefícios são perdidos se uma **terceira parte confiável** ainda for necessária para evitar o duplo gasto. Propomos uma solução para o problema do duplo gasto usando uma **rede peer-to-peer**. A **rede carimba as transações com data e hora** ao hashá-las em uma cadeia contínua de **prova de trabalho baseada em hash,** formando um registro que não pode ser alterado sem refazer a **prova de trabalho**. A cadeia mais longa não serve apenas como prova da sequência de eventos testemunhados, mas também como prova de que ela veio do maior pool de poder computacional. Enquanto a maioria do poder computacional estiver controlada por nós que não cooperam para atacar a rede, eles gerarão a cadeia mais longa e superarão os atacantes. **A própria rede requer uma estrutura mínima. As mensagens são transmitidas com o melhor esforço possível, e os nós podem sair e retornar à rede quando quiserem**, aceitando a cadeia de prova de trabalho mais longa como prova do que aconteceu enquanto estavam ausentes.


O Bitcoin não surgiu do nada, mas sim se baseou no trabalho de muitos nas décadas anteriores. Este módulo irá explorar as fundações da internet sobre as quais o Bitcoin foi construído, assim como as pesquisas e desenvolvimentos reconhecidos no whitepaper.

Nos anos 70, um grupo de indivíduos observou como o governo dos EUA, em particular, estava tentando restringir o acesso à criptografia, e se empenhou para garantir que essa tecnologia estivesse disponível para todas as pessoas protegerem sua privacidade online. Alguns desses pioneiros também estavam focados nos potenciais benefícios de um sistema digital de 'dinheiro sólido' que pudesse ser usado para armazenar e trocar valor pela internet emergente. Friedrich Hayek – um dos principais contribuintes da escola austríaca de economia – já havia imaginado como seria uma moeda ideal baseada na competição de livre mercado, bem antes da internet, mas concluiu que isso era tecnicamente e politicamente inviável. Além da privacidade digital, esse grupo, que evoluiu para se tornar os Cypherpunks, tentou realizar a visão de Hayek para o dinheiro digital, mas essas tentativas fracassaram até que Satoshi publicou suas ideias na lista de discussão.

* Protocolo TCP/IP (1976)
* Protocolos para Criptossistemas de Chave Pública - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Carimbo Digital de Tempo (anos 90)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* POW Reutilizável - Hal Finney (2004)
* Whitepaper do Bitcoin - Satoshi Nakamoto (2008)

Uma influência fundamental no desenvolvimento do Bitcoin foi o surgimento do movimento Cypherpunk nos anos 1990. Eles desenvolveram várias tecnologias criptográficas, incluindo a criptografia de chave pública, para permitir que os usuários se comunicassem e compartilhassem informações de forma segura e privada. Muitos dos desenvolvimentos descritos aqui e as pessoas envolvidas faziam parte desse grupo.

A necessidade de dinheiro digital também foi identificada e várias tentativas foram feitas para criá-lo, mas essas tinham limitações que impediram seu sucesso. O gênio de Satoshi Nakamoto foi reunir essas capacidades e, junto com algumas inovações próprias, construir sobre elas para criar o protocolo Bitcoin em uso hoje. Nas próximas seções, exploraremos alguns desses desenvolvimentos e explicaremos como eles ajudaram a informar o design do Bitcoin. Também discutiremos quais eram as peças que faltavam no quebra-cabeça que Satoshi conseguiu resolver.
