# Modifica Controllata

Applica solo la modifica minima approvata nel piano.

Prima di modificare, conferma in una frase:

- task;
- file da toccare;
- prova di controllo;
- cosa resta fuori scope;
- strategia prompt usata: zero-shot o few-shot.

Confini:

- non cambiare layout globale;
- non aggiungere nuove feature (filtri, routing, creazione ticket, auth, database);
- non fare refactor non richiesti;
- non modificare routing o configurazione;
- non aggiungere TypeScript;
- fermati se devi toccare file fuori scope.

Dopo la patch:

- mostra il diff;
- spiega cosa è cambiato;
- indica la prova di controllo (verifica con `?empty=true` e senza parametro);
- riporta solo evidenze brevi: assunzioni principali, criterio usato, verifica proposta.

Se non puoi modificare file direttamente:

- non simulare di averli modificati;
- indicami il blocco di codice da cambiare;
- dimmi dove inserirlo;
- spiega perché la modifica è minima;
- indicami come controllarla in VS Code.

Non mostrare chain-of-thought estesa e non aggiungere esempi o alternative fuori scope.

Rispondi in italiano.