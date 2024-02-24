# Zonnepaneelmetingen

Maak een toepassing *Zonnepaneelmetingen* voor de verwerking van
opbrengstmetingen van zonnepanelen. Een bezitter van zonnepanelen
noteert meestal dagelijks de dagopbrengst (in kWh) van zijn
zonnepanelen. De meting wordt in een tekstbestand *Zonnepanelen.txt*
bewaard. Dit bestand plaats je in de zelf toegevoegde map Bestanden. De
eerste records zijn:

14/03/2019 - 11,8

15/03/2019 - 02,5

16/03/2019 - 09,2

17/03/2019 - 04,6

18/03/2019 - 09,3

19/03/2019 - 08,4

21/03/2019 - 02,4

22/03/2019 - 04,1

23/03/2019 - 14,3

24/03/2019 - 06,7

25/03/2019 - 03,5

27/03/2019 - 14,6

28/03/2019 - 16,1

29/03/2019 - 04,7

.....

Zoals je kan zien staat vooraan de datum van de gemeten dagopbrengst
(dag/maand/jaar), daarna staat steeds " -- ", tenslotte gevolgd door de
dagopbrengst met 1 decimaal cijfer (in totaal steeds 4 posities, dus zo
nodig met voorloopnullen).

Je mag veronderstellen dat er hierin geen fouten staan (bestaande datums
en juiste metingen).

Het venster bevat volgende objecten:

-   Onderaan een statusbar met een *TextBlock* Ready, een *Image*
    DatTime en een *TextBlock* die de datum en tijd weergeeft (zie
    verder).

-   Een tekstvak *TxtResultaat* om resultaten te tonen.

-   Een *Image* om een afbeelding te tonen. Het getoonde beeld is
    [afhankelijk van het seizoen waarin het programma gestart
    wordt]{.underline} (maand van de systeemdatum testen!). Voor
    december, januari en februari wordt "winter.jpg" getoond, voor
    maart, april en mei wordt "lente.jpg" getoond, voor juni, juli en
    augustus wordt "zomer.jpg" getoond en tenslotte wordt voor
    september, oktober en november "herfst.jpg" getoond. Deze 4
    afbeeldingen plaats je in de map Bestanden. Je programma moet tevens
    testen of het betreffende bestand aanwezig is op de betreffende
    locatie. Indien dat niet het geval zou zijn, geef dan een passende
    melding: "Afbeelding winter niet aanwezig", "Afbeelding lente niet
    aanwezig", "Afbeelding zomer niet aanwezig" of "Afbeelding winter
    niet aanwezig".

De toepassing werkt menugestuurd. Voeg volgende menustructuur met 2
hoofdkeuzes toe aan je venster:

-   ***Inlezen***. Deze keuze bevat 2 subitems, nl. Details en
    Samenvatting:

    -   Bij het klikken op de keuze *Details* worden de detailmetingen
        uit het tekstbestand *Zonnepanelen.txt* ingelezen en regel per
        regel getoond in het tekstvak **txtResultaat**. Je mag
        veronderstellen dat het betreffende tekstbestand aanwezig is op
        de door u gekozen locatie. Zie verder voor een voorbeeld van een
        schermafdruk.

    -   Bij het klikken op de keuze *Samenvatting* worden de
        detailmetingen uit het tekstbestand *Zonnepanelen.txt*
        ingelezen. In dit geval worden de details niet getoond, maar
        wordt een samenvatting gegeven: per maand wordt het aantal
        metingen en het gemiddelde van die metingen weergegeven. Zie
        verder voor een voorbeeld van een schermafdruk.

```{=html}
<!-- -->
```
-   ***Opties***. Deze keuze bevat eveneens 2 subitems, nl. *Datum
    tonen/verbergen* en *Achtergrondkleur instellen***.**

    -   Bij het klikken op de keuze *Datum tonen/verbergen* wordt de
        datum en tijd in de statusbalk getoond of verborgen.

    -   Bij het klikken op de keuze *Achtergrondkleur* *instellen* wordt
        de achtergrondkleur van het venster gewijzigd. Bij de start van
        het programma is de achtergrondkleur "geel". Telkens geklikt
        wordt op de keuze Achtergrondkleur instellen verandert
        willekeurig de achtergrondkleur in één van volgende kleuren:
        geel, wit, blauw, rood of groen. Zorg er tevens voor dat er
        nooit 2 keren na elkaar dezelfde kleur geselecteerd wordt.

    -   

***Afdrukvoorbeeld met detailgegevens:***

![Afbeelding met tekst, schermopname, software, computer Automatisch
gegenereerde
beschrijving](./media/image1.png){width="6.399305555555555in"
height="5.634027777777778in"}

***Afdrukvoorbeeld met samenvatting (per maand) van gegevens:***

![Afbeelding met tekst, elektronica, schermopname, software Automatisch
gegenereerde
beschrijving](./media/image2.png){width="6.399305555555555in"
height="5.634027777777778in"}
