# AGENTS.template.md

## Contesto Del Progetto

[Descrivi qui la repo target quando copierai questo template.]

## Obiettivo Corrente

[Scrivi qui il task su cui stai lavorando]

## Ambito Delle Istruzioni

Queste istruzioni valgono per la repo target dopo adattamento.

- Regole stabili: diventano `AGENTS.md` nella repo target.
- Prompt riusabili: restano in `prompt-kit/`.
- Task del momento: va scritto nel prompt o nel ticket, non reso permanente qui.

## Regole Di Lavoro

- Prima di modificare file, riscrivi il task in una frase.
- Prima di modificare file, proponi un piano breve.
- Se la richiesta e' ambigua, fai una sola domanda.
- Se il task diventa troppo largo, fermati e proponi una versione piu' piccola.
- Non simulare modifiche non eseguite.
- Non mostrare chain-of-thought estesa: riporta solo assunzioni principali, criterio usato e verifica proposta.
- Usa esempi few-shot solo se chiariscono formato o criterio; non usarli per anticipare la soluzione.

## Confini

Durante il lavoro:

- non cambiare layout globale;
- non aggiungere nuove feature non richieste;
- non modificare routing o configurazione;
- non fare refactor non richiesti;
- non cambiare file fuori dallo scope del task.

## Comandi Utili

Compila solo se li conosci o se sono nel README della repo target.

- install:
- dev:
- test:
- lint:

## Prova Di Controllo

Per ogni modifica, indica:

- come controllare il caso modificato;
- come controllare che il caso normale funzioni ancora;
- quali controlli non sono stati eseguiti.
- quali assunzioni principali e quale criterio hanno guidato la scelta.

## Output Finale

Alla fine rispondi con:

- file modificati;
- cosa e' cambiato;
- prova di controllo eseguita o da eseguire;
- strategia prompt usata se rilevante: zero-shot o few-shot;
- rischi o dubbi rimasti.
