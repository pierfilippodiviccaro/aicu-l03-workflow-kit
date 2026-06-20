# Consegna - Lezione 03

## Obiettivo

Preparare un workflow kit riusabile con `AGENTS.template.md`, `prompt-kit/` e `handoff-note.template.md`, in modo da adattarlo subito nel lab L04.

Durante L03 non modifichi la repo di codice; nel lab subito dopo si'.

## Repository Di Lavoro

Lavora nel tuo fork della repo:

```txt
aicu-l03-workflow-kit
```

Questa repo non e' la repo di codice del lab. E' il tuo punto di partenza per un metodo di lavoro riusabile.

## Setup Minimo

Preferenza:

1. fai fork della repo `aicu-l03-workflow-kit`;
2. clona il tuo fork;
3. apri la repo in VS Code o editor equivalente.

Comando:

```bash
git clone <url-del-tuo-fork>
```

Se GitHub o Git ti bloccano, usa il fallback indicato dal docente. L'obiettivo resta preparare una traccia controllabile, non risolvere setup.

## File Da Preparare

Lavora sui file della repo kit:

```txt
AGENTS.template.md
prompt-kit/
  01-orientamento.md
  02-piano-breve.md
  03-modifica-controllata.md
  04-controllo-diff.md
  05-handoff.md
handoff-note.template.md
```

## Cosa Va Dove

| Superficie | Uso |
| --- | --- |
| prompt del momento | task specifico che stai chiedendo ora |
| `prompt-kit/` | procedure riusabili per orientamento, piano, modifica, diff e handoff |
| `AGENTS.template.md` | regole riusabili in molte repo, ancora con placeholder |
| `AGENTS.md` nella repo target | regole specifiche di quella repo, dopo averla letta |
| `handoff-note.template.md` | struttura di chiusura per rendere reviewabile il lavoro |

Non mettere task temporanei in `AGENTS.template.md`: rischi di portarli dentro lavori successivi.

Non creare `AGENTS.md` nella repo kit solo per riempire un file: in L04 lo creerai nella repo di codice, dopo averla letta.

Non mettere esempi few-shot nel kit se non servono: bastano 1-2 esempi brevi quando chiariscono formato o criterio. Non chiedere all'AI di mostrare chain-of-thought estesa; chiedi assunzioni, criterio e verifica proposta.

## Personalizzazione Obbligatoria

Personalizza almeno:

- `AGENTS.template.md`;
- `prompt-kit/02-piano-breve.md`;
- `prompt-kit/03-modifica-controllata.md`.

Gli altri prompt sono gia' utilizzabili, ma puoi adattarli al tuo modo di lavorare, al tool che usi e al livello di controllo che vuoi mantenere.

Nei prompt personalizzati fai comparire:

- strategia prompt: zero-shot oppure few-shot;
- eventuali esempi few-shot brevi e non risolutivi;
- evidenze richieste: assunzioni principali, criterio usato, verifica proposta.

## Lingua

Per il Modulo 1 puoi scrivere `AGENTS.template.md` e prompt-kit in italiano.

Nota professionale: in molti contesti di lavoro conviene scrivere istruzioni e prompt in inglese, soprattutto in team internazionali o con strumenti addestrati/documentati principalmente in inglese. Qui usiamo italiano per ridurre attrito.

## Dry-Run Senza Patch

Usa `prompt-kit/02-piano-breve.md` sul task:

```txt
Quando non ci sono ticket aperti, mostra un messaggio chiaro.
```

Non autorizzare modifiche.

Il piano deve essere una bozza in massimo 5 punti operativi. Il limite riguarda la bozza visibile, non il numero di round con l'agente: puoi rivederla finche' e' approvabile. I 5 punti sono decisioni o azioni verificabili, non 5 comandi ne' 5 requisiti separati.

Output atteso:

- file o aree probabili;
- modifica minima;
- cosa non toccare;
- verifica proposta;
- strategia prompt zero-shot/few-shot;
- evidenze brevi da chiedere prima della patch;
- eventuali dubbi.

## Vincoli

- Non iniziare la patch L04.
- Non aprire PR.
- Non fare redesign.
- Non aggiungere filtri, routing o nuove feature.
- Non rendere il kit specifico della ticketing app: l'adattamento concreto arriva in L04.
- Non usare esempi few-shot per anticipare la soluzione L04.
- Non chiedere chain-of-thought estesa: chiedi solo evidenze sintetiche e verificabili.
- Non inserire credenziali, token, file `.env`, dati personali, codice aziendale o log sensibili.

## Pronto Quando

- Hai fork o fallback.
- Hai `AGENTS.template.md`.
- Hai `prompt-kit/`.
- Hai `handoff-note.template.md`.
- Hai personalizzato almeno `02-piano-breve.md` e `03-modifica-controllata.md`.
- Hai fatto un dry-run senza patch.
- Hai deciso quando usare zero-shot e quando aggiungere pochi esempi few-shot.
- Sai quali file copierai/adatterai in L04.
- Hai committato e pushato il kit nel tuo fork.

> **Team Mode**
> In un team, `AGENTS.template.md`, prompt-kit e handoff template aiutano a rendere ripetibile il modo in cui chiedi piano, modifica, diff e handoff. Non sostituiscono il tuo giudizio: lo rendono piu' facile da esercitare.
