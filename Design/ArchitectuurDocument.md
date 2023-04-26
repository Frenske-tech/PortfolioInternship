**ArchitectuurDocument**

Contents

**[ArchitectuurDocument 1](#_Toc133398366)**

[C4-diagram 1](#_Toc133398367)

[Level 1 1](#_Toc133398368)

[Level 2 2](#_Toc133398369)

[Data-flow-diagram 2](#_Toc133398370)

[Use-case-diagram 4](#_Toc133398371)

[Use-cases 4](#_Toc133398372)

[ERD diagram 7](#_Toc133398373)

[Klasse diagram 8](#_Toc133398374)

**C4-diagram**

_Level 1_

![](RackMultipart20230426-1-tx4kzw_html_775cb46e228138a5.png)

_Level 2_

![](RackMultipart20230426-1-tx4kzw_html_3d4011dd55f2cbe6.png)

**Data-flow-diagram**

![](RackMultipart20230426-1-tx4kzw_html_b971216ce39eb281.png)

![](RackMultipart20230426-1-tx4kzw_html_9ba4d3d6933339b1.png)

![](RackMultipart20230426-1-tx4kzw_html_77cb1c3538f92736.png)

**Use-case-diagram**

![](RackMultipart20230426-1-tx4kzw_html_21a26db175c3e524.png)

**Use-cases**

| **Use case** |
| --- |
| **Titel** | **Vertaling aanpassen** |
| **Beschrijving** | **Aanpassen van de vertalingen** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **Gebruiker moet binnen het systeem van Performation zitten.** |
| **Basis flow** |
| **1. Gebruiker navigeert naar de aan te passen vertaling**** 2. De gebruiker vult de aangepaste vertaling in. ****3. Het systeem slaat de aangepaste vertaling op** |
| **Succes scenario** | **Vertaling is aangepast** |

| **Use case** |
| --- |
| **Titel** | **Vertaling zoeken** |
| **Beschrijving** | **Het zoeken naar een bestaande vertaling** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen**** 2. De gebruiker vult de zoekopdracht in ****3. het systeem geeft de resultaten weer** |
| **Succes scenario** | **Het systeem geeft alles gebaseerd op de zoekopdracht weer** |

| **Use case** |
| --- |
| **Titel** | **Vertaling toevoegen** |
| **Beschrijving** | **Het toevoegen van een vertaling** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker voert de benodigde gegevens voor een nieuwe vertaling in (key, value) ****3. Het systeem slaat de nieuwe vertaling op.**** 4. Het systeem laat de nieuwe vertaling zien.**
 |
| **Succes scenario** | **Het systeem voegt de nieuwe vertaling toe.** |

| **Use case** |
| --- |
| **Titel** | **Filteren op een domein** |
| **Beschrijving** | **Het specifieke filteren op een domein waardoor alleen vertalingen binnen dat domein worden weergegeven** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1.**
 |
| **Succes scenario** | **Het systeem filtert op het specifieke domein en laat alleen maar vertalingen uit dit domein zien.** |

| **Use case** |
| --- |
| **Titel** | **Vertalingen doorzetten** |
| **Beschrijving** | **De vertalingen opslaan en doorzetten naar de git submodule, deze aanpassingen moeten dan wel gecontroleerd worden door iemand.** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker heeft aanpassingen gemaakt ****3. De gebruiker heeft de aanpassingen opgeslagen**** 4. De gebruiker zet de vertalingen door ****5. het systeem communiceert met de submodule en maakt de gemaakte aanpassingen en zet deze door.**
 |
| **Succes scenario** | **Het systeem zet de vertalingen door voor controle en hierna compleet doorgezet naar de submodule** |

| **Use case** |
| --- |
| **Titel** | **Opslaan vertaling** |
| **Beschrijving** | **Het opslaan van de gemaakte aanpassingen/toevoeging** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker voegt iets toe of maakt een aanpassing ****3. De gebruiker slaat de gemaakte aanpassing of toevoeging op**** 4. Het systeem slaat de aanpassing/toevoeging op in de database.**

 |
| **Succes scenario** | **Het systeem slaat de aanpassingen/toevoegingen op in de database** |

**ERD diagram**

I ![](RackMultipart20230426-1-tx4kzw_html_2f209eb18eb315f1.png) k ga geen ERD diagram maken aangezien dit heel veel tijd zou kosten omdat er veel verschillende tabellen moeten komen dit is maar een deel ervan maar ieder van deze Aparte bestanden krijgt een tabel in de database, alleen zal het niet 3 aparte tabellen hebben voor de ondersteunde talen deze zullen dan samen in een tabel zitten.

![](RackMultipart20230426-1-tx4kzw_html_9c7bbe011b5640bc.png)

Dit is een zo'n bestand hier is een key die uniek is binnen dit bestand en de tekst die daarbij hoort deze zullen dan beide ook in de database staan.

Deze zullen dan voor overzicht waarschijnlijk opgedeeld worden in departementen om alles overzichtelijker te maken, de departementen hebben dan te maken waar ze binnen de applicatie gebruikt worden enkele voorbeelden hiervan zijn beheer, orso en bijvoorbeeld verpleegkundig personeel

**Klasse diagram**

![](RackMultipart20230426-1-tx4kzw_html_888402a5e21ce4c9.png)
