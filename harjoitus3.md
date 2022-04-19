# h3 Versionhallinta

## z) Lue ja tiivistä artikkeli muutamalla ranskalaisella viivalla. Tässä z-alakohdassa ei tarvitse siis tehdä testejä tietokoneella.

    Commonmark contributors: Markdown Reference (huomaa ainakin otsikot risuaidoilla, kappalejako tyhjällä rivillä, sisennys (tab) koodia, lista, linkki, kuva.

- Artikkeli kertoo, että markdown on helppo tapa formatoida tekstiä ja se näyttää hyvältä kaikilla laitteilla.
- Opastaa merkit joilla saa otsikot, lihavoinnin sekä muita hyödyllisiä merkkejä.

## a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.

- Loin GitHubiin repon nimeltä harjoitus3 ja kloonasin sen terminaaliini harjoituskansioon. Harjoitus3.md toimii raporttina.
- Olin aiemmin luennolla lisännyt GitHubiin ssh:n avaimen joten clone -linkki toimi sulavasti.
![image](https://github.com/Joonastesti/harjoitus3/blob/main/git1.png)

## b) Pull first. Tee useita muutoksia git-varastoosi. Tee muutama muutos, jossa yksi commit koskee useampaa tiedostoa. Anna hyvä kuvaukset (commit message), yksi englanninkielinen lause imperatiivissa (määräysmuodossa) "Add top level menu to Foobar synchronizer"

- Loin tehtävää varten muutos1.txt ja muutos2.txt -tiedostot, jotka sisältävät tekstiä.
- Git add . -komentoa seuraavaksi ja git commit sen jälkeen. Commit viestiksi laitoin: Add a new sentence to the bottom for both muutos files.
Näiden jälkeen git pull ja git push ja muutokset menivät perille GitHubiin. 

![image](https://github.com/Joonastesti/harjoitus3/blob/main/git2.png)

## c) Kaikki kirjataan. Näytä omalla git-varastollasi esimerkit komennoista ‘git log’, ‘git diff’ ja ‘git blame’. Selitä tulokset.

- git log -komento listaa kaikki kyseisen repon commitit hasheineen ja viesteineen.
- git diff harjoitus3.md -komento tulostaa ruudulle kyseisen tiedoston muutokset. Näyttää mille riveille on tullut muutoksia.
- git blame harjoitus3.md -komento näyttää kyseisen tiedoston tiedot rivi riviltä kuka on muokannut kyseistä kohtaa ja milloin. Kertoo myös riveistä jos niitä ei ole vielä commitattu. 

![image](https://github.com/Joonastesti/harjoitus3/blob/main/git4.png)
![image](https://github.com/Joonastesti/harjoitus3/blob/main/git5.png)

## d) Huppis! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.

- Tein tyhmän muutoksen muutos1.txt -tiedostoon, jonka jälkeen laitoin git add ., mutta en git commit -komentoa. 
Tuhosin muutokset git reset --hard -komennolla. Katsoin kyseistä txt -tiedostoa niin lisäämäni virke oli kadonnut. 

![image](https://github.com/Joonastesti/harjoitus3/blob/main/git6.png)

## e) Formula. Tee uusi salt-tila (formula, moduli, infraa koodina). (Eli uusi tiedosto esim. /srv/salt/terontila/init.sls). Voit tehdä ihan yksinkertaisen parin funktion (pkg, file...) tilan, tai edistyneemmin asentaa ja konfiguroida minkä vain uuden ohjelman: demonin, työpöytäohjelman tai komentokehotteesta toimivan ohjelman. Käytä tarvittaessa ‘find -printf “%T+ %p\n”|sort’ löytääksesi uudet asetustiedostot.

Loin uuden salt tilan nimeltään init.sls joka asentaa chromium paketin ja tarkastaa että kone on ajantasalla.
Asensin ensin käsiksi jo valmiiksi chromiumin sudo apt-get install chromium ja sen jälkeen loin tilan ja testasin sitä.
Ensitestauksella uptodate-ID sai haaviin chromiumin uuden version ja päivitti sen. 

![image](https://github.com/Joonastesti/harjoitus3/blob/main/git10.png) 
![image](https://github.com/Joonastesti/harjoitus3/blob/main/git7.png) 
![image](https://github.com/Joonastesti/harjoitus3/blob/main/git8.png) 
![image](https://github.com/Joonastesti/harjoitus3/blob/main/git9.png) 

## Lähteet

https://docs.saltproject.io/en/latest/ref/states/all/salt.states.pkg.html


//////////////////////////////////////////////

Tätä dokumenttia saa kopioida ja muokata GNU General Public License (versio 2 tai uudempi) mukaisesti. https://www.gnu.org/licenses/gpl-3.0.html

Pohjana Tero Karvinen 2022 Palvelinten Hallinta -kurssi https://terokarvinen.com/2021/configuration-management-systems-2022-spring/
