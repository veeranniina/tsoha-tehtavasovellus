# Tehtävälista-sovellus
Sovellus ei ole testattavissa Fly.iossa.

Sovelluksen ominaisuuksia:

- Käyttäjä voi luoda uuden tunnuksen ja kirjautua sisään sovellukseen
- Käyttäjä voi luoda tehtävälistoja/muistiinpanoja
- Käyttäjä voi poistaa muistiinpanoja
- Käyttäjä voi määrittää tehtävien nimen, kuvauksen, määräajan
- Käyttäjä voi asettaa prioriteetit tehtäville
- Käyttäjä voi lajitella muistiinpanoja määräajan tai tärkeyden mukaan
- Käyttäjä voi muokata muistiinpanoa
- Käyttäjä voi luoda ja poistaa kategorioita ja liittää niihin muistiinpanoja muokkaamalla niitä
- Kun käyttäjä painaa "Omat kategoriat" -sivulla kategorian nimeä, avautuu kategoriaan liittyvät muistiinpanot
- Käyttäjä voi olla valitsematta kategoriaa luodessaan uutta muistiinpanoa
- Sovellus näyttää, onko käyttäjä kirjautuneena sisään, millä käyttäjänimellä
- Kun käyttäjä ei ole kirjautuneena sisään, sivu(t) ohjautuvat kirjautumissivulle
- Muistutukset näkyvät etusivulla ja omat tehtävät -sivulla
- Käyttäjä voi poistaa tilinsä sovelluksesta




Käynnistysohjeet:

Kloonaa tämä repositorio omalle koneellesi ja siirry sen juurikansioon. Luo kansioon .env-tiedosto ja määritä sen sisältö seuraavanlaiseksi:

DATABASE_URL=<tietokannan-paikallinen-osoite>

SECRET_KEY=<salainen-avain>

Seuraavaksi aktivoi virtuaaliympäristö ja asenna sovelluksen riippuvuudet komennoilla

$ python3 -m venv venv

$ source venv/bin/activate

$ pip install -r ./requirements.txt


Määritä vielä tietokannan skeema komennolla

$ psql < schema.sql

Nyt voit käynnistää sovelluksen komennolla

$ flask run
