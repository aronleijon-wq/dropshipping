# VAKN – Shopify-tema (Horizon)

Hela live-temat "VAKN – mängdrabatt" (id 209490968906), hämtat via Admin API.

VAKN-specifikt:
- `templates/index.json` – startsida
- `templates/product.json` – produktsida
- `snippets/vakn-bundle.liquid` – mängdrabattrutor 1/2/3 st (synkar med Horizons antalsväljare)
- `snippets/vakn-eta.liquid` – beräknat leveransdatum
- `sections/header-group.json` – annonsbanner
- `config/settings_data.json` – färger/typsnitt

Live-temat kan inte skrivas via API. Ändringar pushas till ett opublicerat tema,
förhandsgranskas och publiceras manuellt i admin.

Med Shopify CLI (kräver nätverksåtkomst till *.myshopify.com):

    shopify theme push --store ngzyak-sk.myshopify.com --theme <opublicerat-id>

## Produktfakta (styr all copy)

- Larmet **vibrerar och är tyst** – inget ljud (bekräftat av butiksägaren 2026-10-13).
- Ingen stegräknare. 3 bar (stänk, regn, handtvätt – inte bad/dusch/simning). Uppladdningsbar. Plast, dolt spänne. 6 färger.
- Rabatter: 2 st −20 %, 3 st −30 % (automatiska). Inga andra rabatter/jämförpriser.
