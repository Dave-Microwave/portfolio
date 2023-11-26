<main markdown="1">

Utvärdering av webbplatsers känsla
==================================

I denna rapport ska tre webbplatser utvärderas, i syfte att undersöka och jämföra webbplatsernas färgval, typsnitt och känsla utifrån ett designperspektiv.

Urval
-----------------------

Som urval för uppgiften undersöks Sveriges tre största e-handelsmarknadsplatser. Definitionen som används för att sammanfatta innebörden av begreppet är följande: E-handel som ger en plattform åt tredjepartssäljare för att kunna erbjuda ett mycket brett utbud av varor.

Sverige har många aktörer som kan räknas som e-handelsmarknadsplatser[^1], men enligt en topplista från branschtidningen Ehandel är de största:

1. Amazon
2. Fyndiq
3. CDON[^2]

Metod
-----------------------

### Verktyg
För att genomföra undersökningen används Chrome DevTools - inbyggd funktionalitet i webbläsaren Google Chrome för utvecklare.[^3] Syftet med Chrome DevTools är att undersöka vilka typsnitt de olika webbplatserna använder sig av.

Adobe Color är en webbplats för att skapa färgpaletter.[^4] Adobe Color används i undersökningen som ett hjälpmedel för att förstå tanken bakom webbplatsernas färgval. För att säkerställa att rätt färger jämförs används Eye Dropper som är ett tillägg i Chrome[^5], detta verktyg gör att de exakta färgkoderna som används kan hämtas från respektive webbplats.

### Genomförande
Uppgiften genomfördes genom att webbplatsernas respektive startsida besöks. För att fånga upp alla typsnitt som används på startsidan används Chrome DevTools genom att man navigerar till fliken "Elements" och klickar på HTML-taggen "body". Därefter navigerar man till fliken "Computed" och öppnar menyn "font-family".

Därefter används Eye Dropper för att hämta webbplatsens primära färger. Dessa klistras sedan in i Adobe Color för att ta reda på vilken typ av färgschema som används.

Resultat
-----------------------

### Amazon

![Bild från startsidan på Amazon.se](../image/amazon.png)

#### Typsnitt

Amazon Ember, Arial, sans-serif

#### Färgval

Amazons färgschema använder sig av komplementärfärger för att skapa kontraster. I stort sett använder hela startsidan samma färgschema.

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #195851">
<td style="height: 50px; width: 50px; background-color: #00453E">
<td style="height: 50px; width: 50px; background-color: #F24C10">
<td style="height: 50px; width: 50px; background-color: #e3e6e6">
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
</tr>
</table>

### Fyndiq

![Bild från startsidan på Fyndiq.se](../image/fyndiq.png)

#### Typsnitt

__Mulish_cfc608, __Mulish_Fallback_cfc608

#### Färgval

Fyndiqs färgschema använder sig av en form av Triad-palett. Man har dock valt bort den tredje färgen till förmån för mer neutrala färger. Längre ned på startsidan används en större blandning av färger för att ge olika uttryck till separata kampanjer.

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #00838A">
<td style="height: 50px; width: 50px; background-color: #ff5776">
<td style="height: 50px; width: 50px; background-color: #ffffff">
<td style="height: 50px; width: 50px; background-color: #171717">
<td style="height: 50px; width: 50px; background-color: #454545">
</tr>
</table>

### CDON

![Bild från startsidan på CDON.se](../image/cdon.png)

#### Typsnitt

Manrope, -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial,sans-serif

#### Färgval

Vid första anblick ser färgschemat ut att vara monokromt, men genom att jämföra de exakta färgkoderna kan man se att färgschemat är komplementärt. Längre ned på sidan används den gula färgen i stor utsträckning. 

<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #ffffff">
<td style="height: 50px; width: 50px; background-color: #fff001">
<td style="height: 50px; width: 50px; background-color: #140728">
<td style="height: 50px; width: 50px; background-color: #3a2f4a">
<td style="height: 50px; width: 50px; background-color: #000000">
</tr>
</table>

Analys & diskussion
-----------------------

Dagens datum är 2023-11-25. Det är signifikant eftersom det dels närmar sig jul (en stor shopping-högtid) och dels för att Black Friday (också något av en shopping-högtid) inföll igår. Detta är de stora e-handelsmarknadsplatserna medvetna om och har därför i stor utsträckning anpassat designen på sina webbplatser för att signalera till sina kunder att de har bra erbjudanden. Amazon har därför frångått sin kännetecknande gula färg, CDON har frångått sin kännetecknande gröna färg och Fyndiq har blandat in mer svart på startsidan. Jag var medveten om detta när jag valde den här typen av hemsidor, men jag blev ändå lite förvånad över att de i så stor utsträckning har frångått sina klassiska varumärkesfärger. Om jag hade fått chansen att råda dem i deras designprocess hade jag förespråkat att man skulle behållit mer av sina vanliga färger i kampanj-designerna.

Fyndiq och CDON använder båda olika sans-serif typsnitt, medan Amazon använder ett eget typsnitt - Amazon Ember.[^6] Jag bedömer att samtliga företag vill signalera modernitet, kanske eftersom de till stor del säljer varor som använder modern teknik.

### Källor

Omsättningsdatan kommer främst från 2021-års bokslut. Värt att notera är att Elgiganten inte ingår i topplistan, trots att företaget omsatte nästan 16 miljarder SEK 2021.[^7] Detta tyder på att datan från Ehandel skulle kunna vara felaktig.

<!-- Referenser -->

[^1]: [Ehandel, Lista: Här är alla marknadsplatser i Norden, [hämtad 2023-11-25]](https://www.ehandel.se/har-ar-alla-marknadsplatser-i-norden-resurseffektivt-verktyg)
[^2]: [Ehandel, Topplista: Här är Sveriges 100 största e-handlare, [hämtad 2023-11-25]](https://www.ehandel.se/forum/har-ar-sveriges-100-storsta-e-handlare/)
[^3]: [Chrome DevTools, [hämtad 2023-11-25]](https://developer.chrome.com/docs/devtools/)
[^4]: [Adobe Color, [hämtad 2023-11-25]](https://color.adobe.com/sv/create/color-wheel)
[^5]: [Eye Dropper, [hämtad 2023-11-25]](https://eyedropper.org/)
[^6]: [Amazon Ember, [hämtad 2023-11-25]](https://developer.amazon.com/en-US/alexa/branding/echo-guidelines/identity-guidelines/typography)
[^7]: [Alla Bolag, Elgiganten Aktiebolag, [hämtad 2023-11-25]](https://www.allabolag.se/5564714474/bokslut)

Författare
-----------------------

David Allert.

</main>