# Vihreä tekoäly -työpaja

Tervetuloa! Tämä sivu kokoaa työpajassa käytettävien MCP-palvelimien (Model Context Protocol) käyttöönotto-ohjeet ja aloitusmallit.

## Tilaa päivitykset

Tämän sivun ohjeita ja työkaluja päivitetään ajoittain. Jos haluat sähköpostiisi tiedon muutoksista, [liity sähköpostilistalle tällä lomakkeella](https://forms.gle/oyfNjtdVXftrghAS8).

---

## Mikä MCP on?

MCP (Model Context Protocol) on tapa antaa Claudelle pääsy ulkoisiin palveluihin — Notioniin, Airtableen, Canvaan ja muihin. Liität palvelun kerran, ja sen jälkeen voit pyytää Claudea tekemään asioita siellä keskustelun kautta.

---

## Notion MCP

**Mitä voit tehdä:** luoda ja muokata sivuja, päivittää tietokantoja, hakea sisältöä omasta työtilastasi keskustelun kautta.

### Käyttöönotto

1. Mene osoitteeseen [claude.ai](https://claude.ai) ja kirjaudu sisään
2. Klikkaa profiilikuvaketta (oikea yläkulma) → **Settings**
3. Vasemmasta sivupalkista valitse **Connectors** (joissain tileissä **Integrations**)
4. Etsi listasta **Notion** → **Connect**
5. Sinut ohjataan Notioniin kirjautumaan ja antamaan luvat
6. Valmis — voit nyt pyytää Claudea Notion-toimintoihin

### Aloitusmalli

Kopioi tämä Notion-malli omaan työtilaasi pohjaksi:

[Notion-malli (avaa ja klikkaa "Duplicate")](https://momentous-twill-0ac.notion.site/3505ff90ebd680bfb6c1e4df6bebc08c?v=3505ff90ebd6813e92bc000c050c0c66&source=copy_link)

---

## Airtable MCP

**Mitä voit tehdä:** hallinnoida Airtable-pohjia — rivien lisäys, päivitys, haku ja näkymien muokkaus — keskustelun kautta.

### Käyttöönotto

1. [claude.ai](https://claude.ai) → **Settings** → **Connectors**
2. Etsi **Airtable** → **Connect**
3. Kirjaudu Airtableen ja valitse, mihin pohjiin annat pääsyn

### Aloitusmalli

<!-- TODO: Santeri täydentää — Airtable-mallin linkki tai upotettava HTML, joka tarjoaa "kopioi malli" -toiminnon -->

*Lisätään pian.*

---

## Canva MCP

**Mitä voit tehdä:** generoida ja muokata Canva-designeja, viedä tiedostoja, kommentoida — kaikki keskustelun kautta.

### Käyttöönotto

1. [claude.ai](https://claude.ai) → **Settings** → **Connectors**
2. Etsi **Canva** → **Connect**
3. Kirjaudu Canvaan ja anna pyydetyt luvat

---

## Buffer MCP

**Mitä voit tehdä:** aikatauluttaa sosiaalisen median julkaisuja Bufferin kautta keskustelusta käsin.

### Käyttöönotto

1. [claude.ai](https://claude.ai) → **Settings** → **Connectors**
2. Etsi **Buffer** → **Connect**
3. Kirjaudu Bufferiin ja yhdistä haluamasi kanavat

---

## Vihreä MCP

Vihreiden oma MCP-palvelin — räätälöityjä työkaluja Vihreiden työkäyttöön.

### Käyttöönotto

<!-- TODO: Santeri täydentää — palvelimen URL -->
<!-- HUOM TURVALLISUUS: tähän julkiseen tiedostoon EI saa liittää salaisia bearer-tokeneita tai OAuth client secret -arvoja. Jos OAuth-flow on käytössä (kuten yleensä), käyttäjille riittää URL — he saavat oman tokeninsa kirjautuessaan. -->

1. [claude.ai](https://claude.ai) → **Settings** → **Connectors** → **Add custom connector**
2. Liitä palvelimen URL: *(lisätään pian)*
3. Hyväksy OAuth-kirjautuminen — jokainen käyttäjä saa oman tokeninsa

---

*Päivitetty: 28.4.2026*
