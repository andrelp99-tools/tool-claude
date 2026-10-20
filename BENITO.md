# Note tecniche tool-claude

Creata 19/10/2026.

## Versioni verificate
- caveman: JuliusBrussee/caveman @ bad48a0 — skills/caveman + skills/ultracave unite, max default, tolti riferimenti hook/status. Hook SessionStart: ricorda caveman max.
- scienza: K-Dense-AI/scientific-agent-skills @ 593377bb — 115/177 skill, file invariati. Aggiunti: skill router, indici categorie. Dalla 1.1.0 il menu categorie sta nel plugin menu.
- menu (nostro, 20/10/2026): hook SessionStart `startup|clear` che stampa `hooks/menu.md`. Claude fa come prima cosa due domande (skill benito, categorie scienza) con AskUserQuestion, o menu testo se manca. AskUserQuestion ha max 4 opzioni: categorie scienza raggruppate a coppie, numeri singoli via "Altro".
- hallmark: Nutlope/hallmark @ 13ac0ec — solo skills/hallmark.
- book-to-skill: virgiliojr94/book-to-skill @ a24e62f — patch: variabile BOOK_TO_SKILL_PLUGIN_DIR in testa alla lista percorsi di extract.py.
- humanizer: sorgente github bloccata a 8c307f36.
- superpowers: sorgente github non bloccata (aggiornamenti automatici, scelta di Andrea).

## Skill scientifiche escluse (22)
A pagamento / chiave obbligatoria / account: parallel-web, exa-search, paperclip, rowan, modal, dnanexus-integration, latchbio-integration, alphagenome, genomic-intelligence, generate-image, bgpt-paper-search, paperzilla, research-lookup, infographics, scientific-schematics.
API a consumo: hypogenic, arbor. Rischio/inutili: autoskill (registra schermo), pi-agent, open-notebook (self-hosting), consciousness-council, dhdna-profiler.
Aree escluse: ingegneria, fisica/materiali, proteomica, multi-omica, proteine, neuroscienze, automazione lab, ISO, preclinica, oceanografia.

## Controlli fatti
- `claude plugin validate`: ok su marketplace e plugin.
- Script: nessun pattern pericoloso (curl|sh, exec di codice remoto, rm -rf home). Domini contattati: solo servizi scientifici pubblici (NCBI, EBI, arXiv, OpenAlex, Crossref, KEGG, DepMap…); openrouter.ai solo con chiave opzionale.
- Nessun binario nel pacchetto.

## Aggiornare la libreria
Riclonare upstream, ricopiare le 115 cartelle elencate in `plugins/scienza/categorie/*.md`, ricontrollare, alzare `version` in plugin.json.

## In sospeso
- Andrea: `/plugin marketplace update benito`, poi `/plugin install menu@benito`. Senza il plugin menu non compare più nessun menu (scienza 1.1.0 non ha più il suo hook).
