# 3615 KORHOGO (K Terminal)

Le Minitel de [Korhogo Fauna](https://mauktenieb.github.io/katabase), l'univers de Mauk Tenieb.

En ligne : https://mauktenieb.github.io/3615/

Le K Terminal compose le 3615 et ouvre l'accueil de 3615 KORHOGO. Le menu de l'accueil compte six entrées. Sous le menu, le Hall of Kave montre les cinq premiers de Korong! et de FaunInvaders.

1. WORLD : METEO (Open-Meteo), ENCYCLO (Wikipédia), SNCF et MINITEL, la ligne réelle vers go.minipavi.fr pour les autres codes Minitel.
2. KORHOGO : FAUNA, les 18 fiches de la Fauna ; KAVES, les Direct Kaves, un tchat en direct avec un Kave par personnage ; KALABASS, avec la boîte personnelle chiffrée, l'écriture à un autre Krew, l'annuaire et le profil ; MAUKIE, un mot pour Unkle Maukie, envoyé par e-mail.
3. KOINS : le solde, les gains du jour et le barème. Le libellé se lit KOINS ou KINOS, tiré à chaque visite.
4. KURATIONS : les cassettes « Korhogo Kuration » des visiteurs d'Insert Koin. La touche cœur du magnétoscope d'Insert Koin garde un morceau, et le 3615 lit ces cassettes sur le réseau Nostr. La liste montre 12 cassettes par page ; une cassette montre ses morceaux, 11 par page, et son adresse.
5. CURATORS : les cassettes du magnétoscope d'Insert Koin tirées des classements des curateurs, lues dans `kg-vhs-curations.js`. La liste montre 12 cassettes par page, avec leur nombre de morceaux et leur date républicaine. Une cassette montre ses morceaux, 11 par page ; ENVOI ouvre dans un nouvel onglet la lecture YouTube de ses 50 premières vidéos.
6. HALL OF KAVE : les dix meilleurs de Korong! (Masks battus, buts pris), puis ceux de FaunInvaders (score, vague atteinte), une table par page. Les données viennent de `palmares.json` d'Insert Koin et des relais Nostr.

SUITE et RETOUR tournent les pages, SOMMAIRE ramène à la liste puis à l'accueil, GUIDE affiche l'aide de la page. Le terminal parle français ou anglais.

## Codes

Chaque code marche au numéroteur (« 3615 CODE »), au kiosque et sur les pages KORHOGO. « 3615 HALL » et « HALL » mènent au même endroit.

- WORLD (ou MAIN), KORHOGO, FAUNA, KAVES, KALABASS, MAUKIE
- KOINS (ou KINOS), KURATIONS, CURATORS, HALL
- METEO, ENCYCLO, SNCF, MINITEL, KIOSQUE

Sur l'accueil, le code KORHOGO ouvre l'entrée KORHOGO.

## Pseudo et clé

KAVES et KALABASS demandent un pseudo. À la première visite, le 3615 ouvre la page du profil, puis la page demandée. MAUKIE part par e-mail et s'ouvre tout de suite.

Le navigateur signe chaque message avec une clé Nostr qu'il garde. Avec une clé créée dans le navigateur, le 3615 publie le profil de l'annuaire (kind 0). Une clé importée (nsec1…) garde son profil Nostr d'origine : le 3615 publie pour elle la présence et les messages, et le profil reste dans le navigateur. Chaque message du tchat et de la boîte comprend une preuve de travail (NIP-13, 16 bits, calculée à l'envoi en moins d'une seconde). Le 3615 affiche les messages munis de cette preuve, et un envoi en masse coûte à son auteur un calcul par message.

## Koins

- 3 Koins à la première connexion du jour au 3615 KOINS, puis 1 Koin par connexion, une heure au moins après la précédente, 10 Koins par jour au plus.
- 1 Koin par fiche de la Fauna lue jusqu'à sa dernière page, une fois par fiche.
- 1 Koin par message envoyé, dans un Kave ou en privé, 5 par jour au plus.
- 1 Koin par victoire dans un jeu d'Insert Koin.

La page KOINS affiche le solde, les gains du jour, l'heure du prochain Koin de connexion et ce barème. Le lien `?svc=koins` compose le 3615 KOINS et ouvre cette page, solde crédité. Le solde s'affiche aussi sur le boîtier (voyant `KOINS`) et en haut de l'écran. Les deux sites partagent les Koins d'[Insert Koin](https://mauktenieb.github.io/insertkoin/) (même adresse, `ik.koins` dans le navigateur).

## Fichiers

`index.html` contient tout le terminal. `apercu.png` est l'image d'aperçu des liens, `icone.png` est l'icône de l'onglet. `robots.txt`, `sitemap.xml` et `llms.txt` servent aux moteurs de recherche et aux moteurs de réponse ; `robots.txt` refuse les robots d'entraînement.

## Mettre à jour

Déposer les fichiers modifiés dans le dépôt (Add file › Upload files, puis Commit changes) : GitHub remplace l'ancien, le site suit en une ou deux minutes.

## Droits

Copyright © Mauk Tenieb & Korhogo, tous droits réservés, pour tout ce qui relève de Korhogo : personnages, textes, règles de jeu, portraits, noms (Korhogo™, Korhogo Fauna™, Fauna Masks™, Katabatik™, Insert Koin™). Toute reproduction ou réutilisation demande une autorisation écrite, y compris pour l'entraînement ou l'usage par des systèmes d'intelligence artificielle. Contact : mauktenieb@gmail.com

Le moteur du terminal (décodeur Vidéotex, sons, services généraux) relève de la licence MIT : voir `LICENSE`. La messagerie utilise [nostr-tools](https://github.com/nbd-wtf/nostr-tools) (domaine public), la météo [Open-Meteo](https://open-meteo.com) (CC BY 4.0), les textes encyclopédiques [Wikipédia](https://fr.wikipedia.org) (CC BY-SA 4.0), la police d'écran [VT323](https://fonts.google.com/specimen/VT323) (SIL OFL).

Projet indépendant d'Orange. Minitel est une marque d'Orange.

---

## English

The Minitel of [Korhogo Fauna](https://mauktenieb.github.io/katabase), the universe of Mauk Tenieb. Online: https://mauktenieb.github.io/3615/

The K Terminal dials 3615 and opens the 3615 KORHOGO home page. The home menu has six entries. Below the menu, the Hall of Kave shows the top five of Korong! and of FaunInvaders.

1. WORLD: WEATHER (Open-Meteo), ENCYCLO (Wikipedia), SNCF and MINITEL, the real line to go.minipavi.fr for the other Minitel codes.
2. KORHOGO: FAUNA, the 18 Fauna profiles; KAVES, the Direct Kaves, a live chat with one Kave per character; KALABASS, with the encrypted personal mailbox, writing to another Krew, the directory and the profile; MAUKIE, a word for Unkle Maukie, sent by e-mail.
3. KOINS: the balance, today's gains and the rules. The label reads KOINS or KINOS, drawn at each visit.
4. KURATIONS: the « Korhogo Kuration » cassettes of the visitors of Insert Koin. The heart key of the Insert Koin VHS deck keeps a track, and the 3615 reads these cassettes on the Nostr network. The list shows 12 cassettes per page; a cassette shows its tracks, 11 per page, and its address.
5. CURATORS: the tapes of the Insert Koin VHS deck drawn from the curators' rankings, read from `kg-vhs-curations.js`. The list shows 12 tapes per page, with their number of tracks and their Republican date. A tape shows its tracks, 11 per page; ENVOI opens the YouTube playback of its first 50 videos in a new tab.
6. HALL OF KAVE: the top ten of Korong! (Masks beaten, goals let in), then those of FaunInvaders (score, wave reached), one table per page. The data comes from the Insert Koin `palmares.json` and from the Nostr relays.

SUITE and RETOUR turn the pages, SOMMAIRE goes back to the list and then to the home page, GUIDE shows the help of the page. The terminal speaks French or English.

### Codes

Each code works at the dialler (« 3615 CODE »), in the kiosk and on the KORHOGO pages. « 3615 HALL » and « HALL » lead to the same place.

- WORLD (or MAIN), KORHOGO, FAUNA, KAVES, KALABASS, MAUKIE
- KOINS (or KINOS), KURATIONS, CURATORS, HALL
- METEO (or WEATHER), ENCYCLO, SNCF, MINITEL, KIOSQUE

On the home page, the code KORHOGO opens the KORHOGO entry.

### Nickname and key

KAVES and KALABASS ask for a nickname. On the first visit, the 3615 opens the profile page, then the page asked for. MAUKIE goes out by e-mail and opens at once.

The browser signs each message with a Nostr key it keeps. With a key made in the browser, the 3615 publishes the directory profile (kind 0). An imported key (nsec1…) keeps its original Nostr profile: the 3615 publishes its presence and its messages, and the profile stays in the browser. Every message of the chat and of the mailbox includes a proof of work (NIP-13, 16 bits, computed when it leaves, under a second). The 3615 shows the messages with that proof, and a mass sender pays one computation per message.

### Koins

- 3 Koins at the first connection of the day to 3615 KOINS, then 1 Koin per connection, an hour at least after the previous one, 10 Koins a day at most.
- 1 Koin per Fauna profile read to its last page, once per profile.
- 1 Koin per message sent, in a Kave or privately, 5 a day at most.
- 1 Koin per win in an Insert Koin game.

The KOINS page shows the balance, today's gains, the time of the next connection Koin and these rules. The link `?svc=koins` dials 3615 KOINS and opens this page with the balance credited. The balance also shows on the casing (`KOINS` light) and at the top of the screen. Both sites share the Koins of [Insert Koin](https://mauktenieb.github.io/insertkoin/) (same address, `ik.koins` in the browser).

### Files

`index.html` contains the whole terminal. `apercu.png` is the preview image of shared links, `icone.png` is the tab icon. `robots.txt`, `sitemap.xml` and `llms.txt` serve search and answer engines; `robots.txt` refuses training crawlers.

### Rights

Copyright © Mauk Tenieb & Korhogo, all rights reserved for everything Korhogo: characters, texts, game rules, portraits, names (Korhogo™, Korhogo Fauna™, Fauna Masks™, Katabatik™, Insert Koin™). Any reproduction or reuse requires written permission, including for training or use by artificial intelligence systems. Contact: mauktenieb@gmail.com

The terminal engine (Videotex decoder, sounds, general services) comes under the MIT licence: see `LICENSE`. Messaging uses [nostr-tools](https://github.com/nbd-wtf/nostr-tools) (public domain), weather [Open-Meteo](https://open-meteo.com) (CC BY 4.0), encyclopedic texts [Wikipedia](https://en.wikipedia.org) (CC BY-SA 4.0), the screen font [VT323](https://fonts.google.com/specimen/VT323) (SIL OFL).

Independent project, separate from Orange. Minitel is a trademark of Orange.

<!-- network:start -->
## Korhogo

Mauk Tenieb's transmedia world. [Katabase](https://mauktenieb.github.io/katabase): concept albums, the 18 Masks, the lore · [Insert Koin](https://mauktenieb.github.io/insertkoin/): Mauk Tenieb's Korhogo world, games and machines in a browser.

[Bandcamp](https://mauktenieb.bandcamp.com): music and sales · [Substack](https://korhogo.substack.com): the journal · [YouTube](https://www.youtube.com/@mauktenieb): clips and mini-films.

Index of Mauk Tenieb's sites: https://mauktenieb.github.io/
<!-- network:end -->
