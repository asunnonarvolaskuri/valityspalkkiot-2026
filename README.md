# Välityspalkkiot Suomessa 2026

Kiinteistönvälittäjien julkiset hinnastot 15 kaupungissa ja se, paljonko palkkio on euroina samasta
55 neliön kerrostalokaksiosta. Data on tutkimuksesta
[Välityspalkkiot Suomessa 2026](https://asunnonarvolaskuri.com/tutkimus/valityspalkkiot-2026/),
jossa on myös kaavio ja taulukko.

*English summary below.*

## Mitä data sisältää

- 130 hinnastoriviä 43 välittäjältä, luettu välittäjien omilta sivuilta 7.–8.10.2026.
- Palkkio on hinnastoissa 0,95–5,02 % kauppahinnasta arvonlisäveroineen, ja vähimmäispalkkio on 2 500–7 000 €.
- 15 kaupunkia: Oulu, Turku, Helsinki, Tampere, Jyväskylä, Lappeenranta, Kuopio, Lahti, Espoo, Vantaa, Pori,
  Hämeenlinna, Joensuu, Rovaniemi ja Seinäjoki.

## Tiedostot

### `valityspalkkiot-2026-kaupungit.csv`

Yksi rivi per kaupunki.

| Sarake | Selitys |
|---|---|
| `kaupunki` | Kaupunki |
| `kerrostalo_eur_m2_2025` | Vanhojen kerrostaloasuntojen keskihinta €/m² vuonna 2025 (Tilastokeskus) |
| `kaksio_55m2_keskihinnalla_eur` | 55 m² kaksion hinta keskihinnalla, pyöristetty |
| `hinnastoja` | Kuinka monta hinnastoa kaupungissa on laskettu mukaan |
| `palkkio_halvin_eur` | Halvimman hinnaston palkkio kaksiosta, € |
| `palkkio_keskimmainen_valittaja_eur` | Keskimmäisen välittäjän palkkio, € (jokainen välittäjä kerran, sen hinnastojen keskiarvona) |
| `palkkio_kallein_eur` | Kalleimman hinnaston palkkio kaksiosta, € |
| `edullisin_alue` | Postinumeroalue, jolla neliöhinta oli matalin niistä alueista, joilla oli vähintään 12 kauppaa |
| `kaksio_edullisimmalla_alueella_eur` | 55 m² kaksion hinta edullisimmalla alueella, pyöristetty tuhansiin |
| `osuus_hinnastoista_yli_5_prosenttia_edullisimmalla_alueella` | Kuinka suuri osa hinnastoista ottaisi edullisimman alueen kaksiosta yli 5 % kauppahinnasta |

### `valityspalkkiot-2026-hinnastot.csv`

Yksi rivi per hinnasto, lähdelinkin kanssa.

| Sarake | Selitys |
|---|---|
| `valittaja` | Välittäjä tai ketju |
| `toimisto` | Toimisto tai alueyhtiö |
| `kaupungit` | Kaupungit, joita paikallinen hinnasto koskee (tyhjä = ketjun yleinen tai alueellinen hinnasto) |
| `koskee` | Mitä kohteita hinnasto koskee |
| `prosentti_sis_alv` | Palkkioprosentti arvonlisäveroineen |
| `alv_mainittu` | Ilmoittiko hinnasto prosentin veroineen (`kyllä`) vai muutettiinko se verolliseksi (25,5 %) |
| `vahimmaispalkkio_eur` | Vähimmäispalkkio, € |
| `kiintea_osa_eur` | Kiinteä palkkio tai kiinteä osa, € |
| `pakolliset_lisakulut_eur` | Pakolliset kulut, joille hinnasto kertoo summan, € |
| `lisakulut_selite` | Mitä kulut ovat |
| `lahde` | Linkki välittäjän omaan hinnastoon |
| `tarkistettu` | Päivä, jona hinnasto luettiin |

## Näin luvut on laskettu

- **Palkkio euroina:** prosentti tai kiinteä hinta, vähintään vähimmäispalkkio, ja lisäksi ne pakolliset kulut,
  joille hinnasto kertoo summan. "Enintään"- ja "alkaen"-kuluja ei ole laskettu mukaan.
- **Kaksion hinta:** kaupungin vanhojen kerrostaloasuntojen keskihinta vuonna 2025 Tilastokeskuksen mukaan kertaa 55 m².
- **Keskimmäinen välittäjä:** jokainen välittäjä lasketaan kerran, sen hinnastojen keskiarvona, jottei monen
  alueyhtiön ketju painota tulosta.
- **Mitä ei ole mitattu:** neuvotellut alennukset, palvelun sisältö, välittäjät, jotka eivät julkaise hintojaan,
  sekä Huoneistokeskuksen ja Kiinteistömaailman pakolliset palvelupaketit ja kulut, koska niiden hintaa ei julkaista.

## Lähteet

- Välittäjien omat hinnastot, luettu 7.–8.10.2026 (linkki jokaisella rivillä).
- Tilastokeskus, vanhojen osakeasuntojen hinnat 2025 (CC BY 4.0).

## Lisenssi ja lähdeviite

Data on vapaasti käytettävissä lisenssillä [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Mainitse lähteenä:

> Asunnon arvo laskuri (asunnonarvolaskuri.com)

Tekijä: Lauri Niskasaari, [asunnonarvolaskuri.com](https://asunnonarvolaskuri.com/).
Toimittaja: saat minkä tahansa kaupungin tai postinumeroalueen luvut lähteineen osoitteesta
lauri@asunnonarvolaskuri.com.

Sivusto saa palkkion, jos joku pyytää sen kautta hinta-arvioita välittäjiltä. Se ei vaikuta näihin lukuihin,
koska ne tulevat suoraan hinnastoista ja tilastosta.

---

## English summary

**Real estate agent fees in Finland 2026.** Published price lists of 43 Finnish real estate agencies
(130 price lists, read from the agencies' own websites on 7–8 October 2026) and what the fee comes to in euros
for the same 55 m² flat in 15 cities. Full study with chart and table:
[asunnonarvolaskuri.com/tutkimus/valityspalkkiot-2026/](https://asunnonarvolaskuri.com/tutkimus/valityspalkkiot-2026/).

- Fees in the price lists range from 0.95 % to 5.02 % of the sale price including VAT, and minimum fees
  from €2,500 to €7,000.
- `valityspalkkiot-2026-kaupungit.csv`: one row per city (average price per m² in 2025, the 55 m² flat's price,
  cheapest / middle agency / most expensive fee, cheapest postcode area and the share of price lists that would
  take more than 5 % there).
- `valityspalkkiot-2026-hinnastot.csv`: one row per price list, with a link to the source.
- Method: fee = percentage or fixed price, at least the minimum fee, plus mandatory costs with a stated amount.
  Percentages without VAT were converted at 25.5 %. Flat prices from Statistics Finland 2025.
  Negotiated discounts are not measured.
- Column names are in Finnish; see the tables above.

**Licence:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Cite as
"Asunnon arvo laskuri (asunnonarvolaskuri.com)". Author: Lauri Niskasaari.
