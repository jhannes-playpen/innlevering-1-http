Innlevering #1: HTTP Server
===========================

Oppgaven:
---------

Nesten alle utviklere jobber med HTTP til daglig.Den mest brukte versjonen av HTTP er definert i [RFC 7230](https://tools.ietf.org/html/rfc7230) mm. For at dere skal bli kjent med protokollen går innlevering #1 ut på å lage en minimal implementasjon av protokollen.

Serveren skal bruke parametre fra requesten og svare tilsvarende. Dere kan benytte tjesten [URL Echo](http://ivanzuzak.info/urlecho/) som mal.

HTTP er definert som en request/response protokoll. Det vil si at en klient (typisk en nettleser) oppretter en forbindelse til en server og sender en request. Serveren svarer med en response. Både requesten og responsen er tekst som sendes over nettverket. En typisk utveksling kan se slik ut (fra [RFC 7230](https://tools.ietf.org/html/rfc7230#section-2.1)):

Client request:

     GET /hello.txt HTTP/1.1
     User-Agent: curl/7.16.3 libcurl/7.16.3 OpenSSL/0.9.7l zlib/1.2.3
     Host: www.example.com
     Accept-Language: en, mi


Server response:

     HTTP/1.1 200 OK
     Date: Mon, 27 Jul 2009 12:28:53 GMT
     Server: Apache
     Last-Modified: Wed, 22 Jul 2009 19:15:56 GMT
     ETag: "34aa387-d-1568eb00"
     Accept-Ranges: bytes
     Content-Length: 51
     Vary: Accept-Encoding
     Content-Type: text/plain

     Hello World! My payload includes a trailing CRLF.  


Innleveringen:
--------------

Dere skal levere inn oppgaven i GitHub og jobbe parvis. Dersom du ønsker å være med å påvirke hvem du skal jobbe med, så kan du [fylle ut dette spørreskjema](https://goo.gl/forms/4wHR1X6a7ufjVJh82). Dere kan velge nye grupper til neste innlevering.

I tillegg til koden i GitHub skal dere ta opp en video på 3-8 minutter der dere parprogrammerer litt kode. Screencast-o-matic anbefales som verktøy for video-opptaket, men andre verktøy kan benyttes. En lenke til videoen skal leveres – ikke videoen selv. Husk å åpne for tilgang til videoen («unlisted» i Youtube).


Innholdet i oppgaven er definert i form at et sett med [GitHub issues](https://github.com/jhannes-playpen/innlevering-1-http/issues). Det er lurt å kopiere disse issues til deres eget kopi av prosjektet.




Vurderingskriterier:
--------------------

* Koden må kompilerer og serveren må la seg starte.
* README.md må beskrive hvordan man starter opp serveren
* Det bør være god testdekning på koden
* Serveren bør ikke krasje/falle ned av seg selv
* Klienten bør koble seg fra korrekt
* Prosjektet bør være dokumentert i form av README.md som også bør inneholde:
  * Hvordan man tester løsningen
  * Kommentarer på eget resultat. Hva kunne vært gjort bedre?
  * Eventuelle spørsmål dere trenger svar på for å komme videre.
* Koden bør kunne håndtere funksjonalitet:
  * Forskjellige status codes
  * Forskjellige HTTP headere
  * Forskjellige HTTP bodies





