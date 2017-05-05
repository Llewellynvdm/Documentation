# Personaliseren binnen de Marketing Suite

In de drag-and-drop editor van de [Copernica Marketing Suite](https://ms.copernica.com) 
stel je gemakkelijk e-mails samen. De e-mails verzonden vanuit 
deze editor zijn automatisch responsive en makkelijk in elkaar 
te slepen.

Personaliseren kan op verschillende manieren: een persoonlijke aanhef 
met de voor- en achternaam van de relatie, bepaalde content tonen op 
basis van een interesse, bepaalde producten niet tonen in een aanbieding 
als deze recent zijn aangeschaft, enzovoorts. In de Marketing Suite 
kun je personaliseren met behulp van de volgende syntax:

```text
{$profile/subprofile.<veld>}

Voorbeeld:

Beste {$profile.Voornaam}
```

Je kunt met deze syntax de gegevens van elk database- of collectieveld 
opnemen in een e-mailbericht. Deze code wordt in het verstuurde bericht 
vervangen door de veldwaarde in het profiel van de ontvanger.


## Waar kan ik personaliseren in de drag-and-drop editor

In de  Marketing Suite kun je naast de tekstvelden ook op vele 
andere plaatsen personalisatie toepassen. Deze velden zijn te herkennen 
aan het Dollar `($)` teken in het input-veld. Zo kun je bijvoorbeeld 
de 'from name', het onderwerp, maar ook het 'from adres' aanpassen door 
in deze velden de code toe te passen.


[Ga naar de Marketing Suite](https://ms.copernica.com)