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

![image](https://user-images.githubusercontent.com/71487939/236818133-8f9bc98f-4a14-443e-a391-925a4daf634e.png)

_Level 2_

![image](https://user-images.githubusercontent.com/71487939/236818152-bd292c8c-d05e-4745-aad3-6019a0d15d46.png)

**Data-flow-diagram**

![image](https://user-images.githubusercontent.com/71487939/236818180-72fa1374-64b3-471e-bcd0-7bd8b2bb45df.png)

![image](https://user-images.githubusercontent.com/71487939/236818215-e8d4ec56-e57a-4f39-97d5-8c5bf90a4665.png)

![image](https://user-images.githubusercontent.com/71487939/236818239-d637ba38-2db9-42e3-8d90-ff27911a9b51.png)

**Use-case-diagram**

![image](https://user-images.githubusercontent.com/71487939/236818336-0754f759-997f-458e-8698-807f6236086d.png)

**De geupdaten use-case-diagram met enkele van de eventuele mogelijkheden**

![image](https://user-images.githubusercontent.com/71487939/236818363-03713f47-dd8c-4c6b-8c78-0d85d51eaf7a.png)

**Use-cases**

| **Use case** |
| --- |
| **Titel** | **Vertaling aanpassen** |
| **Beschrijving** | **Aanpassen van de vertalingen** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **Gebruiker moet binnen het systeem van Performation zitten.** |
| **Basis flow** |
| **1. Gebruiker navigeert naar de aan te passen vertaling**** 2. De gebruiker vult de aangepaste vertaling in. ****3. De gebruiker geeft confirmatie voor de gemaakte aanpassing** |
| **Succes scenario** |
|**Vertaling is aangepast** |

![image](https://user-images.githubusercontent.com/71487939/236818430-b37c198b-4701-4f80-ae5a-146220466fa6.png)

| **Use case** |
| --- |
| **Titel** | **Vertaling zoeken** |
| **Beschrijving** | **Het zoeken naar een bestaande vertaling** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen**** 2. De gebruiker vult de zoekopdracht in ****3. De gebruiker ziet een overzicht van de resultaten** |
| **Succes scenario** | 
|**Het systeem geeft alles gebaseerd op de zoekopdracht weer** |

![image](https://user-images.githubusercontent.com/71487939/236818472-0e5804e2-34c8-4a2e-978c-215dbf81c2de.png)

| **Use case** |
| --- |
| **Titel** | **Vertaling toevoegen** |
| **Beschrijving** | **Het toevoegen van een vertaling** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker voert de benodigde gegevens voor een nieuwe vertaling in (key, value) ****3. De gebruiker geeft confirmatie voor de gemaakte aanpassing.**** 4. de gebruiker ziet de nieuwe vertaling toegevoegd.** |
| **Succes scenario** | 
|**Het systeem voegt de nieuwe vertaling toe.** |

![image](https://user-images.githubusercontent.com/71487939/236818585-35e75a18-574e-45f5-856e-7585c9202588.png)

| **Use case** |
| --- |
| **Titel** | **Filteren op een domein** |
| **Beschrijving** | **Het specifieke filteren op een domein waardoor alleen vertalingen binnen dat domein worden weergegeven** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker ziet een lijst van alle domeinen.**  **2. De gebruiker selecteert een domein.**** 3. De gebruiker ziet een lijst van alle vertalingen binnen dat domein**
| **Succes scenario** | 
|**Het systeem filtert op het specifieke domein en laat alleen maar vertalingen uit dit domein zien.** |

![image](https://user-images.githubusercontent.com/71487939/236818624-121abdbf-22d1-49de-aa6a-6078d144ca38.png)

| **Use case** |
| --- |
| **Titel** | **Vertalingen doorzetten** |
| **Beschrijving** | **De vertalingen opslaan en doorzetten naar de git submodule, deze aanpassingen moeten dan wel gecontroleerd worden door iemand.** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker heeft aanpassingen gemaakt ****3. De gebruiker heeft de aanpassingen opgeslagen**** 4. De gebruiker zet de vertalingen door** |
| **Succes scenario** | 
|**Het systeem zet de vertalingen door voor controle en hierna compleet doorgezet naar de submodule** |

![image](https://user-images.githubusercontent.com/71487939/236818665-d0d202ec-8288-45df-a739-64482cbc08b0.png)

| **Use case** |
| --- |
| **Titel** | **Opslaan vertaling** |
| **Beschrijving** | **Het opslaan van de gemaakte aanpassingen/toevoeging** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker voegt iets toe of maakt een aanpassing ****3. De gebruiker slaat de gemaakte aanpassing of toevoeging op**** 4. De gebruiker ziet een confirmatie van de gemaakte aanpassingen/toevoegingen**
| **Succes scenario** | 
|**Het systeem slaat de aanpassingen/toevoegingen op in de database** |

![image](https://user-images.githubusercontent.com/71487939/236818798-44f2da10-c0c1-41e4-b231-1eee2fcb5b7d.png)

| **Use case** |
| --- |
| **Titel** | **Aanpassen branch** |
| **Beschrijving** | **Het aanpassen van de momentele branch van de git submodules** |
| **Actors** | **De gebruiker van de applicatie( een medewerker binnen Performation)** |
| **Precondities** | **De gebruiker moet binnen het systeem van Performation zitten** |
| **Basis flow** |
| **1. De gebruiker navigeert naar de vertalingen pagina**** 2. De gebruiker krijgt een scherm van de verschillende branches die er momenteel zijn ****3.De gebruiker kiest een van de branches**** 4. De gebruiker krijgt alle domeinen/vertalingen binnen deze branch te zien.**
| **Succes scenario** | 
|**Het systeem slaat de aanpassingen/toevoegingen op in de database** |

![image](https://user-images.githubusercontent.com/71487939/236818878-68a8aad0-3479-4108-87cb-001284af60c0.png)

**ERD diagram**

I ![image](https://user-images.githubusercontent.com/71487939/236818936-974d5fa0-52b1-44e6-9ba2-be5bbae41d28.png) k ga geen ERD diagram maken aangezien dit heel veel tijd zou kosten omdat er veel verschillende tabellen moeten komen dit is maar een deel ervan maar ieder van deze Aparte bestanden krijgt een tabel in de database, alleen zal het niet 3 aparte tabellen hebben voor de ondersteunde talen deze zullen dan samen in een tabel zitten.

![image](https://user-images.githubusercontent.com/71487939/236818979-e39a7697-a079-4872-9ad8-63ee85ac82f6.png)

Dit is een zo'n bestand hier is een key die uniek is binnen dit bestand en de tekst die daarbij hoort deze zullen dan beide ook in de database staan.

Deze zullen dan voor overzicht waarschijnlijk opgedeeld worden in departementen om alles overzichtelijker te maken, de departementen hebben dan te maken waar ze binnen de applicatie gebruikt worden enkele voorbeelden hiervan zijn beheer, orso en bijvoorbeeld verpleegkundig personeel

**Na een gesprek met mijn stagebegeleider is hiervoor een alternatief gevonden en deze heb ik verwerkt in een erd diagram**

![image](https://user-images.githubusercontent.com/71487939/236819061-0d40ef85-0049-4cb3-9354-0406b4681441.png)

Enkele fouten gecorrigeerd in deze

![image](https://user-images.githubusercontent.com/71487939/236819098-d74302b1-e0b3-419a-889e-d8707ec3e7d4.png)

**Klasse diagram**

![image](https://user-images.githubusercontent.com/71487939/236819218-c0198da5-882f-4b2e-a09e-cce8759d93ea.png)

**Na feedback heb ik mijn klasse diagram aangepast**

![image](https://user-images.githubusercontent.com/71487939/236819247-d98fd509-b949-402e-bacf-268764cc5055.png)


