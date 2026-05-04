# 2.7 O Bitcoin não é verdadeiramente descentralizado.

> A complexidade das criptomoedas surge das tentativas de descentralização—ao distribuir o poder e a governança no sistema, teoricamente não há necessidade de intermediários confiáveis como instituições financeiras. Essa era a premissa do white paper inicial do Bitcoin, que oferecia uma solução criptográfica destinada a permitir que pagamentos fossem enviados sem envolver qualquer instituição financeira ou outro intermediário confiável. No entanto, o Bitcoin tornou-se centralizado muito rapidamente e agora depende de um pequeno grupo de desenvolvedores de software e pools de mineração para funcionar  
_Fundo Monetário Internacional_

Como mostra a citação acima de uma postagem relativamente recente do Fundo Monetário Internacional, a indústria financeira tradicional continua a afirmar que o Bitcoin não é descentralizado, além de confundir o Bitcoin com outros criptoativos.

##### Introdução

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/46e016b084f3d0ec877ca26eb5ed77515ba0048c-161x167.svg)

A descentralização é um aspecto fundamental do Bitcoin. A capacidade de manter as regras do protocolo, como escassez e distribuição, sem uma autoridade central garante que ele possa atuar como dinheiro sem permissão para uma sociedade global.

Como Satoshi observou em sua correspondência online, serviços descentralizados como o BitTorrent estavam 'se mantendo' contra repressões governamentais, em comparação com serviços com proprietário(s) identificado(s) e servidores centralizados. Ele estava claramente preocupado com o risco potencial de governos ou outros interesses encerrarem ou de alguma forma prejudicarem o Bitcoin.

Neste contexto, estamos interessados na descentralização de:

* O desenvolvimento e a gestão do código que executa o protocolo; quem pode mudar as regras?
* A função de mineração que cria novos blocos de acordo com as regras e valida contra o duplo gasto
* Os nós que validam as transações quanto à validade e mantêm uma cópia do blockchain

##### Desenvolvedores

O Bitcoin é um protocolo de código aberto que qualquer pessoa pode examinar, baixar, copiar ou sugerir alterações. Ele está disponível em uma biblioteca do GitHub, tendo o código-fonte sido lançado originalmente em 2009 por Satoshi Nakamoto. Qualquer pessoa pode baixar o código e rodar um nó, sendo que a maioria executa o software original do Bitcoin Core, que foi atualizado ao longo do tempo.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Fonte: https://river.com/learn/what-is-bitcoin-core/_

O desenvolvimento do Bitcoin Core segue as melhores práticas do desenvolvimento de código aberto. A qualquer momento, pode haver vários desenvolvedores escrevendo ou revisando alterações no código. Eles precisam ouvir as preocupações dos operadores de nós e mineradores, bem como da base de usuários, antes de fazer qualquer alteração crítica no código, que será revisada e acordada conforme mostrado no fluxograma acima antes de ser incorporada ao código.

As regras do Bitcoin são então codificadas neste software Bitcoin Core, que roda em cada nó. Qualquer pessoa pode sugerir uma alteração nas regras – as regras são código, mas elas não são_apenas_código, elas são_acordadas_por consenso. Se forem alteradas unilateralmente, o novo código deixa de fazer parte do consenso e deixa de ser parte do Bitcoin. Mudar algo no Bitcoin e permanecer em consenso é complicado. As alterações sugeridas no código se enquadram em uma de três categorias:

* Dentro das regras existentes: Atualizações menores, como correções ortográficas, melhorias na interface ou na gestão de dados podem se enquadrar nesta categoria e são relativamente triviais de serem aprovadas.
* Adicionar uma nova regra que impõe restrições às regras – como reduzir o tamanho do bloco. Isso é chamado de 'soft fork'. Nós que optarem por não implementar a alteração e permanecerem na versão antiga ainda poderão participar da rede.
* Adicionar uma nova regra que quebra as regras atuais, por exemplo, um aumento no tamanho do bloco. Nós que não atualizarem para o novo código rejeitarão um bloco criado com tamanho maior como inválido. Isso é chamado de 'hard fork' e criará uma divisão na cadeia entre os nós que executam o código original e o novo, criando uma nova moeda. Isso já aconteceu anteriormente, mas não levou a nenhum sucesso de longo prazo para a nova moeda, pois a maioria dos nós decidiu manter o código original.

Portanto, uma única parte ou grupo de pessoas não pode alterar unilateralmente o código do Bitcoin sem obter um acordo de consenso, ou corre o risco de uma divisão da cadeia e da criação de uma nova moeda seguindo um conjunto diferente de regras.

##### Mineração

A função de mineração valida as transações assim como qualquer outro nó na rede, mas então gasta a energia necessária para criar um novo bloco que atenda às regras de consenso do código. O sucesso permite ao minerador obter recompensas na forma de taxas de transação e recompensas em Bitcoin (no momento da escrita, 3,125 moedas por bloco).

A mineração normalmente é realizada por 'pools' de mineração, onde pessoas consolidam o poder de mineração ou taxa de hash para aumentar as chances de minerar um bloco com sucesso e compartilhar as recompensas. Existe o perigo de que um ou mais desses pools de mineração possam se unir para alcançar 51% de domínio na mineração e, essencialmente, sobrepor o protocolo de validação da rede em seu favor para gastar moedas duas vezes. Isso exigiria uma quantidade massiva de recursos a um grande custo, e mineradores individuais podem facilmente mudar para outro pool de mineração a qualquer momento. Tal ataque provavelmente também colapsaria o valor do bitcoin, já que seria óbvio que a integridade da rede foi comprometida. Portanto, o atacante teria que converter rapidamente qualquer bitcoin obtido em moeda fiduciária antes que o valor se erodisse. Isso tornaria ainda mais difícil sustentar um ataque por um longo período, tornando mais lucrativo para um minerador ou operador de pool seguir as regras e tentar minerar blocos válidos.

A distribuição geográfica da função de mineração também é importante para evitar que governos, por exemplo, assumam a capacidade de mineração ou a encerrem. Por exemplo, uma proibição recente da mineração pela China demonstrou a capacidade do Bitcoin de se adaptar e sobreviver a tal intervenção governamental, adaptando-se e se recuperando rapidamente da consequente perda de poder de hash.

##### Nós

Ao contrário da mineração, que exige um investimento financeiro significativo para competir efetivamente na corrida para minerar novos blocos, ou do desenvolvimento de código, que exige conhecimento em programação, rodar um nó é algo que qualquer pessoa interessada em ajudar a manter a descentralização do Bitcoin pode fazer.

Os nós executam o software Bitcoin Core e aplicam as regras que o código inclui para garantir que os mineradores não trapaceiem, por exemplo, atribuindo a si mesmos uma recompensa de bloco maior do que o permitido. Eles também aplicam o limite de fornecimento de 21 milhões, que é fundamental para manter a escassez do Bitcoin. Para que qualquer governo ou agente mal-intencionado pare o Bitcoin, teria que destruir cada cópia do blockchain, atualmente rodando em milhares de nós distribuídos globalmente, uma tarefa quase impossível.

##### Pessoas

Outro aspecto de potencial centralização são as pessoas. Toda outra 'altcoin' tem um líder—alguém que poderia ser potencialmente coagido a defender mudanças que não sejam do interesse do Bitcoin. Satoshi Nakamoto permaneceu tempo suficiente para garantir que o Bitcoin estava no caminho do sucesso antes de desaparecer para sempre, deixando-o nas mãos de outros para aprimorar e adaptar o software.

E quanto aos detentores de grandes quantidades de Bitcoin? Investidores iniciais, que mantiveram suas moedas e não as perderam, serão extremamente ricos neste momento. É importante notar que isso pode realmente ser o caso, mas isso não lhes dá mais influência sobre o sistema do que qualquer outra pessoa, ao contrário das moedas de 'prova de participação', onde os primeiros adotantes, já ricos naquela moeda, ganham vantagens na tomada de decisões e na distribuição de futuras moedas. Isso inevitavelmente levou ou levará à centralização ao longo do tempo.

##### Conclusão

Quais são as ameaças potenciais que a descentralização pode tentar mitigar?

* Governo encerrando ou proibindo o Bitcoin
* Alterações indesejadas no código que favorecem um conjunto de interesses no Bitcoin, por exemplo, aumento da recompensa de bloco
* Coerção do protocolo por parte do governo ou agentes mal-intencionados para influenciar a direção do protocolo
* Capacidade de um pool de mineradores assumir a rede e 'gastar Bitcoin duas vezes' – um ataque de 51%

Como podemos ver, a combinação de nós, desenvolvedores de código e mineradores, bem como o uso do mecanismo de 'prova de trabalho', descentraliza o Bitcoin a um nível suficiente para que essas ameaças potenciais não sejam consideradas de grande preocupação. A comunidade precisará continuar monitorando a situação para garantir que isso continue assim.
