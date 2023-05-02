Onderzoek vertaalmodule

**Wat zijn verschillende manieren voor vertalingen te beheren binnen een applicatie?**

Francois haan

22/03/2023

# Versiebeheer

| **Versie** | **Datum** | **Auteur(s)** | **Wijzigingen** | **Status** |
| --- | --- | --- | --- | --- |
| 1.0 | 22/03/2023 | Francois Haan | 1ste versie | Klaar |
| 1.1 | 03/04/2023 | Francois Haan | Uitwerken conclusie | Klaar |
| 1.2 | 06/04/2023 | Francois Haan | Aanpassingen conclusie | Klaar |
| 1.3 | 14/04/2023 | Francois Haan | Feedback verwerken | Klaar |
| 1.4 | 17/04/2023 | Francois Haan | Spellingscontrole | Klaar |

Contents

**[Versiebeheer 2](#_Toc128580471)**

**[Wat ga ik onderzoeken? 4](#_Toc128580472)**

**[Hoe gaat ik het onderzoeken? 5](#_Toc128580473)**

**[Waarom ga ik het onderzoeken? 6](#_Toc128580474)**

**[Resultaten 7](#_Toc128580475)**

# Wat ga ik onderzoeken?

Ik ga onderzoek doen naar hoe de vertalingen momenteel gedaan worden binnen de bestaande applicatie en naar eventuele andere methodes, en dan kijken naar de verschillen en voordelen die iedere methode met zich meebrengt.

# Hoe gaat ik het onderzoeken?

Ik ga hier literatuuronderzoek gebruiken door op forums, blogs etc. Verschillende manieren om vertalingen te onderhouden bekijken.

# Waarom ga ik het onderzoeken?

Ik ga het onderzoeken omdat dit heel belangrijk is binnen dit project namelijk het belangrijkste gedeelte aangezien dit bepaald hoe ik het moet gaan aanpakken en hoe ik aanpassingen zou moeten maken aan deze teksten of juist niet afhankelijk van wat hier uitkomt.

# Resultaten

Allereerst de verschillen tussen lokalisatie en vertalingen. Vertalingen gaan alleen over de teksten en het vertalen naar andere talen, waar lokalisatie inspeelt op een product toegankelijk maken door aan te passen aan de cultuurdoormiddel van dingen zoals culturele verschillen, koop gewoontes, legale benodigdheden etc. Mijn project en onderzoek zal dus alleen maar draaien over de vertalingen.

Ik vind in het specifiek binnen voor Symfony veel over de manier die momenteel al gebruikt wordt in het systeem van Performation, namelijk met hulp van de Symfony Translatie package wat samenwerkt met Twig door middel van Yaml files die de vertalingen bijhouden aan de hand van een key met een waarde die dan anders is gebaseerd op de taal, dan binnen Twig wordt er gekeken naar de lokale waar de user zich in bevindt en dan wordt de tekst in het Nederlands, Duits of Engels weer gegeven. Hier is ook de mogelijkheid om een standaard te hebben voor zodra de user zich in geen van de bekende locaties bevindt dit komt meestal neer op Engels.

Ook is er natuurlijk de manier van alles opslaan in de database dit zou tenminste het aanpassen van alle bestanden wel makkelijker kunnen maken, maar een nadeel van deze methode is dat bij grotere applicaties er dus heel veel verschillende tables/records aangemaakt zouden moeten worden voor iedere verschillende vertaling/tekst en dit kan vooral bij grote applicaties performance problemen geven.

(2021, Andrew) Verwijst en vernoemt een manier om de vertalingen binnen Symfony te kunnen gebruiken met database Waardes waardoor het voor de vertaalmodule goed te doen zou moeten zijn om bestaande waardes te import en exporteren en dus binnen de applicatie goed te kunnen onderhouden dit moet dan wel gedaan worden doormiddel van een class. Alleen zoals eerder al genoemd zou dit getest moeten worden voor performance. Dit zou eventueel binnen de applicatie als een Docker container met de nodige database die dan de laatste vertalingen up to date houdt. En met deze methode zou het met een simpele CRUD opgelost kunnen worden.

(_How to Translate With GetText PO and POT Files_, z.d.) Ook heb ik iets gevonden over PO en MO files, maar op 1ste indruk lijken deze niet veel te bieden tegenover Yaml files behalve dat deze makkelijk door mensen zonder technische kennis aangepast zouden kunnen worden.

Hier heb je namelijk POT files die krijg je zodra je teksten extract uit de applicatie doormiddel van een tool dit kan dan doorgestuurd worden naar vertalers.

Dan krijg je van de vertalers een PO file terug waar de originele teksten en de vertalingen instaan die makkelijk te lezen zijn voor mensen waardoor het aanpassen ook nog niet ingewikkeld is. Dan wordt dit PO file omgezet naar een MO file die al gecompileerd zijn en makkelijk voor computers om te lezen.

Maar dit is net het probleem wat mijn applicatie moet oplossen dus dit is niet iets waar ik gebruik van zal gaan maken. Aangezien Yaml files ook goed leesbaar zijn en niet zoveel tussenstappen nodig hebben. Maar dit is niet belangrijk voor mij aangezien het hele doel van mij applicatie is om hoe het opgeslagen wordt niet te laten uitmaken voor de doorsnee gebruiker.

(Symfony, z.d.-e)

Een van de bundels binnen Symfony waar het vertalen van de teksten binnen de applicatie geregeld wordt. Die gebruikt maken van de git sub modules waar alle vertalingen worden opgeslagen in 3 verschillende talen en deze worden dan door de Symfony translate bundel vertaald gebaseerd op de ingestelde taal van de gebruiker.

![](RackMultipart20230502-1-iy0219_html_85e03d75b2cd2ee0.png)

Zo ziet het eruit binnen Twig de template engine waar Symfony gebruik van maakt. Ook kan hierin een standaardtaal worden meegegeven als er bijvoorbeeld geen vertaling is voor een taal zal het terug gaan naar de standaard.

![](RackMultipart20230502-1-iy0219_html_f33cb712fcf4c9f4.png)

Dit zijn de commando's waardoor je de content kan updaten en automatisch alles aanpassen

Alle vertalingen moeten wel geplaats worden in de translaties folder of in resources/translaties folder.

De naam van het vertalingen bestand is belangrijk dit moet namelijk in deze specifieke volgorde: domein, locatie en lader.

-domein staat voor het vertalingen domein

-locatie staat voor welke locatie het is bijvoorbeeld nl voor Nederland of de voor Duitsland

-lader voor hoe Symfony het bestand moet laden en neerzetten voorbeelden hiervan zijn xlf, PHP en Yaml die momenteel gebruikt wordt binnen het systeem bij Performation.

Hier zijn ook nog veel meer opties voor onder andere XML, JSON en CSV.

Ook kunnen de vertalingen opgeslagen worden met gebruik van doctrine in een database.

Symfony heeft ook de mogelijkheid gebruik te maken van vertaling providers zoals Lokalise, Crowdin en Loco hiermee kan je vertalingen versturen en ontvangen met een van deze providers dus hoeven ze zelf lokaal niet aangepast te worden maar zou dit gaan via een van deze providers.

Symfony heeft ook de optie met commando's binnen de console te controleren of er fouten zijn binnen de bestanden.

**Conclusie**

Ik zal hoogstwaarschijnlijk in overleg met mijn stagebegeleider besluiten hierover zelf leun ik namelijk richting het gebruik van een database omdat het aanpassen van gegevens hierbij veel vriendelijker is om dit door gebruikers te laten doen, maar er is ook een goeie mogelijkheid dat het met Yaml zal gaan werken en ik dus een manier moet zoeken om deze bestanden om te zetten naar andere applicaties.

**Bronnen**

Fuzul, M. (2022, 5 maart). _Nuts & bolts of internationalization and localization with Symfony_. Medium. https://blog.undabot.com/nuts-bolts-of-internationalization-and-localization-with-symfony-c06cd3ba5697

D. (2023b, maart 17). _What Is Localization, and How to Build a Strategy?_ Phrase. https://phrase.com/blog/posts/how-important-is-localization-for-your-business/

A. (2021, 9 December). _Store translation messages in database in Symfony - Andrew - Medium_. Medium. https://medium.com/@andrew72ru/store-translation-messages-in-database-in-symfony-3f12e579df74

_How to Translate with GetText PO and POT Files_. (z.d.). https://www.icanlocalize.com/site/tutorials/how-to-translate-with-gettext-po-and-pot-files/#:~:text=The%20MO%20file%20includes%20the,file%20to%20display%20the%20translations.

Symfony. (z.d.-e). _Translations (Symfony 5.4 Docs)_. Symfony. https://symfony.com/doc/5.4/translation.html
