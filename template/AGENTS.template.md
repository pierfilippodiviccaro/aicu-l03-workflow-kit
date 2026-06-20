# AGENTS.md

## Contesto Del Progetto
App ticketing minimale: API Express che espone ticket fittizi, UI React/Vite che mostra la lista.
Stack: Node.js, Express, React, Vite, JavaScript/JSX. Niente TypeScript.
Il task del lab è aggiungere un empty state quando la lista è vuota.

## Obiettivo Corrente
Quando l'API restituisce una lista vuota, mostrare un messaggio chiaro e sobrio al posto dello spazio vuoto.

## Ambito Delle Istruzioni
Queste istruzioni valgono per questa repo. Non portare task temporanei qui.
- Regole stabili → questo file.
- Prompt riusabili → `prompt-kit/`.
- Task del momento → nel prompt o nel ticket, non qui.

## Regole Di Lavoro
- Prima di modificare file, riscrivi il task in una frase.
- Prima di modificare file, proponi un piano breve (max 5 punti operativi).
- Se la richiesta è ambigua, fai una sola domanda prima di procedere.
- Se il task diventa troppo largo, fermati e proponi una versione ridotta.
- Non simulare modifiche non eseguite.
- Non mostrare chain-of-thought estesa: riporta solo assunzioni principali, criterio usato e verifica proposta.
- Usa esempi few-shot solo se chiariscono formato o criterio; non usarli per anticipare la soluzione.
- Rispondi in italiano.

## Confini
- Non cambiare layout globale.
- Non aggiungere feature non richieste (filtri, routing, creazione ticket, auth, database).
- Non modificare routing o configurazione.
- Non fare refactor non richiesti.
- Non toccare file fuori dallo scope del task.
- Non aggiungere TypeScript.

## Comandi Utili
- install: `pnpm install`
- dev: `pnpm dev`
- build: `pnpm run build`
- start (serve build): `pnpm start`

## Stati Da Verificare
- Stato con ticket: http://127.0.0.1:5173/
- Stato vuoto: http://127.0.0.1:5173/?empty=true
- API diretta: http://127.0.0.1:3001/api/tickets
- API vuota: http://127.0.0.1:3001/api/tickets?empty=true

## Prova Di Controllo
Per ogni modifica indica:
- come verificare il caso modificato (empty state visibile con `?empty=true`);
- come verificare che il caso normale funzioni ancora (lista ticket visibile senza parametro);
- quali controlli non sono stati eseguiti;
- assunzioni principali e criterio usato.

## Output Finale
Alla fine di ogni modifica rispondi con:
- file modificati;
- cosa è cambiato;
- prova di controllo eseguita o da eseguire;
- strategia prompt usata: zero-shot o few-shot;
- rischi o dubbi rimasti.