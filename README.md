## Geekfem Website

### Set up
#### Installiere Ruby
Fuer mehr Info [hier](https://www.ruby-lang.org/de/downloads/)

#### Github Account anlegen
[Github](https://www.github.com)

#### Mitglied in der geekfem organisation bei github
Es muss dich jemand zur [Organisation](https://github.com/geekfem) hinzufuegen

#### Clone geekfem website repository
    git clone git@github.com:geekfem/geekfem.github.io.git

#### Seite editieren
Neuer Artikel:

    octopress new post "My Title"
Neue Seite:

    octopress new page some-page

#### Lokale Vorschau
Um die Aenderungen lokal anzuschauen: 'jekyll serve'

#### Push und Deployment
Sieht alles super aus, kanns los gehen:  

    git add .  
    git commit -m "Artikel hinzugefuegt"
    git pull --rebase
    git push


Bauen der Seite mit:  

    jekyll build  

Deployen auf github pages mit:  

    octopress deploy

Fuer mehr Informationen ist die Dokumentation von [Octopress 3.0](https://github.com/octopress/octopress) sehr gut

Fuer mehr Informationen zu dem Arbeiten mit git, hier noch ein [Link.](https://de.atlassian.com/git/tutorials)
