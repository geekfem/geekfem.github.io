# Geekfem Website

## Branches
Arbeite immer im develop-Branch, der Master-Branch wird von Octopress für die Deployments genutzt.

## Set up
### Installiere Ruby
Du brauchst (mindestens) die im [Gemfile](https://github.com/geekfem/geekfem.github.io/blob/develop/Gemfile) genannte Version.
Fuer mehr Info [hier](https://www.ruby-lang.org/de/downloads/)
Wenn du auf dem Linux per Packetmanager installierst, vergiss nicht die Header-Dateien (devel) zu installieren.

### Github Account anlegen
[Github](https://www.github.com)

### Mitglied in der geekfem organisation bei github
Es muss dich jemand zur [Organisation](https://github.com/geekfem) hinzufuegen

### Clone geekfem website repository & Projekt initialisieren
    git clone https://github.com/geekfem/geekfem.github.io.git # Projekt runterladen
    cd geekfem.github.io # ins Projektverzeichnis wechseln
    gem install bundler # bundler installieren
    bundle install # octopress und co installieren

### Seite editieren

develop-Branch auschecken:

    git checkout develop
    
Lokale Version aktualisieren:

    git pull
    bundle install
    
Neuer Artikel:

    bundle exec octopress new post "My Title"
Neue Seite:

    bundle exec octopress new page some-page

##### Markdown
Seiten und Posts die du anlegst oder editierst sind in Markdown geschrieben. Hier gibt es ein
[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

### Lokale Vorschau
Um die Aenderungen lokal anzuschauen:

    bundle exec jekyll serve

### Push und Deployment
Sieht alles super aus, kanns los gehen:  

    git add .  
    git commit -m "Artikel hinzugefuegt"
    git pull --rebase
    git push

Bauen der Seite mit:  

    bundle exec jekyll build  

Deployen auf github pages mit:  

    bundle exec octopress deploy

Fuer mehr Informationen ist die Dokumentation von [Octopress 3.0](https://github.com/octopress/octopress) sehr gut

Fuer mehr Informationen zu dem Arbeiten mit git, hier noch ein [Link.](https://de.atlassian.com/git/tutorials)
