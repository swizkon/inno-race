

## Innovation:
*Beskriv er idé och vilket unikt kundvärde ni skapar genom den.*

Den molnbaserade portmonnän XingZen är en finansiell tjänst som tar fördelarna med kontanter in i den digitala världen.
Målet med tjänsten är att erbjuda det enklaste sättet att betala mindre summor utan att behöva autentisera sig i onödan.
Tjänsten ska fungera för alla oavsett ålder och nationalitet, även för dem som exempelvis saknar kreditkort eller bankid.

Genom att överföra pengar till en online-plånbok kan man i ett steg utföra en säker betalning till systemet.
För att använda pengar som överförts till kontot behövs ingen ytterliggare autentisering.

## Teknik:
*Beskriv er tekniska lösning och framtida tillväxtmöjligheter.*

Med hjälp av ett enkelt gränssnitt som genererar unika QR-koder kan säljare skapa betalningar, 
som sedan godkänns av köparen genom att scanna QR-koden. (Flöde finns i bifogat dokument)

Första utgåvan av systemet består av app för iOS/android, en web applikation samt ett Web API uppsäkrat enl FAPI guidelines.
Kommande versioner kan tänkas innehålla stöd för exempelvis momsredovisning och kvitto online samt mer detaljerad specifikation.

Den tekniska arkitekturen för v1 grundar sig i event sourcing och netcore alt. erlang/elixir som språk. Detta gör att systemet kan driftas i valfri cloud-plattform.
Vidare tekniker och infrastruktur som kan behöva användas är WebSockets, 

Den första versionen kan vara beroende av extern betaltjänst/checkout som ex PayPal, Amazon eller direktbanksbetalning.

I framtiden behöver man antagligen ta höjd för interaktioner mot smart watch. Detta kan möjligtvis ske genom en ljudsekvens som kan omkodas till ett ID, eller genom GPS-data.

Demo:
https://xingzen-webapp.azurewebsites.net

## Kommersiell möjlighet:
*Beskriv vilken marknadspotential affärsidén har samt tänkta affärsvillkor för produkten/tjänsten.
Beskriv er kund, vad som är viktig för dem och hur når ni dem.*

Målgruppen är alla som idag gillar att använda kontaktlösa kort och/eller swish, men som vill ha ett
enklare och säkrare sätt att skicka betalningar. Det bör gå att 

I första fasen finns det största kundbehovet privatpersoner emellan, exempelvis överföringar av mindre summor
mellan vänner och köp på loppmarknader etc.

Nästa steg är att bygga store-koncept där en kassa-device kan skapa mer specificerade köpordrar och stödja momsredovisning mm.

I och med att det är möjligt att stödja flera valutor bör det i senare skede skapas en handelssite för att växla valutor med andra aktörer i systemet. Dessa aktörer kan både vara privatpersoner eller växlingskontor.

## Entreprenörskap och affärsmässighet:
*Beskriv varför just du/ni kommer lyckas genomföra din/er idé.*

Denna idé dök först upp i mitt huvud under min föräldraledighet för ca 2,5 år sedan. Dock kändes utmaningen för stor att ta sig an just då.
Under de senaste 2 åren har jag genom mitt konsultuppdrag på en digital nisch-bank insett att det alltid finns en chans att utmana rådande tekniker och paradigmer kring betalning. Jag tror att marknaden nu är redo för detta.

En stor drivkraft i varför jag vill realisera detta koncept är att minska missbruk av säkra identifikationer.
På samma sätt som man ej ska ta antibiotika för en simpel förkylning bär man inte heller slentrianmässigt signera med BankID då man köper en kaffe på söndagspromenaden.

För att få ut en MVP tror jag att ett välvalt team med 4-5 personer kan lyckas med detta på ca 45 dagar. 
I detta teamet bör det ingå följande roller: Produktägare, app/frontend utvecklare, backend utvecklare 
med erfarenhet av säkerhet inom finans, testare med erfarenhet av säkerhet inom finans.
