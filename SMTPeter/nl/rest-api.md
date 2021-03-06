# Verzenden via REST API

SMTPeter heeft een eenvoudige en betrouwbare REST API ontwikkeld, waarmee je e-mails 
kunt versturen via het HTTP protocol. Stuur een POST request naar onderstaande URL 
om een e-mail te versturen:

```text
https://www.smtpeter.com/v1/send?access_token={JOUW_API_TOKEN}
```

`{JOUW_API_TOKEN}` is de access token die je via het dashboard kunt opvragen.
De body van de POST request, met daarin de content van de e-mail, kunnen
als JSON worden meegegeven. De opmaak van de request ziet er 
dan als volgt uit:

```text
POST /v1/send?access_token={JOUW_API_TOKEN} HTTP/1.0
Host: www.smtpeter.com
Content-Type: application/json
Content-Length: 246

{
    "recipient":    "john@doe.com",
    "from":         "info@example.com",
    "to":           "john@doe.com",
    "subject":      "Dit is het onderwerp",
    "text":         "Dit is de inhoud"
}
```

SMTPeter gaat, nadat je een request hebt gedaan, meteen aan de slag. Er wordt een MIME 
(e-mail bericht) aangemaakt met de gespecificeerde "from", "to", "subject" en "text" 
velden. De e-mail wordt uiteindelijk op de juiste manier afgeleverd bij de opgegeven recipient.

De data die je meegeeft aan SMTPeter, kan uit verschillende variabelen bestaan.
In bovenstaand voorbeeld wordt het e-mailbericht door SMTPeter opgemaakt,
maar je kunt ook andere parameters gebruiken: bijvoorbeeld omdat je zelf al 
de MIME hebt opgemaakt of om te verwijzen naar een voorgedefinieerde template.
Alle ondersteunde opties, bij het versturen van e-mail, zijn beschreven 
in de [MIME door SMTPeter laten maken](rest-send-json) documentatie.


## Verken de andere toepassingen

De REST API is uitgebreid en geeft je vrijheid in het maken van keuzes:

* [MIME data versturen](./rest-mime)
* [MIME data door SMTPeter laten versturen](./rest-send-json)
* [Versturen naar meerdere afzenders](./rest-send-multiple-recipients)
* [Versturen op basis van een template](./rest-send-template)
* [Geavanceerde verzendopties](./rest-send-advanced)
* [API respons](./rest-api-reaction)

*Alle beschikbare REST calls kun je [hier](./all-rest-calls) vinden.*
