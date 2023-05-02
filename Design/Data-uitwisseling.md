Onderzoek vertaalmodule

**Hoe gaat de data uitwisseling tussen de Symfony applicatie en de vertaal module werken?**

Francois haan

28/03/2023

# Versiebeheer

| **Versie** | **Datum** | **Auteur(s)** | **Wijzigingen** | **Status** |
| --- | --- | --- | --- | --- |
| 0.1 | 28/03/2023 | Francois Haan | 1ste versie opzet document | Klaar |
| 1.0 | 29/03/2023 | Francois Haan | 1ste versie | Klaar |
| 1.1 | 31/03/2023 | Francois Haan | Verder werken aan onderzoek | Klaar |
| 1.2 | 03/04/2023 | Francois Haan | Verder werken aan onderzoek | Klaar |
| 1.3 | 05/04/2023 | Francois Haan | Verder werken aan onderzoek | Klaar |
| 1.4 | 06/04/2023 | Francois Haan | Conclusie | Klaar |
| 1.5 | 14/04/2023 | Francois Haan | Feedback verwerken | Klaar |
| 1.6 | 17/04/2023 | Francois Haan | Spelfouten en zinsopbouw verbeteren | Klaar |

Contents

**[Versiebeheer 2](#_Toc128580471)**

**[Wat ga ik onderzoeken? 4](#_Toc128580472)**

**[Hoe gaat ik het onderzoeken? 5](#_Toc128580473)**

**[Waarom ga ik het onderzoeken? 6](#_Toc128580474)**

**[Resultaten 7](#_Toc128580475)**

# Wat ga ik onderzoeken?

In dit onderzoek ga ik onderzoeken hoe ik de nodige teksten/data kunnen overzetten van de vertaalmodule applicatie naar de nodige applicaties binnen het systeem van Performation. En hoe dit in de praktijk zou werken ook enigszins rekening houden met de grootte en hoeveelheid teksten die omgezet moeten worden. Ook zal ik hierbij rekening houden dat het momenteel allemaal wordt opgeslagen in Yaml bestanden en of er een mogelijkheid is om teksten over te zetten naar Yaml of Yaml bestanden binnen mijn applicatie aan te passen.

# Hoe gaat ik het onderzoeken?

Ik ga dit uitzoeken door het gebruik van literatuuronderzoek, ik ga online naar bestaande oplossingen zoeken en uitzoeken hoe ik deze zou kunnen toepassen binnen mijn applicatie en welke het beste overeenkomt met het doel van mijn applicatie.

# Waarom ga ik het onderzoeken?

Ik ga het onderzoeken omdat dit heel belangrijk is voor het gebruik van de applicatie namelijk het over kunnen zetten van de aangepaste teksten zonder handmatig in bestanden aanpassingen moeten gaan doorvoeren. Aangezien dit precies het probleem is wat ik probeer op te lossen met de vertaalmodule applicatie.

# Resultaten

Momenteel worden de vertaling bestanden allemaal opgeslagen in Yaml dus mijn vertaalmodule moet hier natuurlijk ook mee werken een mogelijke manier zou eventueel zijn om files vanuit de vertaal module te exporteren en dan importeren binnenin de applicatie, maar dit kost misschien wel minder tijd maar is nog altijd verre van optimaal omdat hier nog altijd redelijk wat tijd in zal gaat zitten.

(Boggiano, z.d.), (2022b)

Deze bundel voor Symfony geeft de mogelijkheid voor het importeren naar de database en een GUI om vertalingen aan te kunnen passen, ook geeft een de mogelijkheid om vertalingen van een database naar een bestand te kunnen exporteren naar bijvoorbeeld yml. En nieuwe vertalingen toe te voegen aan de database was natuurlijk ook mooi meegenomen is en binnen mijn applicatie totaal niet fout zou zijn. Dit geeft ook de mogelijkheid om beide vertalingen van bestanden en de database te gebruiken wel zullen bij dubbel bestaande vertalingen de database het bestand overschrijven.

![image](https://user-images.githubusercontent.com/71487939/235655624-b122dee9-32b2-4fc2-975e-bc1e8a789846.png)

Dit is met gebruik van de bundel en het enige probleem wat ik hier wel al meteen mee zie is dat het totaal niet overzichtelijk is en bij veel verschillende vertalingen kan dit verwarrend worden. Dus deze oplossing zou zeker aangepast moeten worden om het overzichtelijk te houden.

(_Translation and Localization in Symfony 3.4 and 4.0/ Unity Group_, z.d.)

Voor data/vertalingen die aangepast moeten kunnen worden door de gebruiker kan het handig zijn een tabel te maken voor de vertalingen zolang dit niet te veel invloed heeft op de performance.

(_Symfony Translation Bundle — PHP Translation 1.0.0 documentation_, z.d.)

Heeft ook een Symfony WebUI waardoor de vertalingen makkelijk aangepast kunnen worden door iedereen die kan lezen.

Hierbinnen zoals laten zien op de foto zijn er ook verschillende domeinen waar de gebruiker uit kan kiezen waardoor het overzichtelijk blijft ![image](https://user-images.githubusercontent.com/71487939/235655651-810d81b7-c7c3-45ee-abcb-68a88ab119fd.png)

(_About Loco, Translation management_, z.d.)

Loco is een Vertaling manager waar de vertalingen vertaald kunnen worden en dan direct geïntrigeerd met de applicatie waar developers Keys kunnen pushen voor andere gebruikers om de vertalingen te kunnen aanpassen

Natuurlijk ook een manier om data binnen te halen van een andere applicatie is doormiddel van het gebruik van een API die dan wordt aangeroepen door de hoofdapplicatie en die dan als het goed is de nodige data/bestanden binnenkrijgt. Wat ook een mogelijkheid is het gebruik van een Docker container database die beide applicaties gebruiken waar alle vertalingen dan opgeslagen worden en aangepast kunnen worden.

(Z.d.-e)

Symfony heeft ook de mogelijkheid om de API van enkele vertaling providers te gebruiken binnen het config bestand en deze binnen te halen en up te daten door de console misschien is dit ook wel een mogelijkheid voor mijn applicatie.

(Z.d.-b)

Het is mogelijk om binnen symfony meerdere databases te gebruiken dit zou dan hopelijk minimale impact hebben op de applicatie omdat als het goed is de vertalingen binnenhalen maar 1 keer hoeft te gebeuren deze zou dan in een nieuwe Docker container zitten waar de vertalingen up to date worden gehouden en makkelijk toegankelijk zijn voor iedereen.

(Videos, 2017)

Hier wordt uitgelegd dat er ook een mogelijkheid is om binnen Symfony CSV bestanden te importeren dit is ook een mogelijkheid om deze door de vertaalmodule een CSV-bestand te laten exporteren en deze dan in de nodige applicatie te kunnen importeren en in de database op te slaan.

(_How to Import and Export CSV Files Using PHP and MySQL_, 2022b)

Op deze pagina hetzelfde kunnen importeren en exporteren van database gegevens betekent natuurlijk wel dat het in de database opgeslagen moet worden als deze methode wordt gebruikt tenzij er een mogelijkheid is om deze mogelijk wanneer het binnen de applicatie is ze om te zetten naar YAML-bestanden.

Momenteel wordt het binnen het systeem gedaan door de vertaling bestanden in een aparte git sub module zitten, waardoor de bestanden in hun eigen git repository zitten en hiermee kan ik apart de bestanden inladen en aanpassen binnen mijn applicatie.

**Conclusie**

Ik heb zelf nogal moeite met besluiten welke van deze methodes reëel zijn en goed zouden kunnen werken binnen de applicatie en wat de beste manier zal zijn voor deze methodes. Ik zal dit dus met mijn stagebegeleider (expertinterview?) gaan bespreken en dan over de gevonden of eventueel niet gevonden methodes een keuze te maken om me of te focussen voor de vertaalmodule. Na een gesprek een feedback met mijn stagebegeleider zijn we tot de conclusie gekomen dat het al mogelijk is met de momenteel gebruikte git modules voor de vertalingen dus hier zal ik gebruik van maken.

**Bronnen**

Boggiano, J. (z.d.). _lexik/translation-bundle - Packagist_. [https://packagist.org/packages/lexik/translation-bundle](https://packagist.org/packages/lexik/translation-bundle)

L. (2022b, juni 12). _LexikTranslationBundle/index.md at master · lexik/LexikTranslationBundle_. GitHub. https://github.com/lexik/LexikTranslationBundle/blob/master/Resources/doc/index.md#configuration

L. (2022c, juni 12). _LexikTranslationBundle/index.md at master · lexik/LexikTranslationBundle_. GitHub. [https://github.com/lexik/LexikTranslationBundle/blob/master/Resources/doc/index.md#configuration](https://github.com/lexik/LexikTranslationBundle/blob/master/Resources/doc/index.md#configuration)

_Symfony Translation Bundle — PHP Translation 1.0.0 documentation_. (z.d.). https://php-translation.readthedocs.io/en/latest/symfony/index.html

_Translation and Localization in Symfony 3.4 and 4.0 / Unity Group_. (z.d.). https://www.unitygroup.com/blog/translation-and-localization-in-symfony/

_About Loco, Translation management_. (z.d.). Loco. https://localise.biz/about

Bosch, M. (2018, 11 mei). _Share backend translations with the frontend - Maximilian Bosch - Medium_. Medium. [https://medium.com/@\_Ma27\_/share-backend-translations-with-the-frontend-22daf8a4d6e](https://medium.com/@_Ma27_/share-backend-translations-with-the-frontend-22daf8a4d6e)

_Overview - OroCommerce, OroCRM and OroPlatform Documentation_. (z.d.). Oro Documentation. https://doc.oroinc.com/backend/integrations/import-export/overview/

_Sources — SonataExporter documentation_. (z.d.). https://docs.sonata-project.org/projects/exporter/en/3.x/reference/sources/

S. (z.d.-e). _Translations (Symfony Docs)_. Symfony. https://symfony.com/doc/current/translation.html

Krnetic, B. (2021, 11 december). _Multilingual Symfony API - Q agency - Medium_. Medium. https://medium.com/q-software/multilingual-symfony-api-b31fa5f204fe

S. (z.d.-b). _How to Work with Multiple Entity Managers and Connections (Symfony Docs)_. Symfony. https://symfony.com/doc/current/doctrine/multiple\_entity\_managers.html

Videos, C. R. (2017, 3 november). _How To Import A CSV in Symfony_. Code Review Videos. https://codereviewvideos.com/course/how-to-import-a-csv-in-symfony?utm\_content=cmp-true

_How to Import and Export CSV Files Using PHP and MySQL_. (2022b, juni 14). The Official Cloudways Blog. https://www.cloudways.com/blog/import-export-csv-using-php-and-mysql/
