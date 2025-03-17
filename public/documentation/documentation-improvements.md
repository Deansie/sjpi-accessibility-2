
Observerade tillgänglighetsproblem:


        HTML:
-------------------
    1. Lang-attribut kommenterad, påverkar skärmläsare
    
    2. Två titlar, förvirrar skärmläsaren

    3. Navigation, dublett-IDn, tabindex inkonsekvent och bruten länk, försvårar navigering
       för personer med nedsatt rörelseförmåga, förvirrar skärmläsare och förvirrar användaren 
       med brutna länkar.

    4. Dubbla H1-taggar, förvirrar skärmläsaren

    5. H2-tag i slutet av sectionen, gör att skärmläsaren inte vet om att den är på en ny section
       med ny rubrik.

    6. Avsaknad av alt-text till bilder, kan inte förklara vad bilderna innehåller om de inte skulle laddas
       ordentligt.

    7. H3 slut-tag på en H1-tag, felaktig semantik. Troligtvis kan inte skärmläsaren ens läsa ut detta.

    8. A-tag där det skulle varit p-tag.

    9. P-taggar där det skulle varit a-taggar till snabblänkarna i footern, orsakar att det inte blir någon
       vidarelänkning som är förväntad av användare. Även redirection till bruten länk förekommer.

    10. Brutna länkar i footern, förvirrar användaren.



        CSS:
-------------------
    1. För låg kontrast mellan färgerna där "terracotta" används

    2. Navigationen försvinner när sidan understiger 768px i bredd men ersätts inte av någon annan
       meny vilket gör navigationen otillgänglig.



        JavaScript:
-------------------
    1. För denna filen tas inladdningen bort i index.html eftersom koden bara är nonsens som skapar
       hinder för sidan att fungera ordentligt.


        Ändringar

        HTML:
-------------------
    1. Språkattribut aktiverat
    
    2. Endast en title-tag

    3. Hamburgermeny-knapp tillagd för att stödja mobilmeny

    4. Navigation: Förtydligat IDn, korrigerat tabindex och ersatt brutna länkar

    5. Endast en h1-tag i hero-sektionen

    6. Start-tag för h1 ändrad till h3 för att slut-taggen var h3

    7. Lagt till alt-texter på bilder som saknade det

    8. Ändrat knappar från div till button

    9. Korrigerat felaktigt använd a-tagg till p-tagg

    10. Korrigerat felaktigt använda p-taggar till a-taggar

    11. Brutna länkar i footer har ersatts med # och rimliga motsvarigheter

    12. Mindre formateringsändringar i början av koden kring meta-taggarna

    13. Tagit bort kommentarerna i början av filen eftersom det förhindrade W3 HTML Validatorn 
        att passera eftersom lang-attributet var för långt från början av filen


        CSS:
-------------------
    1. Färgändring för "terracotta" eftersom den tidigare hade för dålig kontrast mot andra färger, följer nu WCAG AAA

    2. Styling till hamburgermeny som finns tillgänlig från 768px och neråt i bredd för en användarvänlig navigering


        JavaScript:
-------------------
    1. Tagit bort struntkoden som enbart skapade fördröjning på sidan

    2. Lagt till en eventlistener för att få hamburgermenyn att fungera vid klick
