Utvärdering av webbplatsers hastighet
=======================

I denna rapport ska tre webbplatser utvärderas, i syfte att undersöka och jämföra webbplatsernas hastighet.

Urval
-----------------------

Som urval för uppgiften undersöks Sveriges tre största e-handelsmarknadsplatser. Definitionen som används för att sammanfatta innebörden av begreppet är följande: E-handel som ger en plattform åt tredjepartssäljare för att kunna erbjuda ett mycket brett utbud av varor.

Sverige har många aktörer som kan räknas som e-handelsmarknadsplatser[^1], men enligt en topplista från branschtidningen Ehandel är de största:

1. Amazon

![Amazon's start page](../image/amazonstartpage.png)

2. Fyndiq

![Fyndiq's start page](../image/fyndiqxmas.png)

3. CDON[^2]

![CDON's start page](../image/cdonxmas.png)

Metod
-----------------------

För att genomföra undersökningen används Chrome DevTools - inbyggd funktionalitet i webbläsaren Google Chrome för utvecklare.[^3] Chrome Dev Tools används för att undersöka webbsidors hastighet. Google PageSpeed Insights[^4] används för att hämta ytterligare mätvärden.

Tre webbsidor jämförs på varje webbplats. Startsidan, sökresultatet samt en produktsida. På varje sida öppnas Chrome Dev Tools. Genom att navigera till fliken Network och ladda om den aktuella sidan hämtas relevant data. Längst ned i Dev Tools sammanställs den sammanlagda laddningsdatan för respektive webbsida, som därefter förs över till en tabell.

Varje webbsida undersöks även med hjälp av PageSpeed Insights. Här hämtas de tre viktigaste mätvärdena som därefter också förs över till tabellen. Datan är beräknad utifrån Core Web Vitals-mätvärden under den senaste insamlingsperioden på 28 dagar.[^5]

Som sökterm används sökfrasen "iPhone 15" för samtliga webbplatser. Som produktsida används det första resultatet för denna sökning.


Resultat
-----------------------

<iframe class="load-speed-data" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQ_4zFfawOsZq0o-9zPH0eyMdJ0QQi1JTC6mNdbtks1PhX9K2odNmIaYViEvEMTLqo_b8ejXBJoQ7Vp/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

### Amazon
För Amazon finns förbättringspotentialen framförallt på produktsidan. Där kan man se att webbsidan ungefär är 2-4 gånger så stor som konkurrenternas, samtidigt som man laddar in betydligt större resurser (16+ MB) och har ett högt värde för DomContentLoaded (1700+ ms). Generellt sett har Amazon också höga värden för CLS.

### CDON
CDON är hela tiden på gränsen när det kommer till mätvärdet för CLS som ligger på 0,1. I ett fall ligger man också över detta. CDON skulle behöva sätta en explicit höjd och bredd på sina bilder för att minimera problemen med CLS.

### Fyndiq
Fyndiq har en startsida som underpresterar kraftigt, med en laddningstid på 2-4 gånger konkurrenternas samt en FID på 220 ms och en CLS som överstiger gränsmätvärdet. Anledningen ser ut att vara JavaScript som körs i bakgrunden. Fyndiqs produktsida presterar däremot väldigt bra.

Analys & Diskussion
-----------------------

Generellt sett presterar webbplatserna bra men det finns förbättringspotential inom vissa områden. Det område som konsekvent har fått sämst betyg enligt PageSpeed Insights är CLS - Cumulative Layout Shift. Detta kan skapa minskad konvertering hos kunderna, som kan uppleva att webbplatsens gränssnitt rör på sig medan de använder den. Lösningen till detta är att ange en explicit höjd och bredd för elementen på webbplatsen, vilket gör att det slutgiltiga gränssnittet kan laddas in direkt, oavsett om det tar längre tid för t.ex. bilder att laddas in.

En annan åtgärd som rekommenderas av PageSpeed Insights är att minimera DOM-trädet, man jag misstänker att det kan vara svårt för stora e-handelswebbplatser som dessa.

### Rangordning
Jag skulle vilja rangordna webbplatserna på följande sätt:

1. CDON
2. Fyndiq
3. Amazon

Motiveringen till att CDON vinner är att webbplatsen konsekevent presterar bra i alla kategorier, till skillnad från Amazon där produktsidan utmärker sig av fel anledingar, och Fyndiq där startsidan sticker ut på samma sätt. Eftersom e-handlarna lever av sina produkter bedömer jag att produktsidan är den viktigaste sidan, och eftersom Fyndiq får mycket goda resultat där räcker det till en andraplats.

### Kommentar
Vad jag uppfattar som långsamt beror väldigt mycket på vilken typ av hemsida det handlar om. Gäller det en webbplats med mycket animationer och liknande har jag inget problem med att vänta i kanske 5-10 sekunder. [Exempel](https://solaria.netlify.app/). Men om det gäller e-handelssidor som i det här fallet vill jag inte att det ska ta mer än 2 eller 3 sekunder innan varje sida laddas. Jag upplever att webbplatserna som jag valde klarar av det bra, och det var därför som jag valde att använda de genomsnittliga Web Vitals-mätvärdena från de senaste 28 dagarna istället för mätvärdena för just den sökningen (som alltså var betydligt högre). Jag tyckte att de genomsnittliga värdena bättre återspeglade min upplevelse.

Författare
-----------------------

David Allert.

[^1]: [Ehandel, Lista: Här är alla marknadsplatser i Norden, [hämtad 2023-12-03]](https://www.ehandel.se/har-ar-alla-marknadsplatser-i-norden-resurseffektivt-verktyg)
[^2]: [Ehandel, Topplista: Här är Sveriges 100 största e-handlare, [hämtad 2023-12-03]](https://www.ehandel.se/forum/har-ar-sveriges-100-storsta-e-handlare/)
[^3]: [Chrome DevTools, [hämtad 2023-12-03]](https://developer.chrome.com/docs/devtools/)
[^4]: [Google PageSpeed Insights, [hämtad 2023-12-03]](https://pagespeed.web.dev/)
[^5]: [Web Vitals, [hämtad 2023-12-03]](https://web.dev/articles/vitals)