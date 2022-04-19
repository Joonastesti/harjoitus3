# h3 Versionhallinta

## z) Lue ja tiivistä artikkeli muutamalla ranskalaisella viivalla. Tässä z-alakohdassa ei tarvitse siis tehdä testejä tietokoneella.

    Commonmark contributors: Markdown Reference (huomaa ainakin otsikot risuaidoilla, kappalejako tyhjällä rivillä, sisennys (tab) koodia, lista, linkki, kuva.
- Artikkeli kertoo, että markdown on helppo tapa formatoida tekstiä ja se näyttää hyvältä kaikilla laitteilla.
- Opastaa merkit joilla saa otsikot, lihavoinnin sekä muita hyödyllisiä merkkejä.
## a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.
- Loin GitHubiin repon nimeltä harjoitus3 ja kloonasin sen terminaaliini harjoituskansioon. Harjoitus3.md toimii raporttina.
- Olin aiemmin luennolla lisännyt GitHubiin ssh:n avaimen joten clone -linkki toimi sulavasti.
## b) Pull first. Tee useita muutoksia git-varastoosi. Tee muutama muutos, jossa yksi commit koskee useampaa tiedostoa. Anna hyvä kuvaukset (commit message), yksi englanninkielinen lause imperatiivissa (määräysmuodossa) "Add top level menu to Foobar synchronizer"
- Loin tehtävää varten muutos1.txt ja muutos2.txt -tiedostot, jotka sisältävät tekstiä.
- Näitä ennen olin suorittanut komennot git pull ja git push. Git add . -komento seuraavaksi ja git commit sen jälkeen. Commit viestiksi laitoin: Add a new sentence to the bottom for both muutos files. 
## c) Kaikki kirjataan. Näytä omalla git-varastollasi esimerkit komennoista ‘git log’, ‘git diff’ ja ‘git blame’. Selitä tulokset.

## d) Huppis! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.

## e) Formula. Tee uusi salt-tila (formula, moduli, infraa koodina). (Eli uusi tiedosto esim. /srv/salt/terontila/init.sls). Voit tehdä ihan yksinkertaisen parin funktion (pkg, file...) tilan, tai edistyneemmin asentaa ja konfiguroida minkä vain uuden ohjelman: demonin, työpöytäohjelman tai komentokehotteesta toimivan ohjelman. Käytä tarvittaessa ‘find -printf “%T+ %p\n”|sort’ löytääksesi uudet asetustiedostot.
