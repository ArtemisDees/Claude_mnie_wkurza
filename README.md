# Strona CHUD-POL Garage

Statyczna strona serwowana z Cloudflare Workers (projekt `aged-sun-ecb2`).

- `public/` – cała strona: `index.html` i folder `assets/` (czcionki, logo, animacja). Nic nie jest pobierane z zewnątrz.
- `wrangler.jsonc` – konfiguracja wdrożenia. Pole `name` musi odpowiadać nazwie projektu w Cloudflare.

Każdy commit na gałęzi `main` jest publikowany automatycznie po połączeniu repozytorium w Cloudflare
(projekt → Settings → Builds → Connect). Polecenie wdrożenia: `npx wrangler deploy` (domyślne), bez polecenia budowania.

Dane firmy (nazwa, adres, telefony, cennik) podmienia się w `public/index.html`; lista miejsc jest w komentarzu na początku pliku.
