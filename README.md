# web

## Gestione mod e link download (solo admin, dal sito)

Gli admin possono ora aggiungere nuove mod **direttamente dal sito** tramite un form dedicato.

### Come fare login admin

Nella navbar trovi il pulsante **Admin Login**.

Credenziali richieste:

- `username: tigercecco`
- `password: tigercecco`

Dopo login corretto il sito imposta automaticamente `modhub_role = "admin"` in `localStorage` e ricarica la pagina.

### Cosa può fare l'admin nel sito

- inserire nome, categoria, descrizione e metadati della mod;
- impostare il link download (`downloadUrl`);
- caricare un file locale dal form (viene creato automaticamente un link download);
- impostare il testo del bottone download (`downloadLabel`).

Le mod aggiunte dall'admin vengono salvate in `localStorage` (chiave `modhub_custom_mods`) e mostrate nella lista.

## Note importanti

- La protezione admin è lato client.
- Per sicurezza reale, devi validare permessi e upload lato server/back-end.
