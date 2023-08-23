# 1	Kontrola, zda je došlý soubor typu xml

Kontroluje se, zda je došlý soubor typu xml. Zároveň se kontroluje, zda přípona souboru odpovídá formátu.

| výsledek  | stav | kód chyby | vypsané hlášení |
| ------------- | ------------- |------------- | ------------- | 
| Došlý soubor je typu xml.  | chyba  | 300010 | Struktura SIP neodpovídá NSeSSS v. 3, příloha 3, kapitola 11
| Došlý soubor není typu xml.  |  pořádku  | |  |



výsledek	stav	kód stavu	vypsané hlášení	následující krok
Hodnota atributu <forma_uchovani> je Originál a příslušný soubor odpovídá Formátovým pravidlům	v pořádku			29
Hodnota atributu <forma_uchovani> je Originál ve výstupním datovém formátu a příslušný soubor odpovídá Formátovým pravidlům (tzn. je ve výstupním datovém formátu).	v pořádku			29
Hodnota atributu <forma_uchovani> je Originál ve výstupním datovém formátu a příslušný soubor neodpovídá Formátovým pravidlům (tzn. není ve výstupním datovém formátu nebo nutno rozbalit).	chyba	380110	Komponenta …., poradi = ... s formou uchování "originál ve výstupním datovém formátu" není ve výstupním datovém formátu: identifikovaný formát/ očekávaný formát
popř.
Komponentu ..., poradi = ... nutno rozbalit.	30
Hodnota atributu <forma_uchovani> je Originál, příslušný soubor neodpovídá Formátovým pravidlům a k dané komponentě existuje vyšší verze s <formou_uchování> Originál nebo Originál ve výstupním datovém formátu, která odpovídá Formátovým pravidlům	v pořádku			29
Hodnota atributu <forma_uchovani> je Originál, příslušný soubor neodpovídá Formátovým pravidlům a k dané komponentě neexistuje vyšší verze s <formou_uchování> Originál nebo Originál ve výstupním datovém formátu.	chyba	380120	Komponenta ..., poradi = ... s formou uchování "originál" nesplňuje Formátová pravidla NA. Komponenta splňující Formátová pravidla NA se stejným „poradi" a formou uchování „originál“ nebo „originál ve výstupním datovém formátu" v dokumentu není.
identifikovaný formát/očekávaný formát
popř.

Komponentu …., poradi = ... nutno rozbalit. 	30
Pro koncept není originál, není “Originál ve výstupním datovém formátu”	chyba	380130	Pro komponentu ..., poradi = ... v dokumentu není komponenta se stejným „poradi" a formou uchování  „originál" nebo „originál ve výstupním datovém formátu“.
identifikovaný formát/očekávaný formát	30
Hodnota atributu <forma_uchovani> je Originál, jedná se o nejvyšší verzi dané komponenty a podle Formátových pravidel je vyžadováno individuální posouzení archivářem.	chyba	380140	U komponenty ... je vyžadováno individuální posouzení archivářem.
identifikovaný formát/ očekávaný formát	30
Formát nebyl identifikován	chyba	380150	U komponenty ... se nepodařilo identifikovat formát, je vyžadováno individuální posouzení archivářem.	30


# POKUSNA1
Popis změn
Něco napíšeme

## 29	Validace pro potřeby skartačního řízení
Samostatná validace pro potřeby skartačního řízení vypuštěna. Odchylky od celé validace byly zapracovány do existujících testů.


## 30	SIP je validní
31	Konec
