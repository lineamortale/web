# web

## Gestione mod e link download (solo admin)

Le modifiche a elenco mod e link download sono abilitate **solo per utenti admin**.

Nel frontend, il file `mods.json` viene caricato solo se è presente:

- `localStorage.modhub_role = "admin"`

Se il ruolo non è `admin`, il sito usa automaticamente la lista mod di fallback incorporata nel bundle.

### Dati supportati in `mods.json`

- `id`
- `name`
- `category`
- `description`
- `version`
- `mcVersion`
- `downloads`
- `image`
- `color`
- `downloadUrl`
- `downloadLabel` (opzionale)

> Nota: questa è una protezione lato client. Per sicurezza reale, valida i permessi lato server.
