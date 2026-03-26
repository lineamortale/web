# web

## Admin completo nel sito

Gli admin ora hanno controllo completo dal frontend:

- aggiunta nuove mod;
- modifica mod esistenti;
- eliminazione mod esistenti;
- gestione link download e label;
- caricamento file locale per generare link download.

## Login admin

Usa il pulsante **Admin Login** nella navbar.

Credenziali:

- `username: tigercecco`
- `password: tigercecco`

Dopo login corretto il sito salva `modhub_role = "admin"` in `localStorage`.

## Persistenza dati admin

Le modifiche admin vengono salvate in `localStorage` con chiave `modhub_custom_mods`.

## Pulsanti e link

I pulsanti/link principali ora portano sempre da qualche parte:

- navbar: `#mods`, `#features`, Discord;
- hero CTA: porta a `#mods`;
- explore CTA: porta a `#mods`;
- footer link: privacy/terms/contact con URL reali.

## Nota sicurezza

Questa è una soluzione client-side (demo/prototipo).
Per un sito reale servono autenticazione, autorizzazioni e upload gestiti lato server.
