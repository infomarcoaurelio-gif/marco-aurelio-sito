BOTTEGA MARCOAURELIO — REGISTRO REVISIONE 011
Data: 05 novembre 2026
Oggetto: il sito deve stare interamente nella larghezza dello smartphone,
mantenendo i caratteri grandi già approvati.

PROBLEMA RISCONTRATO
Dopo l'ingrandimento generalizzato dei font, Chrome su Redmi mostrava la
pagina leggermente più larga del viewport. L'utente era costretto a
ridurre lo zoom con un gesto di pinch per vedere il margine destro.
L'intestazione Bottega MarcoAurelio / Orafo / ENG evidenziava lo sforamento.

INTERVENTI IT + EN
- Aggiunto il foglio di stile ma3-viewport-fit in index.html e en.html.
- Limitata la larghezza di pagina e contenitori al 100% del viewport
  (non 100vw: la misura include spesso la barra di scorrimento).
- Intestazione mobile con due colonne: titolo flessibile e comando
  IT/ENG a larghezza contenuta; parole/titoli possono andare a capo.
- Anche il titolo inglese ha adesso gli elementi separati in un
  ab-brand-mainline, come l'italiano.
- I contenuti di schede, griglie e FAQ possono restringersi e andare
  a capo evitando di allargare la pagina.
- Disattivato soltanto lo scorrimento orizzontale come salvaguardia.
- NESSUNA riduzione del corpo dei caratteri: leggibilità invariata.

CONTROLLO
Confermato l'aggiornamento dei file index.html ed en.html via GitHub;
resta utile la verifica visiva dal Redmi dopo il refresh del browser.
