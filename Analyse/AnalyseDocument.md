**ArchitectuurDocument**

Contents

**[ArchitectuurDocument 1](#_Toc134521436)**

[C4-diagram 1](#_Toc134521437)

[Level 1 1](#_Toc134521438)

[Level 2 2](#_Toc134521439)

[Data-flow-diagram 2](#_Toc134521440)

[Use-case-diagram 4](#_Toc134521441)

[Use-cases 5](#_Toc134521442)

[ERD diagram 10](#_Toc134521443)

[Klasse diagram 12](#_Toc134521444)

[Git Flow diagram 13](#_Toc134521445)

**C4-diagram**

_Level 1_

![](RackMultipart20230529-1-ybkd0f_html_775cb46e228138a5.png)

_Level 2_

![](RackMultipart20230529-1-ybkd0f_html_3d4011dd55f2cbe6.png)

**Data-flow-diagram**

![](RackMultipart20230529-1-ybkd0f_html_b971216ce39eb281.png)

![](RackMultipart20230529-1-ybkd0f_html_9ba4d3d6933339b1.png)

![](RackMultipart20230529-1-ybkd0f_html_77cb1c3538f92736.png)

**Use-case-diagram**

![](RackMultipart20230529-1-ybkd0f_html_21a26db175c3e524.png)

**De geupdaten use-case-diagram met enkele van de eventuele mogelijkheden**

![](RackMultipart20230529-1-ybkd0f_html_8123d9faec6f03e6.png)

**Use-cases**

| **Use case** |
| --- |
| **Titel** | **Vertaling aanpassen** |
| **Beschrijving** | **Aanpassen van de vertalingen** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **Gebruiker moet binnen het systeem van Performation zitten.** |
| **Basis flow** |
| **1. Gebruiker navigeert naar de aan te passen vertaling**** 2. De gebruiker vult de aangepaste vertaling in. ****3. De gebruiker geeft confirmatie voor de gemaakte aanpassing** |
| **Succes scenario** | **Vertaling is aangepast** |

![](RackMultipart20230529-1-ybkd0f_html_5816103d2ae4cb14.png)

| **Use case** |
| --- |
| **Titel** | **Vertaling zoeken** |
| **Beschrijving** | **Het zoeken naar een bestaande vertaling** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen**** 2. De gebruiker vult de zoekopdracht in ****3. De gebruiker ziet een overzicht van de resultaten** |
| **Succes scenario** | **Het systeem geeft alles gebaseerd op de zoekopdracht weer** |

![](RackMultipart20230529-1-ybkd0f_html_d42db3dccfbafd4a.png)

| **Use case** |
| --- |
| **Titel** | **Vertaling toevoegen** |
| **Beschrijving** | **Het toevoegen van een vertaling** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker voert de benodigde gegevens voor een nieuwe vertaling in (key, value) ****3. De gebruiker geeft confirmatie voor de gemaakte aanpassing.**** 4. de gebruiker ziet de nieuwe vertaling toegevoegd.** |
| **Succes scenario** | **Het systeem voegt de nieuwe vertaling toe.** |

![](RackMultipart20230529-1-ybkd0f_html_f21f6d65bb9617f.png)

| **Use case** |
| --- |
| **Titel** | **Filteren op een domein** |
| **Beschrijving** | **Het specifieke filteren op een domein waardoor alleen vertalingen binnen dat domein worden weergegeven** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker ziet een lijst van alle domeinen.**  **2. De gebruiker selecteert een domein.**** 3. De gebruiker ziet een lijst van alle vertalingen binnen dat domein**
 |
| **Succes scenario** | **Het systeem filtert op het specifieke domein en laat alleen maar vertalingen uit dit domein zien.** |

![](RackMultipart20230529-1-ybkd0f_html_20c5d7f8a6898ea1.png)

| **Use case** |
| --- |
| **Titel** | **Vertalingen doorzetten** |
| **Beschrijving** | **De vertalingen opslaan en doorzetten naar de git submodule, deze aanpassingen moeten dan wel gecontroleerd worden door iemand.** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker heeft aanpassingen gemaakt ****3. De gebruiker heeft de aanpassingen opgeslagen**** 4. De gebruiker zet de vertalingen door** |
| **Succes scenario** | **Het systeem zet de vertalingen door voor controle en hierna compleet doorgezet naar de submodule** |

![](RackMultipart20230529-1-ybkd0f_html_153fdf59ebe3f264.png)

| **Use case** |
| --- |
| **Titel** | **Opslaan vertaling** |
| **Beschrijving** | **Het opslaan van de gemaakte aanpassingen/toevoeging** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker voegt iets toe of maakt een aanpassing ****3. De gebruiker slaat de gemaakte aanpassing of toevoeging op**** 4. De gebruiker ziet een confirmatie van de gemaakte aanpassingen/toevoegingen**

 |
| **Succes scenario** | **Het systeem slaat de aanpassingen/toevoegingen op in de database** |

![](RackMultipart20230529-1-ybkd0f_html_e9d1d4a393454b50.png)

| **Use case** |
| --- |
| **Titel** | **Aanpassen branch** |
| **Beschrijving** | **Het aanpassen van de momentele branch van de git submodules** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker krijgt een scherm van de verschillende branches die er momenteel zijn ****3.De gebruiker kiest een van de branches**** 4. De gebruiker krijgt alle domeinen/vertalingen binnen deze branch te zien.**

 |
| **Succes scenario** | **Het systeem slaat de aanpassingen/toevoegingen op in de database** |

![](RackMultipart20230529-1-ybkd0f_html_7605a8f87ad01d4c.png)

**ERD diagram**

I ![](RackMultipart20230529-1-ybkd0f_html_2f209eb18eb315f1.png) k ga geen ERD diagram maken aangezien dit heel veel tijd zou kosten omdat er veel verschillende tabellen moeten komen dit is maar een deel ervan maar ieder van deze Aparte bestanden krijgt een tabel in de database, alleen zal het niet 3 aparte tabellen hebben voor de ondersteunde talen deze zullen dan samen in een tabel zitten.

![](RackMultipart20230529-1-ybkd0f_html_9c7bbe011b5640bc.png)

Dit is een zo'n bestand hier is een key die uniek is binnen dit bestand en de tekst die daarbij hoort deze zullen dan beide ook in de database staan.

Deze zullen dan voor overzicht waarschijnlijk opgedeeld worden in departementen om alles overzichtelijker te maken, de departementen hebben dan te maken waar ze binnen de applicatie gebruikt worden enkele voorbeelden hiervan zijn beheer, orso en bijvoorbeeld verpleegkundig personeel

**Na een gesprek met mijn stagebegeleider is hiervoor een alternatief gevonden en deze heb ik verwerkt in een erd diagram**

![](RackMultipart20230529-1-ybkd0f_html_90c2a455c2c2017d.png)

Enkele fouten gecorrigeerd in deze

![](RackMultipart20230529-1-ybkd0f_html_633ca793a135f859.png)

Hier heb ik nog verdere feedback op gekregen en hier is het resultaat van deze feedback:

![](RackMultipart20230529-1-ybkd0f_html_aac6b3bb6737fb4f.png)

**Klasse diagram**

![](RackMultipart20230529-1-ybkd0f_html_888402a5e21ce4c9.png)

**Na feedback heb ik mijn klasse diagram aangepast**

![](RackMultipart20230529-1-ybkd0f_html_18991301a7a96adf.png)

Na de aanpassingen van mijn erd heb ik die ook doorgevoerd binnen het klasse diagram

![](RackMultipart20230529-1-ybkd0f_html_d8fb8050210744c1.png)

**Git Flow diagram**

![](RackMultipart20230529-1-ybkd0f_html_72e44ae10a76e8f8.png)

Hier heb ik feedback op gekregen en besloten dat er een nieuwe branch moet worden aangemaakt zodra de vertalingen doorgezet worden. En nu ziet het er dus iets anders uit namelijk:

![](RackMultipart20230529-1-ybkd0f_html_be088df255043959.png)
