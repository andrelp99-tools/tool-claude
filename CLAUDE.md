# tool-claude (negozio plugin "benito")

Marketplace personale di plugin Claude Code. Andrea usa Claude Code dall'app desktop su Windows e nell'app Claude (web/telefono).
- Plugin: caveman (max default, promemoria a ogni avvio), menu (hook a inizio sessione: chiede quali skill benito usare e quali categorie scienza), scienza (115 skill K-Dense in `plugins/scienza/library/`, caricate a categorie dal menu), hallmark, book-to-skill, humanizer (github, bloccato a sha), superpowers (github, aggiornamenti automatici). Dettagli: **README.md** e **BENITO.md**.
- Le skill della libreria scienza stanno fuori da `skills/` apposta: non vanno caricate tutte (peso ~28k token). Non spostarle.
- Prima di aggiungere un plugin: analizza repo (codice, script, rete, licenza), poi `claude plugin validate .` e su ogni plugin.
- Plugin scartati e perché: BENITO.md e progetto "Implementazioni app da Github".
- Modifica a un plugin → alza `version` nel suo `plugin.json`; Andrea aggiorna con `/plugin marketplace update benito`.

## Regole di lavoro di Andrea
- Rispondi in italiano, stile **caveman max** (risposte corte, solo sostanza). Plugin `caveman@benito` se installato.
- Prima di agire fai domande per capire contesto, richieste, scopi. Proponi idee sensate quando servono.
- Lavora sempre inline: **mai sub-agenti** (vale anche per le skill di superpowers che li usano).
- Modifiche grafiche, anteprime di come verrebbe una funzione o lunghe serie di domande con esempi: mostrale in una pagina HTML/mockup invece che a testo.
- Ogni libreria o repo esterna nuova: prima controlla codice, licenza, sicurezza, permessi; poi proponi.
- Commit firmati `Claude <noreply@anthropic.com>`, **mai con l'email personale**: il profilo GitHub personale (andrelp99) è collegato a LinkedIn e il lavoro dell'org non deve comparire lì.
- PC Windows di casa, spesso spento, niente Docker/WSL. Andrea non ama la riga di comando: comandi pronti da incollare, spiegati in breve.
- A fine lavoro aggiorna **BENITO.md** (note tecniche) e la sezione "In sospeso".
- Contesto completo (scelte, storico, altre app): progetto "Implementazioni app da Github" nell'app Claude.
