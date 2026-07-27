# 8.2 Model UTXO

##### Co jsou to UTXO?

Nenechte se odradit zvláštním názvem. UTXO si můžete představit jako kousky bitcoinu, podobně jako bankovky a mince ve vaší peněžence. Například pokud zaplatíte za zboží v hodnotě 6 € bankovkou v hodnotě 10 €, dostanete zpět 4 € jako drobné. Bitcoin funguje podobně.

Všechny bitcoiny, které vlastníte, jsou složené z různých UTXO. Když posíláte bitcoin, vaše peněženka použije jeden nebo více těchto kousků k provedení platby.

Pokud je kousek, který utratíte, větší než částka, kterou posíláte, zbytek hodnoty se vám vrátí jako drobné ve formě nového UTXO. Zároveň příjemce obdrží nové UTXO, které představuje bitcoin, který jste poslali.

Zůstatek vaší peněženky je jednoduše součtem hodnot všech UTXO, které ovládáte.


> **Callout – Soukromí**
>
> Neměli byste ostatním sdělovat své UTXO, protože pokud je někdo zná, může sledovat vaše transakce a nakonec zjistí, kolik peněz vlastníte.


###### Příklad

1. Alena chce poslat Petrovi 5 BTC.
1. Její peněženka použije dvě její UTXO, která dohromady mají hodnotu 6 BTC.
1. Transakce odešle **5 BTC Petrovi**, čímž vytvoří nové UTXO v Petrově peněžence.
1. Zbývajících **0,99 BTC se vrátí Aleně jako drobné**, po zaplacení **0,01 BTC transakčního poplatku**.
1. Jakmile je transakce potvrzena, je přidána do účetní knihy Bitcoinu a UTXO použité Alenou jsou označeny jako utracené, takže je již nelze znovu použít.

###### Zdroje


[▶ Podívejte se na „How Bitcoin Works under the Hood“](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
