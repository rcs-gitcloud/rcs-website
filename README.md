# rcs-website

Onepager van Rog Consultancy Services op https://rogcoser.nl, gehost
met GitHub Pages. Statisch: geen PHP, geen CMS, geen inlog.

| Bestand | Doel |
|---|---|
| index.html | De pagina (logo, tekst, mailto naar info@rogcoser.nl) |
| logo.png | Brandmark |
| CNAME | Custom domain voor GitHub Pages |
| .nojekyll | Bestanden 1-op-1 serveren, zonder Jekyll-build |

## DNS (bij TransIP)

De zone blijft bij TransIP. Alleen de webrecords wijzen naar GitHub
Pages; mail (Microsoft 365) blijft ongemoeid.

| Naam | Type | Waarde |
|---|---|---|
| @ | A | 185.199.108.153 |
| @ | A | 185.199.109.153 |
| @ | A | 185.199.110.153 |
| @ | A | 185.199.111.153 |
| @ | AAAA | 2606:50c0:8000::153 |
| @ | AAAA | 2606:50c0:8001::153 |
| @ | AAAA | 2606:50c0:8002::153 |
| @ | AAAA | 2606:50c0:8003::153 |
| www | CNAME | rcs-gitcloud.github.io. |

`www.rogcoser.nl` stuurt GitHub Pages automatisch door naar
`rogcoser.nl`.

## Wijzigen

Aanpassen op `main` en pushen; GitHub Pages publiceert binnen een
minuut. Hosting is tijdelijk: de definitieve plek (mogelijk Microsoft
365) volgt na een afweging.
