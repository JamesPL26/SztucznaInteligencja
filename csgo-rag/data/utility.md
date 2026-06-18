# Utility (granaty) w CS:GO

Utility to granaty, które obok celowania decydują o wygrywaniu rund w CS:GO.
Profesjonalne drużyny wydają $700–$1100 na granaty w każdej rundzie full buy.
Dobrze rzucone utility potrafi wygrać rundę bez oddania strzału.

## Limity granatów

Każdy gracz może mieć maksymalnie 4 granaty naraz:
- Maksymalnie 1× HE Grenade (granat odłamkowy)
- Maksymalnie 1× Molotov/Incendiary (granat ognisty)
- Maksymalnie 2× Flashbang (granat ogłuszający)
- Smoke Grenade i Decoy nie mają limitu ilościowego w slotach, ale max 4 granaty łącznie

Typowy full buy utility CT: smoke + 2 flash + molotov/incendiary = 4 sloty
Typowy full buy utility T: smoke + 2 flash + molotov = 4 sloty

## Smoke Grenade (granat dymny)

- Cena: $300
- Czas trwania: około 18 sekund
- Działanie: tworzy kulisty dym blokujący widoczenie (nie blokuje dźwięków!)
- Zastosowanie:
  - Odcięcie linii ognia (block line of sight)
  - Zasłonięcie wejścia na bombsite (execute smoke)
  - Blokowanie pozycji AWP (smoke off angle)
  - One-way smoke — dym ustawiony tak, że widzisz wroga, a on ciebie nie
  - Fake smoke — smoke na jednym site, żeby zmylić rotację CT
- Smoke wybucha po ~1 sekundzie od rzutu (nie od razu)
- Smoke można zniszczyć granatem odłamkowym (HE) — "smoke busting"
- Smoke na ziemi można przeskoczyć — dym nie blokuje ruchu

### Znane smoki (przykłady)
- Mirage: smoke window (z T spawn), smoke connector, smoke jungle
- Dust II: smoke long, smoke cross (mid→long), smoke B doors
- Inferno: smoke banana, smoke CT (A site)
- Nuke: smoke outside, smoke ramp

## Flashbang (granat ogłuszający)

- Cena: $200
- Działanie: oślepia (biały ekran) i ogłusza graczy patrzących w stronę wybuchu
- Czas oślepienia: zależy od odległości i czy gracz patrzy prosto (do ~3 sekund)
- Można mieć 2 flashbangi naraz — kluczowe w execute
- Zastosowanie:
  - Pop flash — rzut tuż przed wejściem na site, oślepia broniących
  - Support flash — flash dla sojusznika wchodzącego na pozycję
  - Self flash — flash dla siebie (trudniejsze, wymaga odwrócenia się)
  - Flash over wall — flash przez ścianę (nie trzeba widzieć wroga)
  - Fake flash — rzut bez wejścia, żeby wyciągnąć rotację
- Flash oślepia też sojuszników! Uważaj na team flash (TK flash)
- Okulary antyflash (modele postaci) skracają czas oślepienia — kosmetyka
- Flash wybucha po ~1.5 sekundy — licz timing

## Molotov (Terroryści) / Incendiary Grenade (Antyterroryści)

- Cena: Molotov $400 (T), Incendiary $600 (CT)
- Czas trwania ognia: około 7 sekund
- Obrażenia: ~40 HP/s przy staniu w ogniu (bardzo wysokie!)
- Zastosowanie:
  - Area denial — blokowanie przejścia (np. banana na Inferno, choke point)
  - Wykurzanie gracza z osłony (force out of cover)
  - Opóźnianie wejścia wroga na site
  - Przerywanie rozbrajania bomby (CT nie może stać w ogniu)
  - Post-plant molotov — ogień na bombę, wymusza wycofanie CT
  - Molotov na defuse kit — wymusza przerwanie rozbrajania
- Ogień rozlewa się po podłożu — nie można go przeskoczyć
- CT Incendiary droższy ($600) i mniejszy zasięg niż T Molotov ($400)

## HE Grenade (granat odłamkowy)

- Cena: $300
- Działanie: wybucha natychmiast po uderzeniu, zadaje obrażenia obszarowe
- Obrażenia: do ~57 HP w centrum wybuchu (maleje z odległością)
- Można mieć tylko 1 HE
- Zastosowanie:
  - Dobijanie osłabionych przeciwników (np. 30 HP po wymianie)
  - Zadawanie obrażeń grupie wrogów (stack damage)
  - Niszczenie smoke'a (smoke busting)
  - Otwieranie rundy (opening nade) — rzut na znane miejsce (np. banana)
  - HE lineup — precyzyjny rzut zadający stałe obrażenia
- HE może zabić samego siebie — uważaj na self damage

## Decoy Grenade (granat wabik)

- Cena: $50 (najtańszy granat)
- Działanie: imituje dźwięk strzałów broni gracza, myląc minimapę wroga
- Czas trwania: około 15 sekund
- Zastosowanie:
  - Fake attack — decoy na jednym site, atak na drugi
  - Zwiad — sprawdzenie reakcji CT (rotacja = wiedza o pozycjach)
  - Fałszywe informacje na minimapie
  - Rzadko używany profesjonalnie, ale tani ($50)

## Execute (składany atak na site)

Execute to skoordynowany atak T-side na bombsite z pełnym wykorzystaniem utility:
1. Smokes — zasłaniają kluczowe pozycje CT (AWP angles, crossfires)
2. Flashes — oślepiają graczy na site przed wejściem
3. Molotov — wykurza CT z osłon (np. molotov car na Dust II B)
4. Entry fragger — pierwszy gracz wchodzi po flashu, szuka opening kill
5. Trade — sojusznicy wchodzą za entry, żeby zabić tego kto zabił entry

Typowy execute wymaga 4–5 granatów od całej drużyny (nie od jednego gracza).

## Lineupy (stałe rzuty granatów)

Lineup to precyzyjny punkt celowania + pozycja stania, który za każdym razem
daje ten sam efekt (smoke w to samo miejsce, flash przez ścianę, HE na znany spot).

- Ćwiczy się na serwerach treningowych (yprac, aim_botz, map-specific nade servers)
- Kluczowe lineupy: smoke window Mirage, smoke long Dust II, molotov banana Inferno
- Jump throw bind — bind do rzutu w skoku (wymaga sv_cheats 0 na serwerze community)
- Komenda: `bind "key" "+jump; -attack; -jump"` (uproszczony jumpthrow)

## Utility po stronie CT

CT używa utility defensywnie:
- Smoke — opóźnienie pushu T (smoke choke point)
- Flash — oślepienie wchodzącego T
- Molotov/Incendiary — blokowanie wejścia, wykurzenie z bomb site po plant
- HE — obrażenia na znane wejścia (pre-fire nade spots)
- Retake utility — granaty do odzyskania site po podłożeniu bomby

## Utility w retake (odzyskiwanie site)

Po podłożeniu bomby przez T, CT musi ją odzyskać:
- Smoke na bombę — zasłonięcie defusera
- Flash przed wejściem na site
- Molotov na bombę — wymusza przerwanie defuse
- HE na znane pozycje post-plant (default, car, pit)

## Kluczowe zasady utility

- Smoke + flash przed wejściem na site to podstawa execute
- Molotov świetnie nadaje się do przerwania rozbrajania bomby
- Nie marnuj utility w rundach eco — oszczędzaj na full buy
- Team utility > solo utility — koordynacja 5 graczy wygrywa rundy
- Timing flashów: za wcześnie = wróg się schowa, za późno = giniesz przed flash
- Po smoke wroga: możesz przebiec przez dym (risky) lub czekać aż opadnie
