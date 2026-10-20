# tool-claude — negozio plugin "benito" per Claude Code

Plugin scelti e verificati (codice, licenza, rete) prima dell'installazione.

| Plugin | Cosa fa | Origine |
|---|---|---|
| caveman | Risposte corte, livello max di default, sempre attivo | JuliusBrussee/caveman (Apache-2.0), adattato |
| menu | A inizio sessione chiede quali skill benito usare (e quali categorie scienza) | nostro |
| scienza | 115 skill scientifiche, caricate a categorie scelte dal menu | K-Dense-AI/scientific-agent-skills (MIT) |
| hallmark | Design pagine/interfacce senza "faccia da AI" | Nutlope/hallmark (MIT) |
| book-to-skill | Libro/documento → skill | virgiliojr94/book-to-skill (MIT) |
| humanizer | Toglie i tic da testo AI (versione bloccata) | blader/humanizer (MIT) |
| superpowers | Metodo: brainstorming, piano, test, debug (si aggiorna da solo) | obra/superpowers (MIT) |

## Installazione (Claude Code)

In una sessione:

```
/plugin marketplace add andrelp99-tools/tool-claude
/plugin install caveman@benito
/plugin install menu@benito
/plugin install scienza@benito
/plugin install hallmark@benito
/plugin install book-to-skill@benito
/plugin install humanizer@benito
/plugin install superpowers@benito
```

Aggiornare: `/plugin marketplace update benito`.

## menu: come funziona

- A inizio sessione (avvio o `/clear`) un hook chiede, prima di tutto, quali skill usare: superpowers, hallmark, humanizer, book-to-skill, e quali categorie scienza caricare.
- Nell'app desktop arriva come finestra di domande a scelta multipla; sul web o sul telefono come menu di testo numerato.
- "niente" salta. Le skill non scelte restano disponibili se le chiedi dopo.

## scienza: come funziona

- Le 115 skill stanno in `plugins/scienza/library/`, fuori dalla cartella `skills/`: Claude Code non le carica, quindi non pesano.
- Le categorie si scelgono dal menu del plugin `menu`: dati, ml, comunicazione, metodo, database, infrastruttura, bio, chimica, clinica, imaging.
- Scegli categorie → la skill `scienza` legge l'indice `categorie/<nome>.md` e usa le skill di quelle categorie per tutta la sessione.
- "carica <categoria>" aggiunge una categoria a metà sessione. "niente" salta.

Note tecniche: BENITO.md.
