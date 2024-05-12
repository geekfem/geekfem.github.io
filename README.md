# How To

Dies ist die Webseite der Gruppe Geekfem; sie ist hier live: [geekfem.net](https://geekfem.net).

## Neuer Post auf dem Blog

Blogposts sollen fürderhin nicht für die normalen Terminankündigungen verwendet werden, sondern nur noch für Inhaltliches. Der Termin kann auf "Kontakt" gesetzt werden.

```
hugo new content posts/my-first-post.md
```

Dann den Post editieren.

Dann den Server die Seiten (inkl. drafts) bauen lassen:
```
hugo server --buildDrafts
hugo server -D 
```

Mehr Infos [hier](https://gohugo.io/getting-started/quick-start/#step-2-create-a-new-site).

## Bilder einfügen

Syntax, um Bilder einzufügen:
```
{{< figure src="/arduino_small.jpg" alt="Arduino Hardware" position="center" style="border-radius: 8px;" caption="" captionPosition="right" captionStyle="color: black;" >}}
```

## Was ist wo?

- Blogposts in `content/posts/
- Bilder für die Blogposts in static/

## Github Pages

Die Webseite ist über Github Pages gehostet. Die Konfiguration dafür findet sich in .github/workflows/hugo.yml. Die Datei wurde von Github automatisch erstellt.


