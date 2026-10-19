---
name: scienza
description: Carica categorie della libreria scientifica di Andrea (dati, ml, comunicazione, metodo, database, infrastruttura, bio, chimica, clinica, imaging). Usa quando Andrea sceglie categorie dal menu di inizio sessione, scrive "carica <categoria>" o "/scienza", o chiede un lavoro scientifico o di analisi dati.
---

# Libreria scienza

La libreria sta due cartelle sopra questa skill: `<Base directory>/../../`.
- Indici: `../../categorie/<categoria>.md`
- Skill: `../../library/<nome>/` (contiene `SKILL.md`, a volte `scripts/` e `references/`)

## Caricare categorie

1. Per ogni categoria scelta, leggi `../../categorie/<categoria>.md`. Contiene l'elenco delle skill con una riga di descrizione.
2. Conferma ad Andrea in una riga quali categorie sono attive e quante skill contengono.
3. Le categorie restano attive per tutta la sessione. Andrea può aggiungerne altre con "carica <categoria>".
4. Se Andrea scrive "niente", non caricare nulla. La skill resta disponibile se la richiede dopo.

Numeri del menu: 1 dati, 2 ml, 3 comunicazione, 4 metodo, 5 database, 6 infrastruttura, 7 bio, 8 chimica, 9 clinica, 10 imaging.

## Usare una skill

1. Quando un compito corrisponde a una skill di una categoria attiva, leggi `../../library/<nome>/SKILL.md` per intero prima di lavorare.
2. Seguila come una skill normale. I percorsi relativi nel suo testo (per esempio `scripts/x.py`, `references/y.md`) partono da `../../library/<nome>/`. Usa percorsi assoluti quando lanci script.
3. Leggi i file di `references/` solo quando la skill lo chiede.
4. Una skill di una categoria non attiva serve? Proponi di caricare quella categoria, non usarla di nascosto.

## Regole

- Non installare pacchetti Python senza dirlo prima ad Andrea.
- Chiavi API: le skill funzionano senza. Se una funzione chiede una chiave opzionale (NCBI, OpenAlex, FRED, Zotero, HF), dillo e prosegui senza.
- Rimosse perché a pagamento o rischiose: parallel-web, exa-search, paperclip, rowan, modal, dnanexus, latchbio, alphagenome, genomic-intelligence, generate-image, hypogenic, arbor, autoskill, pi-agent, open-notebook, consciousness-council, dhdna-profiler, bgpt-paper-search, paperzilla, research-lookup, infographics, scientific-schematics. Se una skill rimanda a una di queste, salta quel passaggio.
