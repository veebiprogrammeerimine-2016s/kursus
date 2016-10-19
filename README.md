# Veebiprogrammeerimine sügis 2016

* **Kursuseprogramm:** [IFI6076](http://www.cs.tlu.ee/instituut/oppe_tegevus/kp/kp_s_2016/)
* **Õpetaja:** Romil Rõbtšenkov, [romilr@tlu.ee](mailto:romilr@tlu.ee)
* **Testserver:** greeny.cs.tlu.ee, [tunneli loomise juhend](http://minitorn.tlu.ee/~jaagup/kool/java/kursused/09/veebipr/naited/greenytunnel/greenytunnel.pdf)
* **Tunni näited testserververis:** ~romil/if15
* **Rühmad:** [I rühm](https://github.com/veebiprogrammeerimine-2016s?utf8=%E2%9C%93&query=-I-ruhm), [II rühm](https://github.com/veebiprogrammeerimine-2016s?utf8=%E2%9C%93&query=-II-ruhm), [III rühm](https://github.com/veebiprogrammeerimine-2016s?utf8=%E2%9C%93&query=-III-ruhm), [IV rühm](https://github.com/veebiprogrammeerimine-2016s?utf8=%E2%9C%93&query=-IV-ruhm)
* **Stiilijuhend:** [Coding Style Guide](http://www.php-fig.org/psr/psr-2/)
* **GIT õpetus:** [Become a git guru.](https://www.atlassian.com/git/tutorials/)
* **Abimaterjale:** [Veebirakenduste loomine PHP ja MySQLi abil](http://minitorn.tlu.ee/~jaagup/kool/java/loeng/veebipr/veebipr1.pdf), [PHP with MySQL Essential Training] (http://www.lynda.com/MySQL-tutorials/PHP-MySQL-Essential-Training/119003-2.html)
* **Vajad abi?**
   *  Loo [Issue](https://github.com/veebiprogrammeerimine-2016s/kursus/issues)
   * Kirjuta [email](mailto:romilr@tlu.ee) - 1:1 abi

## Kodused tööd ja projektid

Kõik kodused tööd on välja toodud [Kursus](#Kursus) tundide loendis.

### Ühendus Greeny'sse

* Windows | [VIDEO](https://youtu.be/kg5NAsRQAJ8)

    * [Guide to create tunnel (in estonian, but with screenshots)](http://minitorn.tlu.ee/~jaagup/kool/java/kursused/09/veebipr/naited/greenytunnel/greenytunnel.pdf)

* Mac OS | [VIDEO](https://youtu.be/RJc-Gvpn9M4)
```
1. open Terminal app

2. write:
ssh university_username@lin2.tlu.ee -L 5555:greeny.cs.tlu.ee:80
3. then write TLU password

    Now you can access greeny from browser localhost:5555

3. open new tab in Terminal (cmd+t) and write:
ssh university_username@lin2.tlu.ee -L 2222:greeny.cs.tlu.ee:22
4. then write TLU password

5. now open FTP client (CyberDuck, FileZilla, Coda) for example and connect to greeny via SFTP
    host: localhost or some require 127.0.0.1 (127.0.0.1 = localhost)
    port: 2222
    username: your_greeny_username
    password: your_greeny_username

6. choose one Terminal tab and connect to greeny via ssh, write:
ssh greeny_username@greeny.cs.tlu.ee
7. then enter your Greeny username password
    ls             – to view files and folders in current path
    cd folder_name - to enter folder
    cd ..          – to exit folder to previous path

```

### GitHub'i töövoog

1. *Fork*'i ülesande/projekti repositoorium (leiab [github.com/veebiprogrammeerimine-2016s](https://github.com/veebiprogrammeerimine-2016s)).
1. *Clone*'i see repositoorium enda arvutisse/serverisse ja määra repositooriumi URL kuhu edaspidi muudatusi salvestad.
  ```
  git clone https://USERNAME@github.com/USERNAME/REPOSITORY.git
  ```
1. Muuda faile ülesande lahendamiseks ja *Commit*'i iga olulisem muudatus, kasutades kahte käsku.
  ```
  git add .
  ```
  ```
  git commit -m "Added this functionality to the app"
  ```
1. Veendu, et kogu kood on *Commit*'itud.
  ```
  git status
  ```
1. *Push/sync*'i GitHub'i.
  ```
  git push origin
  ```
1. [Ava *pull request*](https://help.github.com/articles/creating-a-pull-request) ülesande originaalses repositooriumis. Ülesannete tähtajaks on järgmise tunni algus, kui pole teisiti kirjas.
1. Muudatusi ja täiendusi võib *push*'ida repositooriumisse, kuni ette antud  kuupäevani.

Tagasisidet saab otse *pull request*'i millele ootan Sinupoolseid kommentaare/mõtteid/küsimusi. Võid julgselt avada *pull request*'i kohe kui hakkad kodutöö kallal tegelama ja siis kui hätta jääd võid esitada sinna küsimuse. Maini kommentaaris minu kasutajat `@romilrobtsenkov` siis jõuan sellele kiiremini vastata.

### Nõuded

Need rakenduvad ka päris elus!

* Peab järgma "head programmeerimise stiili"
    * Muutujate nimed peavad kirjeldama muutujat ning peavad olema inglise keeles
    * Funktsiooni nimi peab olema "lühike"
    * Optimeeritud koodi lugemiseks
    * Projektide jaoks tuleb kasutada objektorienteeritud lähenemist
    * Laenatud koodile tuleb viidata
* Boonuspunktid:
    * Loomingulisus (nb! nõuded peavad olema täidetud)

## Kursus

### 1. tund

1. Sissejuhatus
    * Arutleme, mis antud kursus endas hõlmab
    * Igaüks tutvustab ennast
        * Nimi
        * Millised on Sinu huvid/hobid?
        * Mis toob Sind informaatikat õppima?
1. Ettevalmistus
    * Installi GitHub [Mac](https://mac.github.com) või [Windows](https://windows.github.com) (isiklikku arvutisse)
    * Tee endale [GitHub](https://github.com/)'i kasutaja
1. GitHub töövoog
    * Räägime läbi GitHub'i töövoo
    * Teeme testrepositooriumid
1. Kasutatud käsud
```
// kausta sisenemine
cd kaustaNimi

// kaustas väljumine
cd ..

// käskude ajalugu
history

// GIT
git clone https://romilrobtsenkov@github.com/romilrobtsenkov/kursus.git
git add .
git commit -m "Sõnum muudatustest"
git push origin master 

// kui annab Forbidden error'i siis võib olla salvestuse URL vale, saab muuta nt nii
git remote set-url origin https://romilrobtsenkov@github.com/romilrobtsenkov/kursus.git
```

### 2. tund

1. Alustame koodikirjutamist
    * muutujad, loogika, tsüklid, kuupäev
    * HTML vorm ja selle valideerimine
1. Abimaterjal
    * [PHP 5 Form Handling] (http://www.w3schools.com/php/php_forms.asp)
    * ...
    * [PHP 5 Form Complete] (http://www.w3schools.com/php/php_form_complete.asp)
1. Kodutöö
    * [1. kodutöö](https://github.com/veebiprogrammeerimine-2016s?utf8=%E2%9C%93&query=1.kodutoo)

### 3.tund
```SQL
CREATE TABLE user_sample (
    id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    email VARCHAR(255) NOT NULL,
    password VARCHAR(128) NOT NULL,
    created TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    UNIQUE(email)
);
```
### 7.tund
```SQL
CREATE TABLE interests (
    id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    interest VARCHAR(255) NOT NULL,
    UNIQUE(interest)
);

CREATE TABLE cars_and_colors (
  id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  plate VARCHAR(6) NOT NULL,
  color VARCHAR(7) NOT NULL
);
```
## Litsents
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Käesolev <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">leht</span> ja kõik teised https://github.com/veebiprogrammeerimine-2015s materjalid on <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International Litsensiga</a>.
