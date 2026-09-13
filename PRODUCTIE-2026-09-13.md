# Productierecord 2026-09-13

Gebruiker gaf expliciet opdracht: Zet in productie.

- Release: 2e20b536afff6ca8377a40efbfd73c1e75417cc6 (PR 1, squash naar main).
- Herstelpunt: ebcc95faf3515d26d57f206fe0c428935d35ae13.
- Hosting en domeinconfiguratie niet gewijzigd.
- Eigenaar website en beheer: Reinier Lammerts, repositoryaccount ReinierNoob.

## Productiecontrole

Op https://reinierlammerts.nl/ met de browser bevestigd: nieuwe homepage, zakelijke foto zichtbaar, afbeelding geladen met intrinsieke afmetingen 1122 x 1402, geen horizontale overflow op het gecontroleerde desktopscherm.

Navigatie daadwerkelijk aangeklikt: homepage → Expertise → Bespreek je vraagstuk → Contact. Nieuwe teksten en mailto-link naar het bestaande contactadres gecontroleerd. Over mij ook geopend en nieuwe tekst bevestigd. Geen e-mail verzonden.

## Open controles

Mobiele visuele controle en performancemeting zijn niet uitgevoerd. Browsercontrole van /robots.txt werd geblokkeerd met ERR_BLOCKED_BY_CLIENT; daarna geen alternatieve route gebruikt. Sitemap live daardoor niet gecontroleerd. Beide bestanden zijn eerder statisch gevalideerd en staan in de release.

De foto heeft een ongewijzigde PNG in een SVG-container. Social preview bevat titel en beschrijving, geen afbeelding. Praktijkcases, extra certificeringsdetails en EAW-verwijzing zijn nog niet toegevoegd wegens ontbrekende bronverificatie.

## Beheer en herstel

De vorige productieversie blijft in Git bereikbaar. Bij uitval van hoofdcontent, navigatie of portret: oorzaak controleren en zo nodig releasewijzigingen via een revert terugdraaien naar het hierboven geregistreerde herstelpunt. Niet force-pushen of geschiedenis verwijderen. Er zijn geen databases, migraties, contactformulieren of nieuwe accounts toegevoegd.

Geen permanente monitoring ingesteld; eigenaar kan problemen via deze conversatie laten onderzoeken. Inhoudelijke updates en aanvullende bronbevestiging lopen via de eigenaar. Geen secrets in dit record.

Status: productiepublicatie en desktop-smoketest geslaagd; volledige poort 8 blijft beperkt door open mobiele en overige runtimecontroles. Dit record vervangt de eerdere status 'productie niet gewijzigd' in de stagingoverdracht.
