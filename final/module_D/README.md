# Moduuli D - Interaktiivisen moduulin tekeminen

**Tehtävään käytettävä kilpailuaika: 4h**

![snakegame](/module_D/snake.webp)
Tässä moduulissa luot interaktiivisen matopelin. Idea on sama kuin Nokian tekemässä matopelissä, mutta tässä ohjataan yhtä aikaa kahta matoa. Pelin on näytettävä ja tunnuttava kuin oikea retropeli.

Pelin tulee olla saatavilla URL-osoitteessa: `/pelit/matopeli`

## Pelin aloitus

Peli alkaa “Aloita”-painikkeesta.

## Pelin toiminnallisuus

Pelissä pelaaja ohjaa yhtä aikaa kahta matoa. Ensimmäistä matoa ohjataan näppäimillä ADWS ja toista nuolinäppäimillä. Mato liikkuu neljään suuntaan (ylös, oikealle, alas ja vasemmalle). Pelissä ilmestyy satunnaisesti syötäviä “omenia”, joita syömällä pelaaja saa pisteitä (yksi piste omenasta) ja mato kasvaa pituutta (yksi piste lisäksi). Kun pelaaja kulkee pelialueen reunan yli, mato siirtyy ruudun vastakkaiselle puolelle. Peli päättyy, kun mato törmää itseensä tai toiseen matoon.

## Pelin päätösruutu

Peli päättyy päätösruutuun, jossa näkyy pisteet.
Lisäksi kysymys ”Haluatko tallentaa tuloksen?” kuvataan pelaajalle. Pelaaja voi valita ”kyllä” tai ”ei”:

- Jos pelaaja valitsee ”kyllä”, silloin nimen syöttökenttä ja lähettämispainike tulevat näkyviin. Nimen syötön jälkeen (pakollinen), tulokset tallennetaan tietokantaan (käyttäjänimi, tulos sekä päivämäärä ja kellonaika) ja pelaajalle näytetään onnistumisviesti sekä ”pelaa uudelleen?” -painike.
- Jos pelaaja valitse ei, sitten ”pelaa uudelleen?” painike tule näkyviin.

## Hall of Fame päivitys

Jos pelaaja valitsee tallentaa tuloksen, pelaajan nimi ja tulos näytetään pelin Hall of Fame -tulosten listalla tietokannasta.

**Päivän lopussa sinun on toimitettava C ja D moduulit:**

- toimiva verkkosivusto mikä käyttää tietokantaa.
- Lopullinen GitHub-repositorio
- `README.md` tiedosto sisältää ohjeet intranettiin ja peliin
