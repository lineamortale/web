# web

## Requested structure

- The home page shows only **2 selected mods**:
  - OptiFabric Ultra
  - Sodium Extended
- There is a dedicated `mods.html` page with the same visual style as home (font, colors, and UI style) that shows **all mods**.
- Categories are filterable through a menu containing all available category types.
- Categories are rendered as a premium dark-purple left sidebar with badges, active/hover states, and built-in Filters (Game Version + Mod Loader).

## Full admin access in the site

Admins now have full frontend control:

- create new mods;
- edit existing mods;
- delete existing mods;
- manage download links and button labels;
- upload a local file to generate a download link.

## Admin login

Use the **Admin Login** button in the navbar.

Credentials:

- `username: tigercecco`
- `password: tigercecco`

After successful login, the site stores `modhub_role = "admin"` in `localStorage`.

## Admin data persistence

Admin changes are saved in `localStorage` under the key `modhub_custom_mods`.

## Buttons and links

Main buttons/links now always go somewhere:

- navbar: mods page / features / Discord;
- hero CTA: goes to `/mods.html`;
- explore CTA: goes to `/mods.html`;
- footer links: privacy/terms/contact with real URLs.

## Security note

This is a client-side demo/prototype.
For a real production website, authentication, authorization, and uploads must be handled server-side.
