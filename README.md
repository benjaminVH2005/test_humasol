# Humasol Kennisbank

Startpakket voor de Humasol-kennisbank, gebouwd met [Zensical](https://zensical.org/), de opvolger van Material for MkDocs.
Het leest het bestand `mkdocs.yml`, dus alle MkDocs-uitleg blijft bruikbaar.

## Online zetten (eenmalig, ±30 minuten)

1. Maak op GitHub een nieuwe repository aan, bv. `kennisbank`
2. Upload de volledige inhoud van deze map (inclusief de verborgen map `.github`)
3. Ga naar **Settings → Pages** en kies bij *Source*: **GitHub Actions**
4. Pas in `mkdocs.yml` de `repo_url` aan naar jullie repository
5. Na een paar minuten staat de site op `https://<jullie-naam>.github.io/kennisbank`

## Lokaal bekijken (optioneel)

```
pip install zensical
zensical serve
```

Open daarna http://127.0.0.1:8000 in je browser.

## Structuur

```
docs/
├── index.md                  Start hier
├── projecttypes/
│   ├── zonne-energie/        Uitgewerkt voorbeeld
│   │   ├── technologie/      Submap met meerdere pagina's
│   │   └── ...
│   └── waterpompen/
├── landen/
├── archief/
├── sjablonen/
└── bijdragen.md
```
