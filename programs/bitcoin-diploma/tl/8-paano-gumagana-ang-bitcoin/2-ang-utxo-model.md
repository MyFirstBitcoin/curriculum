# 8.2 Ang UTXO Model

##### Ano ang mga UTXO?

Huwag kang matakot sa kakaibang pangalan. Maaari mong isipin ang UTXO bilang mga piraso ng bitcoin, katulad ng mga papel at barya sa iyong pitaka. Halimbawa, kung magbabayad ka ng ₱300 gamit ang ₱500 na bill para sa isang bagay na nagkakahalaga ng ₱300, makakatanggap ka ng ₱200 na sukli. Ganoon din ang paraan ng paggana ng Bitcoin.

Ang lahat ng bitcoin na pagmamay-ari mo ay binubuo ng iba't ibang UTXO. Kapag nagpapadala ka ng bitcoin, ginagamit ng iyong wallet ang isa o higit pang mga piraso na ito para gawin ang bayad.

Kung ang piraso na ginamit mo ay mas malaki kaysa sa halagang ipinadala mo, ang natitirang halaga ay babalik sa iyo bilang sukli sa anyo ng bagong UTXO. Kasabay nito, makakatanggap ang tumanggap ng bagong UTXO na kumakatawan sa bitcoin na ipinadala mo.

Ang balanse ng iyong wallet ay simpleng kabuuang halaga ng lahat ng UTXO na kontrolado mo.


> **Callout – Pribasiya**
>
> Hindi mo dapat ipaalam sa iba ang tungkol sa iyong mga UTXO dahil kapag nalaman nila ito, maaari nilang subaybayan ang iyong mga transaksyon at sa huli ay malalaman nila kung magkano ang pera mo.


###### Halimbawa

1. Gustong magpadala ni Ana ng 5 BTC kay Ben.
1. Gumamit ang kanyang wallet ng dalawa sa kanyang mga UTXO na ang kabuuang halaga ay 6 BTC.
1. Ang transaksyon ay nagpapadala ng **5 BTC kay Ben**, na lumilikha ng bagong UTXO sa wallet ni Ben.
1. Ang natitirang **0.99 BTC ay bumabalik kay Ana bilang sukli**, matapos mabayaran ang **0.01 BTC na bayad sa transaksyon**.
1. Kapag nakumpirma na ang transaksyon, ito ay idinadagdag sa ledger ng Bitcoin at ang mga UTXO na ginamit ni Ana ay itinatala bilang nagastos na, kaya hindi na ito maaaring gamitin muli.

###### Mga Sanggunian


[▶ Panoorin ang “How Bitcoin Works under the Hood”](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
