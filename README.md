# TwinStickShooter

## Johdanto
SwinStickShooter on Unreal Engine 5.2 versiolla luotu peli, jossa pelaaja ohjaa hahmoa käyttäen peliohjainta tai WASD-näppäimiä. Tämä dokumentti sisältää asennusohjeet, pelimekaniikan kuvauksen ja teknisen dokumentaation.

## Asennusohjeet
1. Asenna Unreal Engine versio 5.5 Epic Games Launcherilla.
2. Lataa projekti GitHubista osoitteesta https://github.com/fnike005/MyProject-2 ja avaa `MyProject`-tiedosto Unreal Editorissa.
3. Käännä projekti Visual Studiolla, jos käyttöjärjestelmä sitä vaatii.

## Peliohjeet
- **Pelin aloitus:** Avaa MainMenuMap, ellei se ole jo valittuna. Sen jälkeen paina play-näppäintä. Tämä vie pelin aloitusvalikkoon, josta painamalla "play" peli alkaa.
- **Liikkuminen:** Käytä peliohjaimen vasenta ja oikeaa tattia, tai WASD- ja nuolinäppäimiä hahmon ohjaamiseen.
- **Pelin lopettaminen:** Peli on mahdollista lopettaa quit-näppäimellä aloitusvalikosta tai vastaavasti elämän loppuessa ilmestyvästä "game over" valikosta. 

## Tekninen dokumentaatio
Projekti on rakennettu yhdistämällä Blueprintit ja C++-koodit.

Projektin luomisessa pieniä haasteita liittyen tutoriaalissa käytettyyn vanhempaan pelimoottori versioon 4.8. Ongelmat oli kuitenkin helposti sovellettavissa. 

Projektin rakenteessa keskeisenä ongelmana ilmeni Hero Characterin childiksi luotu Enemy Character, joka peri automaattisesti osan Hero Characterin ominaisuuksista, joita en ollut tarkoittanut perittäväksi. Esimerkkinä aseen kytkeytyminen myös Enemy Characteriin, mutta tämän sain korjattua. 

Projectilen toiminta ei ole täysin ideaalinen. Lasereiden tulsi pysähtyä viholliseen osuttaessa, mutta tähän en löytänyt syytä. Alkeelliset particle efektit olivat myös työn alla, mutta ne eivät luonnollisesti ole nähtävissä pelissä. 

Jatkokehityksenä projektista tulisi korjata virheet ja sen jälkeen voisi luoda progressiivisesti vaikeutuvia tasoja. Lisäksi elämät, kerättävät itemit tai gemit lisäisivät hauskuutta pelikokemukseen. Menut tulisi tehdä täysin uudelleen peliin paremmin sopiviksi sekä tarjota pelaajalle mahdollisuuksia määrittää asetuksia.

Katso lisätiedot lähdekoodista ja Blueprint-kommenteista.
