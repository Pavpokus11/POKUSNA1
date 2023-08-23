# 1	Kontrola, zda je došlý soubor typu xml 

Kontroluje se, zda je došlý soubor typu xml. Zároveň se kontroluje, zda přípona souboru odpovídá formátu.

| výsledek  | stav | kód chyby | vypsané hlášení |
| ------------- | ------------- |------------- | ------------- | 
| Došlý soubor je typu xml.  | chyba  | 300010 | Struktura SIP neodpovídá NSeSSS v. 3, příloha 3, kapitola 11
| Došlý soubor není typu xml.  |  pořádku  | |  |
| Došlý soubor je typu xml, ale nemá správnou příponu. | chyba  | 300010 | Struktura SIP neodpovídá NSeSSS v. 3, příloha 3, kapitola 11

# 2	Kontrola, zda je došlý soubor typu zip

Kontroluje se, zda je došlý soubor typu zip. Zároveň se kontroluje, zda přípona souboru odpovídá formátu.

| výsledek  | stav | kód chyby | vypsané hlášení |
| ------------- | ------------- | ------------- | ------------- | 
| Došlý soubor je typu zip.  | pořádku  | |  |
| Došlý soubor není typu zip.  |  chyba  | 100000| Soubor není ve správném formátu. |
| Došlý soubor je typu zip, ale nemá správnou příponu. | chyba  | 100001 | Přípona souboru neodpovídá formátu.


| výsledek |	stav |	kód stavu |	vypsané hlášení	| následující krok
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| Hodnota atributu <forma_uchovani> je Originál a příslušný soubor odpovídá Formátovým pravidlům |	v pořádku | | |	29 |
|Hodnota atributu <forma_uchovani> je Originál ve výstupním datovém formátu a příslušný soubor odpovídá Formátovým pravidlům (tzn. je ve výstupním datovém formátu). |	v pořádku |	| |	29 |


# POKUSNA1
Popis změn
Něco napíšeme

## 29	Validace pro potřeby skartačního řízení
Samostatná validace pro potřeby skartačního řízení vypuštěna. Odchylky od celé validace byly zapracovány do existujících testů.


## 30	SIP je validní
31	Konec
