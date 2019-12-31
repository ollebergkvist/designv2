---
---

# Webbplatsdesign

Denna uppgift gick ut på att först och främst välja ut ett visst antal webbplatser utav samma kategorityp och därefter analysera och dokumentera resultatet utifrån aspekten webbplatsdesign och aktuella trender.

## Urval

Den gemensamma nämnaren för urvalet av webbplatser som ingår i denna studie är att samtliga är webbshoppar med Sverige som bas. Urvalet gjordes genom att slumpmässigt välja ut 3 stycken webbplatser från Ehandel.se topplista över Sveriges största e-handlare under 2019. Topplistan är baserad på en analystjänst vid namnet Ehandelsindex som har hämtat in data från företagens senast inlämnade bokslut, där grundkravet har varit att minst 50 % utav butikernas omsättning måste komma från e-handel för att ha möjlighet att kandidera till listan.

De utvalda webbshopparna är följande:

-   [Stadium](https://www.stadium.se/)
-   [Junkyard](https://www.junkyard.se/guys)
-   [Care of Carl](https://www.careofcarl.com/)

## Metod

Anträffande metod för denna studie, så har respektive webbplats studerats först och främst med avseende till deras layout men även val utav färgschema och typografi ingår i studien. Därefter har analyserna jämförts för att se om där tycks finnas en gemensam trend för utformningen utav denna kategori utav webbplatser. Gällande verktyg för att inspektera färgval så har ColorZilla använts medan verktyget inspector från Google Developer tools har brukats för att ta fram vilka typsnitt som återfinns på webbplatserna. Studien utgår i respektive fall från varje webbplats index sida om inte annat anges.

## Resultat

### Stadium

[FIGURE src=image/stadium.png?w=300 caption="Stadium - indexsida"]

##### Layout

Generellt gällande Stadiums webbplats har man valt en så kallat horisontell layout där man valt att varva regioner med "fullscreen design", dvs. regioner som sträcker sig utöver hela fönstrets bredd med regioner som har fått en fixed width. Exempel som tydligt tilldelats den förstnämnda egenskapen är navbaren, footern samt flashbilden. Medan ett exempel på region som har fått en fixed width är body delen som är har fått en bredd om 1440px. Navbaren är en så kallad statisk top meny som först och främst är indelad i 3 huvudkategorier, stadium, stadium outlet och sneakers point, där man implementerat en geometrisk form i form utav en semi button knapp med rundade kanter som smälter ihop med navbaren på ett väldigt fint sätt. För underkategorierna har man valt att implementera en dropdown meny som i sin tur innehåller collapsable submenus för somliga kategorier. Efter navbaren möts besökaren utav en flashbild i stor skala som upptar hela webbfönstrets bredd och som fått accentfärgen "Pedua". I övrigt när det kommer till accent färger så används en orange färg sparsamt för att markera specialpriser samt en enstaka knapp. Flashbilden däremot nyttjas för en kampanj för att påminna om att det snart är jul och att det är presenttider, det är intressant att man valt en ljusgrön / turkos nyans i detta fall över en röd för att markera julen. Därefter möts besökaren utav body delen som har ett tydligt grid system där man använder sig huvudsakligen utav jämna nummer för dela upp de objekt som man önskar att presentera och marknadsföra. Man har även valt att använda margins mellan objekten i gridsystemet, vilket jag förmodar grundar sig i att man vill skapa en luftigare layout och design. Stundvis förekommer det enstaka objekt som får lov att ta upp body delens fixerade bredd om 1440px. Slutligen möts besökaren utav en så kallad expansive footer som huvudsakligen fungerar som en kompletterande navigationsmeny.

##### Färgschema

Färgschema (Akromatiskt):

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #231F20">
<td style="height: 50px; width: 50px; background-color: #333333">
<td style="height: 50px; width: 50px; background-color: #404040">
<td style="height: 50px; width: 50px; background-color: #E4E4E4">
<td style="height: 50px; width: 50px; background-color: #F1F1F1">
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
</tr>
</table>

Accentfärg:

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #80AC91">
<td style="height: 50px; width: 50px; background-color: #8DB4A3">
<td style="height: 50px; width: 50px; background-color: #FF6600">
</tr>
</table>

##### Typografi

-   H1: StadiumSansW01
-   H2: StadiumSansW01
-   H3: StadiumSansW01
-   Brödtext: StadiumSansW01
-   Typkaraktär: Samtliga är utav typen sans-serif

### Junkyard

[FIGURE src=image/junkyard.png?w=300 caption="Junkyard - indexsida"]

###### Layout

Junkyards layout påminner mycket om Stadiums, även här har man tillämpat en så kallad horisontell design med en blandning av fixed samt fullwidth design för webbplatsens regioner. Det är precis som i fallet Stadium exakt samma regioner som har fått en full eller fixed width. Det enda som skiljer är att body delen har fått en mindre fixed width, i detta fall är det 1140px som gäller. Till skillnad från Stadiums navigeringsmeny så har man här valt ett mer lekfullt typsnitt för a-länkarna, detta i form utav sans-serif typsnittet Bebas Neue. Man jobbar även här med att försöka implementera enstaka geometriska former i en annars minimalistisk komposition, i detta fall är det sökfältet som har fått rundade kanter samt en liten pyramid konstruktion som hjälper användaren att se vilken huvudkategori i menyn som användaren pekar på. I övrigt är det raka linjer som gäller rätt igenom designen. Även här möts besökaren utav en dropdown meny, men här har man valt att expandera menyn genom en hover effekt till skillnad från Stadiums meny där besökaren behöver klicka på en utav huvudkategorierna för att öppna submenyn, detta skapar både rörelse och UX i form utav interaktivitet för besökaren. Precis som i Stadiums fall så möts besökaren direkt efter menyn utav en väldigt stor flashbild med full width, flashbilden används även här för att annonsera en kampanj och här gäller det julrea om upp till 70 % av originalpriserna. Det är även just här som man valt att använda en accent färg, men i detta fall är det inte bakgrundsfärgen som tilldelats accentfärgen utan det är text elementet "SALE", samma rosa färg används för att markera a-länken REA i toppmenyn. Därefter följer body delen som även här har fått en grid-baserad layout, där objekten har fått margins mellan varandra. Det enda som skiljer är i stort sett att man här har valt att arbeta med udda antal nummer i gridet i somliga regioner samt att man har valt att varva och dela upp regioner från varandra genom att använda en vit bakgrundsfärg samt en beige accent färg. Precis som i Stadiums fall så har man valt en väldigt fet footer som på ett liknande sätt används som en expanderad navbar.

##### Färgschema

Färgschema (Akromatiskt):

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #141414">
<td style="height: 50px; width: 50px; background-color: #2F2F2F">
<td style="height: 50px; width: 50px; background-color: #333333">
<td style="height: 50px; width: 50px; background-color: #F9F9F9">
<td style="height: 50px; width: 50px; background-color: #FFFFFF">

</tr>
</table>

Accentfärg:

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #ECDDCF">
<td style="height: 50px; width: 50px; background-color: #FF3D63">
</tr>
</table>

##### Typografi

-   H1: Museo Sans
-   H2: Museo Sans
-   H3: Museo Sans
-   Brödtext: Museo Sans
-   Typkaraktär: Museo Sans är utav typen sans-serif

### Care of Carl

[FIGURE src=image/careofcarl.png?w=300 caption="Care of Carl - indexsida"]

##### Layout och design

Care of Carls webbplats följer i stort sätt samma trender samt typ utav layout som föregående webbplatser. Vad som skiljer denna webbplats framförallt åt är att man här valt att arbeta med ett monokromatiskt färgschema i blått som framför allt används för att markera sidans olika regioner samt enstaka knappar. Det är ett färgschemat som utgår från logotypens marinblåa färg. Även stora delar utav sidans text element har fått olika nyanser i denna blåa färg, framför allt handlar det om rubriker och länkar. Något annat som skiljer denna webbshop åt från Stadiums och Junkyards är att man här valt att ge flashbilden samma width som body delen, vilket är 1150px. Denna webbplats tar även hem priset i den webbplats som har den mest expansiva footern av de tre, den är så pass stor att den upptar en hel 15 tums skärm. Något annat som skiljer Care of Carl åt är att man inte jobbat med interaktiva bilder på samma sätt som de två andra, denna sida saknar helt och hållet zoom effekter på sina försäljningsobjekt. Den enda interaktiviteten som tycks skådas på index-sidan är en hover effekt som underlinar huvudfabrikerna i navigeringsmenyn.

##### Färgschema

Färgschema (Monokromatiskt):

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #051D29">
<td style="height: 50px; width: 50px; background-color: #09283A">
<td style="height: 50px; width: 50px; background-color: #092636">
<td style="height: 50px; width: 50px; background-color: #082939">
<td style="height: 50px; width: 50px; background-color: #F3F3F3">
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
</tr>
</table>

Accentfärg: Ingen

##### Typografi

-   H1: Merriweather
-   H2: Merriweather
-   H3: Merriweather
-   Brödtext: Lato
-   Typkaraktär: Merriweather är utav typen serif medan Lato är sans-serif

## Analys

Gemensamt för samtliga webbplatser är att man valt en horisontell layout och där man valt att åtminstone tilldela header och footer fullscreen width, medan innehållet i main delen har tilldelats en smalare bredd. Webbplatserna följer alla samma big dropdown meny trend där det enda som skiljer de åt är vilken typ utav eventlyssnare man har lagt för att besökaren ska kunna expandera menyn.

Alla tre webbplatser använder sig även utav en flashbild placerad direkt under headern i stor skala för att marknadsföra relevanta kampanjer. Och därefter följer ett rektangulärt grid-system i main delen där man implementerat mellanrum mellan objekten i samtliga onlinebutiker. Det är ingen som valt att sticka ut genom ett så kallat broken grid system. I alla tre fall har man valt att jobba med huvudsakligen en vit bakgrundsfärg i main delen, detta för att antagligen ge hög kontrast åt de objekt man önskar att sälja. Det är endast Junkyard som valt att varva regionerna i main delen med en beige accentfärg, vilket markerar de olika regionerna på ett tydligt sätt men utan att fokus från bildinnehållet.

Rörande footern så använder alla webbplatser som analyserats så kallade expansive footers, som till skillnad från en reguljär footer inte endast bara innehåller essentiella länkar och copyright disclaimers. Utan här inkluderar man även en kompletterande navigeringsmeny, kontakt information, länkar till sociala medier genom ikoner, prenumeration för nyhetsbrev, köpvillkor och mycket mera. Footern har med andra ord getts högre betydelse och många användare har idag vant sig vid att hitta viktiga länkar längst ner på sidan genom footern.

Gällande val utav färgschema så kan en se en tydlig trend här att det är akromatiska eller monokromatiska färger som gäller samtidigt som man använder en hel del white space i sin design för att skapa ett luftigt intryckt för besökaren. Om accentfärger används så är det extremt sparsamt och endast för att markera särskilda kampanjer i en övrigt minimalistisk design. Då det huvudsakliga innehållet består utav just bilder, så är min teori att man valt den här typen av färger för att ge hög fokus till de objekt man önskar sälja.

Efter att ha studerat de här tre webbplatserna så är det tydligt att man valt att efterfölja samma designmönster och trender. Det är väldigt lite som skiljer sidorna åt både layout som typsnitt som färgmässigt. Alla hemsidor har implementerat sans-serif typsnitt i brödtexten, vilket är känt för att vara den optimala kategorin av typsnitt för webben när det kommer till förhöjd läsbarhet. Det är endast Junkyard som sticker ut genom att välja ett serif typsnitt för somliga rubriker. Övriga webbplatser har hållt antalet typsnitt till ett, vilket förstärker den minimalistiska estetiken som denna typ utav layout utstrålar.

## Referenser

-   Beaird, G. (2014). The principles of beautiful web design. 3. uppl., USA: SitePoint Pty. Ltd.
-   Canva. (u.å). Design Elements & Principles. https://www.canva.com/learn/design-elements-principles/ [2019-12-19]
-   Wikipedia. (2019-12-11). Visual design elements and principles. https://en.wikipedia.org/wiki/Visual_design_elements_and_principles [2019-12-19]
-   Ehandel. (2019-03-07). Topplista: Här är de 100-största e-handlarna i Sverige. https://www.ehandel.se/Har-ar-de-100-storsta-e-handlarna-i-Sverige,14379.html [2019-12-19]

## Övrigt

Rapporten är skriven av Olle Bergkvist, distansstudent vid programmet Webbprogrammering vid BTH.
