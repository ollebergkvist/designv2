---
---

# Laddningstid

Denna uppgift gick ut på att testa samt dokumentera laddningstiden för 3 olika webbplatser samt att se om några implementeringar kan göras för att förbättra användbarheten samt tiden det tar för respektive sida att ladda. Urvalet kunde göras från en kategori utav webbplatser eller från olika kategorier.

## Urval

Mitt urval gjordes baserat på ett intresse för musikutrustning och teknik, utifrån detta intresse valdes 3 stycken onlinebutiker som jag som privat person har köpt musikutrustning och teknik ifrån, som föremål för denna studie. Två utav webbshopparna är baserade i Sverige medan den tredje är baserad i Tyskland. Affärernas storlek och försäljningssiffror skiljer markant, där JAM endast har en fysisk butik med tillhörande e-handel i Stockholm medan Webhallen är en av sveriges största e-butiker med 22 fysiska butiker i landet och Thomann är Europas största e-butik för musikutrustning. Det var ett medvetet val att välja butiker i olika storlekskategorier för denna studie, detta för att undersöka om där finns en markant skillnad mellan en mindre webbshop kontra en större. Studien utgår från respektive webbplats index-sida.

De utvalda webbplatserna är följande:

-   [Thomann](https://www.thomann.de/)
-   [JAM](http://www.jam.se/)
-   [Webhallen](https://www.webhallen.com/se/)

## Metod

Anträffande metod för denna studie, så användes verktyget PageSpeed Insights utav Google DevTools för att testa respektive sidas Performance betyg som ges mellan 0-100 och därefter dokumenterades betyget. Varje test utfördes både för Mobile och Desktop. Därefter uppmättes laddningstid, antalet resurser samt sidans totala storlek med hjälp utav Network modulen via Google DevTools. Varje test genomfördes 3 gånger och mätvärdena dokumenterades. Slutligen beräknades medelvärdet för respektive testområde.

## Dokumentation

[Excel fil med test-värden från samtliga webbplatser](https://docs.google.com/spreadsheets/d/1sOo9yPkfbl8Sn9v0scScpsU4JZdziNh07ipW3sIoQ5U/edit?usp=sharing)

## Resultat

### Thomann

[FIGURE src=image/thomann.png?w=300 caption="Thomann - indexsida"]

| Webbsida | Prestanda (Mobil) | Prestanda (Desktop) | Laddningstid (s) | Resurser (st) | Storlek (MB) |
| -------- | :---------------- | :------------------ | :--------------- | :------------ | :----------- |
| Index    | 35/100            | 67/100              | 5.45             | 205           | 2.8          |
| Contact  | 40/100            | 55/100              | 2.75             | 32            | 2.1          |
| Studio   | 38/100            | 46/100              | 2.89             | 110           | 1.3          |

-   [Index](https://www.thomann.de/intl/index.html)
-   [Contact](https://www.thomann.de/intl/compinfo_contact.html)
-   [Studio](https://www.thomann.de/intl/studio_equipment.html)

##### Förbättringar:

-   Undvika upprepade omdirigeringar
-   Ta bort oanvänd CSS
-   Minska svarstiderna från servern
-   Ta bort resurser som blockerar renderingen

### JAM

[FIGURE src=image/jam.png?w=300 caption="JAM - indexsida"]

| Webbsida | Prestanda (Mobil) | Prestanda (Desktop) | Laddningstid (s) | Resurser (st) | Storlek (MB) |
| -------- | :---------------- | :------------------ | :--------------- | :------------ | :----------- |
| Index    | 38/100            | 66/100              | 4.23             | 132           | 3.3          |
| Kontakt  | 98/100            | 100/100             | 1.25             | 30            | 0.2          |
| Studio   | 36/100            | 54/100              | 4.05             | 130           | 3.5          |

-   [Index](http://www.jam.se/)
-   [Kontakt](http://www.jam.se/kontaktajam/)
-   [Studio](http://www.jam.se/studio/)

##### Förbättringar:

-   Skicka bilder i modernare bildformat
-   Ta bort oanvänd CSS
-   Koda bilder effektivt
-   Ta bort resurser som blockerar renderingen

### Webhallen

[FIGURE src=image/webhallen.png?w=300 caption="Webhallen - indexsida"]

| Webbsida | Prestanda Poäng (Mobile) | Prestanda Poäng (Desktop) | Laddningstid (s) | Resurser (st) | Storlek (MB) |
| -------- | :----------------------- | :------------------------ | :--------------- | :------------ | :----------- |
| Index    | 41/100                   | 76/100                    | 2.98             | 151           | 1.4          |
| Kontakt  | 36/100                   | 86/100                    | 4.21             | 84            | 1.2          |
| Spel     | 40/100                   | 68/100                    | 2.18             | 150           | 1.6          |

-   [Index](https://www.webhallen.com/se/)
-   [Kontakt](https://www.webhallen.com/se/info/7-Kontakta-oss)
-   [Spel](https://www.webhallen.com/se/section/1-Spel)

##### Förbättringar:

-   Ta bort resurser som blockerar renderingen
-   Skjuta upp inläsningen av bilder som inte visas på skärmen
-   Ta bort oanvänd CSS

## Analys

Den gemensamma nämnaren för samtliga webbplatser är att de har väldigt låga testvärden när det kommer till den mobila prestandan,
antalet person som surfar och konsumerar via mobiler och tablets ökar för varje dag, samtliga webbplatser bör därför se till att försöka
förbättra prestandan för dessa enheter så att de kan förbättra användarupplevelsen för sina kunder.

Rörande de vanligaste förbättringarna som kan implementeras så handlar det i samtliga fall framför allt om att ta bort oanvänd css kod samt resurser som blockerar renderingen
av sidan.

Gällande att ta bort oanvänd css så handlar det först och främst om att inte inkludera css filer som inte används för den specifika sidan samt att kontrollera i respektive css
fil att där inte ligger kod som inte används utav något element, slutligen kan en optimera laddningstiden genom att lägga den kritiska css koden för att måla upp sidan
som inline element direkt i head delen i html filen och därefter asynkront ladda sidans övriga css kod med hjälp utav preload länkar.

Gällande de resurser som blockerar renderingen av sidan, handlar det först och främst att identifiera vilka resurser som är kritiska och vilka som inte är det. Precis som tidigare handlar det även i detta fall om att lägga den kritiska koden som inline element för att göra den första renderingen och därefter bygga upp sidan med preload länkar stegvis. Samt att se till att minifiera all kod.

## Vinnare

| Prisplats | Prestanda Poäng (Mobile) | Prestanda Poäng (Desktop) | Laddningstid (s) | Resurser (st) | Storlek (MB) |
| --------- | :----------------------- | :------------------------ | :--------------- | :------------ | :----------- |
| 1         | Webhallen                | Webhallen                 | Webhallen        | Jam           | Webhallen    |
| 2         | Jam                      | Thomann                   | Jam              | Webhallen     | Thomann      |
| 3         | Thomann                  | Jam                       | Thomann          | Thomann       | Jam          |

Topplistan togs fram genom att jämföra testvärdena för respektive webbplats index-sida. Webhallen är den webbplats som tar hem första platsen
i flest kategorier: prestandan mobilt, prestanda desktop, laddningstid samt storlek och utses därmed som vinnare i testet.

## Absolut laddningstid

En generell riktlinje är att den absoluta laddningstiden bör vara runt 2 sekunder om möjligt.
Gällande de 3 webbplatserna som har analyserats är jag förvånad över deras låga prestanda när jag tittar på testvärdena för laddningstiden, särskilt med tanke på att Webhallen är en av Sveriges största e-butiker inom sitt område och Thomann är Europas största webbshop
för musikutrustning, gällande Jams uppmätta värden har jag något större förståelse då det rör sig om en liten butik i det här sammanhanget. Samtliga webbplatser är hemsidor som jag besökt och shoppat från under en lång tidsperiod och jag har aldrig upplevt och upplever inte heller nu i skrivande stund någon utav hemsidorna som långsamma. Baserat på min personliga upplevelse
anser jag därför att laddningstiden för en snabb hemsida är ca 2s och om värdet överstiger 5s så anser jag webbplatsen som långsam.

## Referenser

-   Beaird, G. (2014). The principles of beautiful web design. 3. uppl., USA: SitePoint Pty. Ltd.
-   Google. (u.å). PageSpeed Insights. https://developers.google.com/speed/pagespeed/insights/ [2019-12-6]
-   Moz. (u.å). Page Speed. https://moz.com/learn/seo/page-speed/ [2019-12-6]
-   Google. (u.å). PageSpeed Insights Rules. https://developers.google.com/speed/docs/insights/rules [2019-12-6]

## Övrigt

Rapporten är skriven av Olle Bergkvist, distansstudent vid programmet Webbprogrammering vid BTH.
