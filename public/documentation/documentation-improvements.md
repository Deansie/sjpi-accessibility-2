
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



        JavaScript:
-------------------