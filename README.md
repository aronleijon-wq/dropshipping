# SleepWell (tidigare VAKN) – Shopify-tema (Horizon)

Domän: https://sleep-well.se (primär, DNS hos Simply.com). Live-tema: "SleepWell".

Temat i repot motsvarar:
- Live och utkast växlar: det tema som är opublicerat får nya ändringar och publiceras sedan.
- Live (2026-10-14): "SleepWell – video" (id 209715069258). Nytt utkast med ny startsida (vk-hero) och SLUTSÅLD-etikett:
  "SleepWell – ny startsida" (id 209762189642), kopierat från live 2026-10-14. Äldre teman är inte i synk.
- Pris: 499 kr/st från 25 okt 2026 (399 kr 23–25 okt, 449 kr kort 25 okt). Black Week-pris 349 kr tidigast 26 nov (−30 %). Automatiska rabatter: 2 st −20 % (798,40 kr), 3 st −30 % (1 047,90 kr). Inköp ca $20 (≈210 kr) per st.
- Läslampa: 249 kr 28 okt (ca 1 h), 349 kr från 28 okt 2026. Black Week-pris 229 kr tidigast 28 nov. Inköp 38,84 kr + frakt 18,68 kr (under 100 kr) + import ca 69 kr.
  Kontrollera med Admin API (themes { role }) vilket som är MAIN innan uppladdning.

VAKN-specifikt:
- `templates/index.json` – startsida
- `templates/product.json` – produktsida
- `snippets/vakn-bundle.liquid` – mängdrabattrutor 1/2/3 st (synkar med Horizons antalsväljare)
- `snippets/vakn-eta.liquid` – beräknat leveransdatum
- `sections/header-group.json` – annonsbanner
- `config/settings_data.json` – färger/typsnitt

Live-temat kan inte skrivas via API. Ändringar laddas upp till det opublicerade temat,
förhandsgranskas och publiceras manuellt i admin. Efter publicering: duplicera live-temat
till ett nytt utkast innan nästa ändring.

Med Shopify CLI (kräver nätverksåtkomst till *.myshopify.com):

    shopify theme push --store ngzyak-sk.myshopify.com --theme <opublicerat-id>

## Produktfakta (styr all copy)

- Larmet **vibrerar och är tyst** – inget ljud (bekräftat av butiksägaren 2026-10-13).
- Funktioner enligt leverantörens bild ("9 major functions"): tid/datum, stegräknare, tyst larm, sömnmätning, stoppur, distans (km), kalorier, byte av stegräkningsläge, minne för träningsdata.
- 3 bar (stänk, regn, handtvätt – inte bad/dusch/simning). Uppladdningsbar. Plast, dolt spänne. 6 färger.
- Rabatter: 2 st −20 %, 3 st −30 % (automatiska). Inga andra rabatter/jämförpriser.
