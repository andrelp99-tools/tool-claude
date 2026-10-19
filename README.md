# tool-claude — negozio plugin "benito" per Claude Code

Plugin scelti e verificati (codice, licenza, rete) prima dell'installazione.

| Plugin | Cosa fa | Origine |
|---|---|---|
| caveman | Risposte corte, livello max di default, sempre attivo | JuliusBrussee/caveman (Apache-2.0), adattato |
| scienza | 115 skill scientifiche, caricate a categorie da menu a inizio sessione | K-Dense-AI/scientific-agent-skills (MIT) |
| hallmark | Design pagine/interfacce senza "faccia da AI" | Nutlope/hallmark (MIT) |
| book-to-skill | Libro/documento → skill | virgiliojr94/book-to-skill (MIT) |
| humanizer | Toglie i tic da testo AI (versione bloccata) | blader/humanizer (MIT) |
| superpowers | Metodo: brainstorming, piano, test, debug (si aggiorna da solo) | obra/superpowers (MIT) |

## Installazione (Claude Code)

In una sessione:

```
/plugin marketplace add andrelp99-tools/tool-claude
/plugin install caveman@benito
/plugin install scienza@benito
/plugin install hallmark@benito
/plugin install book-to-skill@benito
/plugin install humanizer@benito
/plugin install superpowers@benito
```

Aggiornare: `/plugin marketplace update benito`.

## scienza: come funziona

- Le 115 skill stanno in `plugins/scienza/library/`, fuori dalla cartella `skills/`: Claude Code non le carica, quindi non pesano.
- A inizio sessione un hook mostra il menu: dati, ml, comunicazione, metodo, database, infrastruttura, bio, chimica, clinica, imaging.
- Scegli categorie → la skill `scienza` legge l'indice `categorie/<nome>.md` e usa le skill di quelle categorie per tutta la sessione.
- "carica <categoria>" aggiunge una categoria a metà sessione. "niente" salta.

Note tecniche: BENITO.md.
