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

### Vaalikampanja-pohja

[Avaa Vaalikampanja-pohjan asennustyökalu](./airtable-vaalikampanja.html) — luo automaattisesti Airtable-tietokannan, joka sisältää 144 valmista tehtävää, tiimitaulun, 26 Uudenmaan kuntaa ja viisi kampanjavaihetta.

Tarvitset:

* Airtable-tilin (luo ilmainen tili osoitteessa [airtable.com/signup](https://airtable.com/signup), jos sellaista ei vielä ole)
* Henkilökohtaisen API-avaimen (asennustyökalu opastaa sen luomisessa)

Asennus kestää muutamia sekunteja.

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

> **Huom:** Buffer eroaa yllä olevista kolmesta — sitä ei voi liittää yhdellä napin painalluksella claude.ai:n integraatiovalikosta, vaan se on "custom connector", joka vaatii käyttäjäkohtaisen API-avaimen.

### Käyttöönotto

**1. Hae oma API-avaimesi Bufferista**

1. Kirjaudu [buffer.com](https://buffer.com)-tiliisi
2. Avaa Bufferin asetuksista API-osio ("Get API Key")
3. Kopioi avain talteen — se on **henkilökohtainen salaisuus**, älä jaa sitä eteenpäin

**2. Lisää Buffer claude.ai:hin custom connectorina**

1. [claude.ai](https://claude.ai) → **Settings** → **Connectors** → **Add custom connector**
2. Liitä palvelimen URL: `https://mcp.buffer.com/mcp`
3. Lisää bearer-tunnistus Authorization-otsakkeena: `Bearer SINUN_API_AVAIMESI`
4. Tallenna

Yksityiskohtaiset ohjeet ja vianetsintä: [Bufferin viralliset MCP-ohjeet](https://developers.buffer.com/guides/integrations/mcp.html).

---

## Vihreä MCP

Vihreiden oma MCP-palvelin — tarjoaa Clauden chatissa työkaluja Vihreiden vaalitulosten, tapahtumien ja virallisten asiakirjojen hakuun.

> **Huom:** Vihreä MCP on custom connector, joka vaatii oman `client_id`:n ja `client_secret`:n. Tunnukset jaetaan erikseen turvallista kanavaa pitkin — niitä ei voi laittaa tähän julkiseen ohjeeseen. Pyydä omat tunnukset osoitteesta [santeri.leinonen@vihreat.fi](mailto:santeri.leinonen@vihreat.fi).

### Käyttöönotto

1. Avaa [claude.ai](https://claude.ai), kirjaudu sisään (mikä tahansa Claude-tilaus käy, myös ilmainen)
2. **Settings → Connectors → Add Custom Connector**
3. Täytä:
   * Server URL: `https://vihrea-mcp.leinonensanteri.fi`
   * Client ID: *(jaetaan erikseen)*
   * Client Secret: *(jaetaan erikseen)*
4. **Connect** → claude.ai ohjaa OAuth-autentikaatioon, joka pyörii hetken
5. Vihreä Connected-merkki = käytössä

Kysy esim. *"Mitä mieltä vihreät ovat perustulosta?"*, *"Ketkä ovat vihreiden ääniharavia Helsingissä?"*, *"Mitä tapahtumia Turussa on tulossa?"*

**Tunnukset ovat jaettuja kaikkien luotettavien käyttäjien kesken — älä levitä eteenpäin.** Jos epäilet vuotoa, ota yhteyttä: [santeri.leinonen@vihreat.fi](mailto:santeri.leinonen@vihreat.fi).

---

*Päivitetty: 3.5.2026*
