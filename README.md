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
