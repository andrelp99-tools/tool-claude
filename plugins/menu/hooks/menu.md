Preferenza di Andrea: la prima cosa di ogni nuova sessione è il menu delle skill benito, prima di qualunque altra domanda o lavoro, anche se il primo messaggio di Andrea è già una richiesta.

Con lo strumento AskUserQuestion (se c'è) fai due domande nella stessa chiamata, entrambe a scelta multipla:

1. "Quali skill benito uso in questa sessione?" (header "Skill"). Opzioni:
   - superpowers: metodo (brainstorming, piano, TDD, debug, review)
   - hallmark: design di pagine e interfacce senza faccia da AI
   - humanizer: toglie i tic da AI dai testi
   - book-to-skill: da libro o documento a skill
2. "Carico categorie della libreria scienza?" (header "Scienza"). Opzioni:
   - Dati e ML: 1 dati, 2 ml
   - Scrittura e metodo: 3 comunicazione, 4 metodo
   - Database e infrastruttura: 5 database, 6 infrastruttura
   - Scienze della vita: 7 bio, 8 chimica, 9 clinica, 10 imaging
   Nella descrizione ricorda che con "Altro" Andrea può scrivere numeri singoli (es. "4, 6") o "niente".

Senza AskUserQuestion (app web o telefono) mostra il menu come testo, due righe:
- Skill: 1 superpowers, 2 hallmark, 3 humanizer, 4 book-to-skill, niente
- Scienza: 1 dati, 2 ml, 3 comunicazione, 4 metodo, 5 database, 6 infrastruttura, 7 bio, 8 chimica, 9 clinica, 10 imaging, niente

Dopo la risposta:
- Conferma in una riga cosa è attivo.
- Skill scelte: per tutta la sessione invocale con lo strumento Skill quando il lavoro le tocca (superpowers:using-superpowers e le sue skill di processo, hallmark:hallmark, humanizer:humanizer, book-to-skill:book-to-skill). Le skill non scelte restano disponibili se Andrea le chiede.
- Categorie scienza scelte: invoca la skill scienza:scienza e segui le sue istruzioni per caricarle.
- "niente" o nessuna scelta: non caricare nulla e passa alla richiesta di Andrea.
