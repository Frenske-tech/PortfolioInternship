Onderzoek vertaalmodule

**Hoe ga ik de front-end van de vertaal module inrichten om de verschillende categorieën,**

**Waar heel veel vertalingen voor zijn, overzichtelijk weer te geven?**

Francois haan

28/03/2023

# Versiebeheer

| **Versie** | **Datum** | **Auteur(s)** | **Wijzigingen** | **Status** |
| --- | --- | --- | --- | --- |
| 0.1 | 28/03/2023 | Francois Haan | 1ste versie opzet document | Klaar |
| 1.0 | 29/03/2023 | Francois Haan | 1ste versie | Klaar |
| 1.1 | 31/03/2023 | Francois Haan | Verder werken resultaat en conclusie | Klaar |
| 1.2 | 03/04/2023 | Francois Haan | Verder werken resultaat en conclusie over hoe de pagina het beste in te richten | Klaar |
| 1.3 | 05/04/2023 | Francois Haan | Conclusie verder afgewerkt | Klaar |
| 1.4 | 06/04/2023 | Francois Haan | Toevoeging aan conclusie en zinsopbouw en taalfouten verbeterd | Klaar |

Contents

**[Versiebeheer 2](#_Toc128580471)**

**[Wat ga ik onderzoeken? 4](#_Toc128580472)**

**[Hoe gaat ik het onderzoeken? 5](#_Toc128580473)**

**[Waarom ga ik het onderzoeken? 6](#_Toc128580474)**

**[Resultaten 7](#_Toc128580475)**

# Wat ga ik onderzoeken?

Ik ga onderzoeken hoe ik een op een goede en duidelijke manier veel verschillende teksten aan laten passen en de domeinen hierbinnen zonder een enorme muur van tekst voor de gebruiker om doorheen te spitten.

Ook zal ik hierin een klein onderzoek doen naar de verschillende front-end frameworks en kijken of er een is die mij specifiek aanspreekt voor dit project. En wat de voordelen zijn een front-end framework gebruiken. Ik zal hierbij wel rekening ermee houden dat momenteel binnen het systeem bij Performation Vue wordt gebruikt.

# Hoe gaat ik het onderzoeken?

Ik zal voor dit onderzoek literatuur onderzoek en available product analysis gaan toepassen.

Available product analysis doormiddel van kijken naar bestaande vertaling beherende applicaties en hier onderzoeken hoe het overzicht van alle verschillende teksten beheerd wordt.

Literatuur onderzoek zal ik onderzoek doen door onderzoek te doen naar eventuele front-end tips en principes om het overzicht te behouden als er gewerkt wordt met veel en verschillende teksten. Dit zal ik ook toepassen in mijn onderzoek naar een geschikte front-end framework om mee te werken.

# Waarom ga ik het onderzoeken?

Het hele doel van mijn applicatie is om tijd en geld te besparen en development kracht te kunnen besparen dus daarom is het heel belangrijk dat de gebruikers niet lang bezig hoeven zijn met het zoeken naar de juiste plek om het aan te passen. En het onderzoek naar de front-end zodat ik weet wat de voor en nadelen van een aantal front-end frameworks en welke het beste zouden aansluiten binnen mijn project

# Resultaten

**Wat is een javascript framework**

Alles wat te doen is met javascript maar kan tijdintensief zijn frameworks zijn een soort verzameling van templates om sommige functionaliteiten sneller toe te kunnen voegen.

Dan is het makkelijker dan het vanaf het begin te moeten maken heb je al een bestaande structuur om op te bouwen waardoor developers complexere applicatie makkelijk en efficiënter kunnen opbouwen. Ook is een javascript framework een collectie van javascript bibliotheken om code snippits te kunnen gebruiken.

**Waar wordt een javascript framework voor gebruikt?**

Javascript frameworks worden gebruikt om het proces van web applicaties maken te versimpelen en versnellen. Developers hebben toegang tot pre-written code en een structuur om op te bouwen wat veel tijd scheelt. Frameworks kunnen ook taken zoals data management, user interface maken en server side communicatie voorzien onder andere, frameworks maken web development makkelijker en sneller.

**Wat doet een javascript framework?**

Frameworks zijn een structurele basis van een groter component wat zorgt voor veel basis functionaliteiten met minimale inspanning van het implementeren van het framework. Wat heel veel kan helpen bij het maken van een user interface of bij het gebruik van veel data. Kan de functionaliteiten binnen het framework gebruikt worden wat tijd en werk scheelt.

**Verschillende javascript frameworks**

- React
- Vue
- Angular

Er zijn er natuurlijk nog veel meer maar ik heb gekozen op basis van ervaring en populariteit om specifieker onderzoek te doen over deze 3 frameworks.

**React**

Voordelen

- Makkelijk te leren
- Herbruikbare componenten
- Grote community
- Snelle updates
- Gemaakt door facebook

Nadelen

- JSX syntax kan ingewikkeld zijn om te leren
- Documentatie

React is het populairste front-end framework en met facebook als developer erachter, heeft het ook een groot bedrijf en veel developers. Het heeft ook een hele grote community en heeft een relatief makkelijk leercurve met uitzondering van het gebruik van JSX. Wel is de documentatie niet optimaal wat het initiële werk en oplossingen vinden zou kunnen vertragen in tegenstelling tot alternatieven

**Vuejs**

Voordelen

- Snel en klein
- Goeie documentatie
- Beginner vriendelijk
- Makkelijk te begrijpen syntax
- Actieve community

Nadelen

- Relatief nieuw en niet gemaakt door een bedrijf maar door individuele
- Weinig plug-ins
- Niet ondersteund door grote bedrijf

Vuejs is een van de beste front-end frameworks voor een spa(single page applicatie) vanaf het begin of kleinere web development projecten, en is relatief populair maar heeft wel geen groot bedrijf zoals facebook erachter. Vue heeft wel goede documentatie en een behulpzame community en is redelijk makkelijk om mee te werken en aan te wennen in tegenstelling tot andere front-end frameworks

**Angular**

Voordelen

- Support van google
- Sterke community
- Goed training materiaal
- Dependency injection
- Betere server performance

Nadelen

- Moeilijk te leren voor beginners
- Veel code en veel in grootte

Angular wordt ondersteund door google, heeft een grote en actieve community. Is wel moeilijk voor beginnende developers en ik heb in tegenstelling tot Vue en React nog geen ervaring met Angular. Wel zijn de trainingen, video's en documentatie die Angular biedt goed en duidelijk en kunnen de leercurve hiervan iets minder moeilijk maken.

Ik heb enkele tips die je kan gebruiken wanneer een site/pagina veel tekst heeft namelijk:

Lineclamp gebruiken waardoor niet elke tekst volledige getoond hoeft te worden, meerdere fonts gebruiken voor enig verschil, grootte van de teksten laten verschillen. Op de lijn lengte letten, spacing tussen lijnen, readability, tekst-alignement gebruiken

Mijn eigen idee om het overzichtelijk te houden is ook te werken in categorieën en hier 1 van te laten selecteren en hierbinnen verder kunnen filteren tussen teksten bijvoorbeeld doormiddel van een zoekbalk die werkt met Ajax waardoor real time zoekopdrachten uitgevoerd kunnen worden en er minimale tijd gebruikt wordt met zoeken naar de plek waar het momenteel opgeslagen staan, het enigste risico wat ik hierbij zie is dat heel incidenteel zelfde vertalingen zijn.

(_Symfony Translation Bundle — PHP Translation 1.0.0 documentation_, z.d.)

Enkele voorbeelden van Symfony bundles die de mogelijkheid bieden voor aanpassingen te maken doormiddel van een User interface

![](RackMultipart20230411-1-kiuzsu_html_21cd1c05145e0976.png)

Dit kan zeker iets van een front-end styling gebruik maken maar hoe het wordt laten zien met de verschillende talen/locaties en de verschillende domeinen waardoor het overzichtelijk blijft.

(2019)

Enkele tips voor het gebruik van input velden is bijvoorbeeld het gebruik van een achtergrondkleur voor alles behalve de input zelf zodat het duidelijk is voor de gebruiker waar de informatie ingevuld moet worden.

![](RackMultipart20230411-1-kiuzsu_html_7541627b5075b75f.png)

Ook is het belangrijk dat er voor de gebruiker duidelijk wordt aangegeven waar er momenteel tekst ingevuld wordt zodat dingen niet op de verkeerde plek worden ingevoerd. Dit kan onder andere doormiddel van gebruik van kleur een dikkere rand om de input heen. Wel moet bij kleuren altijd rekening gehouden worden met kleurenblinden gebruikers.

(Babich, 2018)

Voor labels moet je maar 1 of 2 woorden gebruiken zodat het meteen duidelijk is binnen mijn systeem zou dit hoogstwaarschijnlijk de momentele key binnen de code worden.

Ook moet het input veld niet te groot of te klein zijn binnen mijn applicatie kan dit nogal veel verschillen van elkaar dus zal ik mogelijk verschillende groottes afhankelijk van de input gaan hebben . zoals eerder ook al genoemd ook focus op input veld zodra iets wordt ingevoerd. Ook labels niet in allemaal hoofdletters.

De tekst van de inputs moet ook groot genoeg zijn hier wordt aangegeven om 16px aan te houden afhankelijk van wat er nog meer op de pagina staat.

-

**Conclusie**

Na te hebben gekeken naar de verschillende front-end frameworks kan ik naar alle voor en nadelen kijken, maar het feit dat binnen Performation er wordt gewerkt met Vue was ik al meer in die richting te kijken. Maar ook dat ik persoonlijk al ervaring heb met Vue lijkt mij dit de beste keuze voor dit project vooral aangezien de vertaal module geen grote complexe applicatie wordt lijkt Vue mij voldoende tegenover React en Angular.

Ik heb doormiddel van nog meer tips te hebben gevonden voor onder andere input velden en het weergeven van informatie die ik kan toepassen om mijn applicatie overzichtelijk te maken ook het verstoppen van op dat moment niet relevante informatie of het gebruik van accordeons kan goed zijn om het overzichtelijk te houden, het gebruik van bijvoorbeeld een zoekopdracht en kunnen wisselen tussen de verschillende domeinen En dividers gebruiken tussen elementen zodat het overzichtelijker is.

Ook een eventueel hulpmiddel om het compacter te maken zou ook kunnen zijn door de domeinen ook in verschillende verzamelgroepen te zetten zoals bijvoorbeeld Orso, verpleegkundig personeel etc. waardoor er mogelijkheid is om verder te filteren waardoor de gebruiker niet door eindeloze lijnen heen moet gaan.

**Bronnen**

_9 Best JavaScript Frameworks to Use in 2023_. (z.d.). https://ninetailed.io/blog/best-javascript-frameworks/

Arora, S. K. (z.d.). _10 Best JavaScript Frameworks to Use in 2023_. Hackr.io. https://hackr.io/blog/best-javascript-frameworks

_Top 10 Popular Frontend Frameworks to Use in 2023 | AppMaster_. (z.d.). AppMaster - ultimate all-in no-code platform. https://appmaster.io/blog/popular-frontend-frameworks

_What is Virtual DOM?_ (z.d.). Stack Overflow. https://stackoverflow.com/questions/21965738/what-is-virtual-dom

_React Virtual DOM - Using Virtual DOM in React_. (z.d.). [https://www.knowledgehut.com/blog/web-development/react-virtual-dom](https://www.knowledgehut.com/blog/web-development/react-virtual-dom)

_CSS tips and tricks for text-based content | Angry Nerds_. (z.d.). AN. https://angrynerds.co/blog/css-tips-and-tricks-for-text-based-content/

Opara, C. (2022, 4 augustus). _Guidelines for Working with Text in UI Designs - Bootcamp_. Medium. https://bootcamp.uxdesign.cc/guidelines-for-working-with-text-in-ui-designs-933d4edd6aa5

Yalanska, M. (2021, 11 mei). _UX Design: How to Make User Interface Readable_. Tubik Blog: Articles About Design. https://blog.tubikstudio.com/ux-design-readable-user-interface/

_Symfony Translation Bundle — PHP Translation 1.0.0 documentation_. (z.d.). https://php-translation.readthedocs.io/en/latest/symfony/index.html

_What are some good methods for displaying large amounts of text?_ (z.d.). User Experience Stack Exchange. https://ux.stackexchange.com/questions/61323/what-are-some-good-methods-for-displaying-large-amounts-of-text

A. (2019, 30 september). _The Best Way to Display Text Fields_. UX Movement. https://uxmovement.com/forms/the-best-way-to-display-text-fields/

Babich, N. (2018, 20 juni). _Designing Perfect Text Field: Clarity, Accessibility and User Effort_. Medium. https://uxplanet.org/designing-perfect-text-field-clarity-accessibility-and-user-effort-d03c1e26004b

_Best way to display large amounts of user data on a single page?_ (z.d.). User Experience Stack Exchange. https://ux.stackexchange.com/questions/16237/best-way-to-display-large-amounts-of-user-data-on-a-single-page
