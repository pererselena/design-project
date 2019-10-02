---
---
LESS struktur
=========================

Jag har valt att strukturera LESS-koden i layout filer, moduler och en tema fil samt en bas fil.
Detta är ett bra sätt att strukturera koden då det innebär att man kan återanvända modulerna i många teman och bara byta ut värdet i de variabler man använder.

Jag valde att mestadels ha variabler för färger och typsnitt, övriga delar byttes ut genom att läsa in olika moduler.

Varje tema läste in layout och bas modulerna. De läser även in alla gemensamma moduler samt en unik modul för varje tema, vilket t.ex. innehåller olika hover effekter.

Det här är de moduler som jag använder.


**normalize.css/normalize.less**
Används för att normalisera alla inställningar, marginaler, padding etc så sidan ser så lika ut som möjligt i olika webbläsare.


**@desinax/responsive-menu/less/responsive-menu.less**
Lägger till en responsiv meny.


**module/navbar.less**
Denna modul sätter en grund stil på navbaren, med flex och justify-content för att ändra om utseendet och gömmer hamburger menyn.


**module/header.less**
Den här modulen ändrar om grund utseendet på header regionen med flex. Vi ändrar storlek och utseendet på logon sätter en variable för textfärg av logo.


**module/main.less**
Denna modul sätter en grund struktur och stil på regin-main och använder magicNumber för marginaler. En struktur för sidebar sätts även med denna modul.

**module/footer.less**

Denna modul sätter en grundstruktur för footern, med variabler för färger och använder fontawesome för ikoner.


**module/utils.less**
Den här modulen är för saker som inte passade in på andra ställen. Vi sätter en grundstruktur för .next .previous, bredcrumb och toc.

**module/stylechooser.less**
Denna modul används för att sätta en procentuell width på stylechooser för att göra den responsiv.

**module/responsive.less**
Denna modul innehåller media queries för att köra sidan responsive med olika break-points.

**module/flash.less**
Denna modul sätter en grundstruktur för flash regionen, width: 100%.

**module/multi-col3.less**
Denna modul används för att sätta en grundstruktur och en variabel bakgrundsfärg på de tre kolumerna på index sidan.

**@desinax/typographic-grid/less/typography-font-families.less**
Denna moduler läses in för att hantera typsnitt.


**@desinax/typographic-grid/less/typography-defaults.less**
Denna moduler läses in för att läsa in standard värden för typsnitt, färger, storlek etc för olika element.

**base/base_kmom03.less**
Denna modul sätter några bas värden och variabler. Det här är värden som jag anser alltid skall finnas, men som enkelt går att skrivas över.

**@desinax/vertical-grid/less/grid.less**
Genom denna modul lägger vi till ett vertikalt grid som möjliggör att vi kan anpassa de olika regionerna på sidan till att ta upp olika mycket plats (kolumner) på ett responsivt sätt.

**layout/layout_v3.less**
Denna modul har en grundläggande layput för webbplatsen med grids.

**layout/responsive.less**
Denna modul gör layouten responsiv med oliak break-points.

**layout/regions.less**
Denna modul sätter bakgrundsfärger på regionerna som sedan kan skriva över.

**@desinax/figure**
Dessa moduler används för att styla figure och figurecaptions elementen samt innehåller klasser som styr hur dessa elemente skrivs ut på webbplatsen.

**@fortawesome/fontawesome-free/less/fontawesome.less**
**@fortawesome/fontawesome-free/less/solid.less**
**@fortawesome/fontawesome-free/less/brands.less**
Dessa moduler används för att få till fontawesome ikoner på webbplatsen.


**module/kmom10-design-alternativ.less**
Denna modul är specefika till det alternativa temat. Här ändras stil på olika element och områden som jag vill ändra på i temat. T,ex. backgrundsbilden och hover effekten i navbaren. Hover effekten på toc classen ändras också.

**module/kmom10-design.less**
Denna modul är specefika till default temat. Här ändras stil på olika element och områden som jag vill ändra på i temat. T,ex. hover effekten i navbaren.


Övrigt
-----------------------

Rapport gjord av Elena Perers.
