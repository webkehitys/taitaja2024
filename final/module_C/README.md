# Moduuli C - Intranetin toteuttaminen sivustolle

**Tehtävään käytettävä kilpailuaika: 3h**

Tässä moduulissa toteutetaan aiemmin luotuun sivustoon intranet/ylläpitotyökalu, jossa hyödynnetään tietokantaa. Intranetin pääasiallinen tarkoitus on käsitellä Hall of Fame -pelejä, niiden osallistujia ja tuloksia. Kaikkien tietojen on tultava tietokannasta, ja sinun on luotava kaikki tarvittavat tietokantataulukot. Sinun on määritettävä turvallinen ja suojattu tietokantayhteys, mukaan lukien kryptaus esim. Argon2-algoritmilla.

Koodin tuottamisessa on huomioitava, että se on laadukasta ja jatkokehityskelpoista. Koodin on oltava napakkaa, yksinkertaista ja sisältää tekniikoita, jotka helpottavat sen lukemista, jäsentämistä ja ymmärtämistä. Varmista, että lisäät readme-tiedostoon selkeät ohjeet intranetin käyttöön.

Huomioithan, että tämä moduuli tehdään samanaikaisesti seuraavan moduulin kanssa ja tämän moduulin tulokset toimitetaan kilpailupäivän lopussa.

- Intranet on saatavilla osoitteessa `/admin`
- Sisäänkirjautuminen on saatavilla osoitteessa `/login`

## Sisäänkirjautuminen

Intranet-sivustoon pääsee vain kirjautumissivun kautta sisään kirjautumalla. Jos intranet-sivuston URL-osoitteeseen menee ilman sisäänkirjautumista, niin käyttäjä ohjataan kirjautumissivulle. Kun käyttäjä on kirjautunut sisään, käyttäjänimi ja uloskirjautumispainike näkyvät päävalikossa. Kirjautumislomakkeen tiedot tarkistetaan ennen lomakkeen lähettämistä.

Kirjautumaan tulee päästä tunnuksilla:

- **admin** ja salasanalla **taitaja2024** – admin rooli
- **user** ja salasanalla **taitaja2024** – käyttäjä kirjoitus/lukuoikeudet

## Intranet

Intranetissä ylläpitäjä voi nähdä kaikki rekisteröityneet käyttäjät ja lisätä, muokata ja poistaa käyttäjiä. Lisäksi ylläpitäjät voivat nähdä kaikki Hall of Fame pelit ja tapahtumat sekä lisätä ja muokata pelejä / tapahtumia.
Käyttäjät voivat nähdä oman profiilinsa ja pelit, joihin heillä on oikeus tehdä muutoksia.

## Käyttäjäroolit

- admin (_superuser_)
- käyttäjä kirjoitus/lukuoikeudet (_user_)

**Admin voi:**

- kirjautua sisään ja ulos
- lisätä uusi käyttäjiä
  - uutta käyttäjää luodessa oletussalasana on 'taitaja2024'
- muokata käyttäjiä salasanoja
- poistaa käyttäjiä
- lisätä uusia pelejä / tapahtumia
  - uutta peliä luotaessa tarvittavat tiedot ovat otsikko (pakollinen), kuva (valinnainen), oletuksena luomishetken aikaleima päivämäärälle, montako tulosta Hall of Fame sivulla kuvataan.
- muokata pelin otsikkoa, kuvaa, päivämäärää ja näytettyjen tulosten määrä
- lisää jokaiseen peliin käyttäjiä, joilla on oikeudet lisätä ja muokata pelituloksia.

**Käyttäjä voi:**

- kirjautua sisään ja ulos
- muokata omaa salasanaa
- lisätä ja muokata pelikohtaisesti osallistujia, tuloksia, montako tulosta kuvatan pelin / tapahtuman Hall of Fame sivulla
