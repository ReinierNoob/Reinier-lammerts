# Verbetering persoonlijke website

## Omgeving en afbakening

- Repository: ReinierNoob/Reinier-lammerts.
- Featurebranch: codex/professionele-site-20260913.
- Basiscommit: ebcc95f (Create CNAME).
- Stack: statische HTML en gedeelde CSS, zonder framework, package manager, database, formulieren, tracking of client-JavaScript.
- Bestaande productie: reinierlammerts.nl. CNAME en main blijven ongewijzigd.
- Geen productiepublicatie, DNS-wijziging of externe berichtverzending uitgevoerd.
- Geen AGENTS.md aangetroffen in de repository; de oorspronkelijke werkboom was schoon.

## Implementatiemapping

| Aanbeveling | Implementatie | Controle |
| --- | --- | --- |
| Scherpere positionering | Home, expertise en over-pagina herschreven | Copyreview tegen oorspronkelijke pagina's |
| Duidelijke vervolgstap | Contactknoppen en context per pagina | Alle lokale links en mailto-adres gecontroleerd |
| Zakelijk portret | Nieuwe reinier-zakelijk.svg met ingebedde ongewijzigde PNG, origineel behouden | Bestand en intrinsieke afmetingen gecontroleerd |
| Minder privacygegevens | Gezinsnamen en exacte woonplaats verwijderd | Statische inhoudscontrole |
| Geen lege blogpromesse | Blog uit navigatie, bestaande route bruikbaar en noindex | Navigatie, metadata en sitemap gecontroleerd |
| SEO-basis | Unieke titels/descriptions, canonicals, OG en sitemap/robots | Statische HTML-controle |
| Toegankelijkheid | Donkerder links, zichtbare focus, skiplink, landmerken | Contrast- en statische review |
| Onderhoudbaarheid | Gedeelde styles.css, native fonts, geen Google Fonts-verzoeken | Broncodecontrole |
| Foutafhandeling | Eigen 404-pagina met herstelroutes | Lokale doelen bestaan |

De teksten zijn redactioneel aangescherpt op basis van bestaande website-inhoud. Geen nieuwe opdrachtgevers, projectresultaten, cijfers, certificeringen of beschikbaarheidsclaims toegevoegd.

## Verificatie en beperkingen

- git diff --check: geslaagd.
- Alle zes HTML-pagina's: één H1, main-doel voor skiplink en bestaande lokale links/assets.
- Onafhankelijke statische review: akkoord op structuur, metadata, contactroutes, privacy, contrast en focus.
- Geen bestaande install-, lint-, typecheck- of buildtaak aanwezig; niet van toepassing op deze ongebouwde statische website.
- Browsercontrole van localhost werd expliciet geblokkeerd met ERR_BLOCKED_BY_CLIENT. Geen omzeiling uitgevoerd.
- Publieke staging en visuele controles op desktop/mobiel, keyboardtabvolgorde en gemeten performance zijn daarom nog niet afgerond.
- De nieuwe PNG is circa 1,95 MB. Dit is een ongeoptimaliseerde generatie; geen snelheidsclaim. Afbeeldingsoptimalisatie is een open vervolgpunt.
- Geen fictieve praktijkcases gemaakt: probleem, eigen bijdrage en verifieerbaar resultaat per case moeten nog door de eigenaar worden aangeleverd/bevestigd.
- Certificeringsdetails en EAW-koppeling zijn niet toegevoegd zonder actuele broncontrole.

## Overdracht

Geen nieuwe platformkoppelingen of accounts nodig. Voor publicatie eerst een bereikbare staging-URL en browsercontrole op desktop en mobiel regelen, daarna aparte productiegoedkeuring. Controleer na publicatie HTTPS, canonicals, robots/sitemap, linkpreview en contactroutes op het echte domein.

Eindstatus: poort 4 geblokkeerd op publieke staging en runtime/browser-QA. De implementatie is gereed voor die controle; productie is niet gewijzigd.

## Upload via GitHub-app

Het portret is zonder pixelwijzigingen in een SVG-container opgenomen, omdat de gekoppelde GitHub-app tekstbestanden ondersteunt. De pagina gebruikt deze SVG. Open Graph-afbeelding is bewust weggelaten: een SVG is niet geschikt als algemene social-preview-afbeelding; titel en beschrijving blijven beschikbaar. De oorspronkelijke PNG blijft lokaal bewaard. Productie is niet gewijzigd.
