# 3.1 O desenvolvimento do TCP/IP

A maioria de nós está familiarizada com os protocolos TCP/IP em uso hoje como a base da internet. Suas origens remontam ao final dos anos 70, quando cientistas exploravam designs alternativos para a Arpanet – uma rede ainda mais antiga concebida pelo Departamento de Defesa dos EUA para possibilitar o compartilhamento de recursos entre computadores remotos. O TCP/IP tornou-se o padrão de protocolo para a Arpanet em 1983, o que levou a se tornar o modelo dominante de redes até o final dos anos 1990 e a base para a internet na qual o Bitcoin opera atualmente.


| Modelo OSI | TCP/IP |
| --- | --- |
| Aplicação | Aplicação |
| Apresentação | Aplicação |
| Sessão | Aplicação |
| Transporte | Transporte |
| Rede | Rede |
| Enlace de Dados | Enlace de Dados |
| Físico | Físico |


Ao mesmo tempo em que o modelo TCP/IP estava sendo desenvolvido, uma estrutura semelhante, porém mais abrangente, estava sendo criada pela Organização Internacional de Padronização (ISO) e pela indústria de Telecomunicações (CCITT). O processo para desenvolver novos protocolos ou sugerir mudanças era lento e pouco prático em comparação com a abordagem mais descentralizada usada no desenvolvimento do TCP/IP, levando ao domínio deste modelo atualmente.

##### Solicitação de Mudança

Quaisquer desenvolvimentos sugeridos para protocolos existentes ou ideias para novos podem ser propostos no modelo TCP/IP através de uma **Solicitação de Mudança** processo. Estes passam por um processo de aprovação, gerenciado pela Internet Engineering Task Force (IETF), e tornam-se de código aberto uma vez aprovados, permitindo que qualquer pessoa os implemente e adote. Alguns exemplos notáveis:

* 1969 RFC 1 Documentou como os pacotes seriam enviados na Arpanet
* 1981 RFC791 definiu o protocolo de Internet V4 – ainda amplamente adotado hoje
* 1982 RFC 821 Protocolo simples de transferência de e-mail
* 1987 Sistema de Nomes de Domínio – como nomes de domínio são resolvidos para endereços IP
* 1999 RFC 2616 Protocolo de Transferência de Hipertexto – essencial para navegação na web


> **Callout**
>
> A **Proposta de Melhoria do Bitcoin** (BIP) segue uma abordagem semelhante à RFC, mas focando exclusivamente em melhorias para o próprio Bitcoin, em vez do desenvolvimento de novos protocolos ou alternativas. O Bitcoin também se inspira nesse modelo em camadas, e você verá protocolos adicionais descritos como camada dois ou três.


Da mesma forma que as camadas base do modelo TCP/IP mudaram relativamente pouco nas últimas décadas, com a inovação ocorrendo nas camadas superiores, espera-se que a camada base do Bitcoin mude muito lentamente neste momento, com soluções de escalabilidade como Lightning e Liquid ocorrendo acima.

Um bom exemplo de como protocolos de camada base se tornam difíceis de mudar ao longo do tempo é o IPv6. A esperada exaustão do espaço de endereços no IPv4 criou uma demanda por um novo protocolo. O primeiro rascunho do padrão foi criado em 1998, mas só foi ratificado como padrão da internet em 2017. Embora tenha resolvido muitos problemas do IPv4 e seja muito mais preparado para o futuro, ainda assim teve uma adoção muito lenta na indústria atualmente. Durante esse tempo, muitos novos protocolos foram definidos nas camadas superiores para possibilitar multimídia, e-mail etc.

##### Os blocos de construção usados pelo Bitcoin

Essa separação dos problemas de interconectividade permite que os protocolos sejam desenvolvidos independentemente das camadas acima e abaixo. Em vez de ter que reinventar soluções para cada camada, a rede Bitcoin pode contar com as capacidades subjacentes da rede fornecidas nas camadas física e de enlace de dados.


| Camada | TCP/IP Original |
| --- | --- |
| Aplicação | Usa o Sistema de Nomes de Domínio (DNS) para identificar nós vizinhos. A porta 8333 sinaliza o protocolo Bitcoin. |
| Transporte | UDP para comunicações FIBRE entre mineradores para baixa latência. TCP para comunicações P2P entre nós. |
| Transporte | Roteamento TOR: Permite anonimato e privacidade. Protocolo de Broadcast: Roteia o tráfego pela rede. |
| Enlace | Opera sobre qualquer meio (por exemplo, Ethernet, Wi-Fi, etc.) |
| Físico | Transmissão física via wireless, Ethernet ou outras interfaces de hardware. |


##### Bitcoin é um protocolo neutro para transferir valor assim como HTTPS é um protocolo para transferir informação

* **HTTPS**: Sites Seguros
* **SMTP**: Enviar e-mails
* **FTP**: Transferir arquivos
* **DNS**: Gerenciar nomes de domínio
* **BTC**: Armazenar e transferir valor

O Bitcoin permite que o valor seja transportado de forma confiável e sem a necessidade de um terceiro entre pessoas ou dispositivos pela Internet. Espera-se que isso libere um valor imenso.
