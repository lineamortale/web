# web

## Nuova struttura richiesta

- In home page vengono mostrate solo **2 mod scelte**:
  - OptiFabric Ultra
  - Sodium Extended
- Esiste una nuova pagina `mods.html` con grafica uguale alla home (font, colori e stile) dove vedere **tutte le mod**.
- La categoria è filtrabile tramite un menu con tutti i tipi di categoria disponibili.

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

- navbar: pagina mod / features / Discord;
- hero CTA: porta a `/mods.html`;
- explore CTA: porta a `/mods.html`;
- footer link: privacy/terms/contact con URL reali.

## Nota sicurezza

Questa è una soluzione client-side (demo/prototipo).
Per un sito reale servono autenticazione, autorizzazioni e upload gestiti lato server.
