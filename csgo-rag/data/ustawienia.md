# Ustawienia w CS:GO

Optymalne ustawienia poprawiają widoczność, responsywność i komfort gry.
Profesjonalni gracze spędzają dużo czasu na dopasowaniu configu.

## Launch options (opcje uruchamiania)

Launch options ustawia się w Steam: prawy klik na CS:GO → Właściwości → Ogólne →
Opcje uruchamiania.

Najczęściej używane:
- `-novid` — pomija intro przy starcie gry (szybsze uruchamianie)
- `-tickrate 128` — ustawia serwery lokalne/treningowe na 128 tick (nie działa na matchmaking)
- `-high` — uruchamia grę z wysokim priorytetem procesora
- `+fps_max 0` — zdejmuje limit klatek na sekundę (lub `+fps_max 300` dla stabilności)
- `-novsync` — wyłącza synchronizację pionową (mniejszy input lag)
- `-freq 144` — ustawia częstotliwość odświeżania monitora (144 Hz)
- `-console` — włącza konsolę przy starcie
- `-nojoy` — wyłącza obsługę joysticka (nieznacznie mniej RAM)
- `-d3d9ex` — szybsze alt-tabowanie (Windows)

## Crosshair (celownik)

Celownik konfiguruje się komendami w konsoli (włącz konsolę w ustawieniach gry: ~).

### Styl celownika
- `cl_crosshairstyle 4` — statyczny klasyczny (najpopularniejszy u pro graczy)
- `cl_crosshairstyle 5` — dynamiczny (rozszerza się przy strzale)
- `cl_crosshairstyle 0` — domyślny, zmienia się z ruchem

### Wygląd celownika
- `cl_crosshairsize 2` — rozmiar celownika
- `cl_crosshairthickness 1` — grubość linii
- `cl_crosshairgap -2` — odstęp między liniami (ujemny = mniejszy)
- `cl_crosshairdot 0` — kropka na środku (0 = wyłączona, 1 = włączona)
- `cl_crosshaircolor 1` — kolor (1=zielony, 2=żółty, 3=niebieski, 4=cyan, 5=czerwony)
- `cl_crosshaircolor_r/g/b` — własny kolor RGB (np. r=0 g=255 b=0)
- `cl_crosshairalpha 255` — przezroczystość (255 = pełna widoczność)
- `cl_crosshairusealpha 1` — włącza przezroczystość
- `cl_crosshair_drawoutline 1` — czarna obwódka (lepsza widoczność)
- `cl_crosshair_outlinethickness 1` — grubość obwódki
- `cl_crosshair_t 0` — styl T (0 = pełny krzyżyk, 1 = T-shape)

Można wygenerować kod celownika na stronach (np. crashz crosshair generator) i wkleić w konsoli.

## Czułość myszy (sensitivity)

- `sensitivity 2.0` — czułość w grze (przykładowa wartość, każdy ma inną)
- `m_rawinput 1` — surowy odczyt myszy (pomija ustawienia Windows, zalecane: 1)
- `m_customaccel 0` — wyłącza akcelerację myszy (zalecane: 0)
- `m_mouseaccel1 0` — wyłącza dodatkową akcelerację
- eDPI = DPI myszy × sensitivity w grze
- Wielu pro graczy gra w przedziale eDPI 600–1000 (np. 400 DPI × 2.0 sens = 800 eDPI)
- NIE zmieniaj DPI i sensitivity często — mięście pamięć wymagają stałych ustawień

## Viewmodel (model broni w rękach)

- `viewmodel_fov 68` — pole widzenia modelu broni (54–68, wyższe = broń dalej)
- `viewmodel_offset_x 2.5` — pozycja lewo/prawo
- `viewmodel_offset_y 0` — pozycja góra/dół
- `viewmodel_offset_z -1.5` — pozycja przód/tył
- `viewmodel_presetpos 1` — preset (1=desktop, 2=couch, 3=classic)
- Niższy viewmodel = więcej widoczności ekranu (mniej broń zasłania)

## Ustawienia wideo

### Rozdzielczość i proporcje
- Większość pro graczy gra w 4:3 stretched (1024×768, 1280×960) lub natywnym 16:9
- 4:3 stretched — szersi modele graczy (łatwiejsze celowanie), mniej FOV
- `-w 1280 -h 960` w launch options dla rozdzielczości
- `mat_queue_mode 2` — multi-threaded rendering

### Grafika (wpływ na widoczność)
- Global Shadow Quality: Low/Medium — cienie graczy widoczne na niskich ustawieniach
- Model / Texture Detail: Low — łatwiejsze wyróżnienie gracza na tle
- Effect Detail: Low — mniej rozpraszających efektów
- Shader Detail: Low
- Multisampling Anti-Aliasing: None/2x — wyższe FPS
- FXAA Anti-Aliasing: Disabled
- VSync: Disabled (w grze i w NVIDIA panel)
- Motion Blur: Disabled
- Boost Player Contrast: Enabled (CS2) — lepszy kontrast modeli graczy

## Ustawienia audio

- `volume 0.5` — głośność ogólna
- `voice_enable 1` — włącza voice chat drużynowy
- `voice_scale 0.5` — głośność głosów sojuszników
- Dobry headset pozwala słyszeć kroki wroga — kluczowe na wyższych rangach
- `snd_mixahead 0.05` — opóźnienie audio (niższe = lepsze, ale może trzeszczeć)
- `snd_headphone_pan_exponent 2` — lepsze pozycjonowanie dźwięku w słuchawkach

## Radar (minimapa)

- `cl_radar_scale 0.4` — zoom radaru (niższe = szerszy widok)
- `cl_radar_always_centered 0` — radar pokazuje całą mapę (0) vs centrowany na graczu (1)
- `cl_radar_icon_scale_min 0.6` — rozmiar ikon na radarze
- `cl_hud_radar_scale 1.0` — skala HUD radaru
- Radar to kluczowe źródło informacji — patrz na minimapę co kilka sekund

## Rate i networking

- `rate 786432` — maksymalna przepustowość (786432 dla 128 tick)
- `cl_cmdrate 128` — ile pakietów wysyłasz na sekundę
- `cl_updaterate 128` — ile pakietów odbierasz (128 na 128 tick serwerze)
- `cl_interp 0` — interpolacja (0 = minimalna)
- `cl_interp_ratio 1` — ratio interpolacji
- Na matchmaking (64 tick): `cl_cmdrate 64`, `cl_updaterate 64`

## Bindy (skróty klawiszowe)

Przykładowe bindy w autoexec.cfg:
- `bind "f" "slot7"` — szybkie wyciągnięcie flashbang
- `bind "c" "slot8"` — smoke
- `bind "x" "slot10"` — molotov
- `bind "mouse4" "+voicerecord"` — push-to-talk na boczny przycisk myszy
- `bind "mwheeldown" "+jump"` — bunny hop scroll (trudne na 64 tick)
- `bind "r" "+reload; r_cleardecals"` — reload + czyszczenie krwi/dekali
- `bind "n" "toggle cl_crosshairdot 0 1"` — toggle kropki na celowniku

## Autoexec.cfg

Plik z komendami ładującymi się przy starcie gry.
Lokalizacja: `Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg\autoexec.cfg`
W launch options: `+exec autoexec.cfg`

Przykład autoexec.cfg:
```
sensitivity 2.0
m_rawinput 1
cl_crosshairstyle 4
cl_crosshairsize 2
fps_max 0
rate 786432
cl_cmdrate 128
cl_updaterate 128
```

## Przydatne komendy konsoli (trening)

- `sv_cheats 1` — włącza komendy treningowe (tylko serwer lokalny z botami)
- `mp_warmup_end` — kończy rozgrzewkę
- `mp_restartgame 1` — restart gry
- `mp_roundtime_defuse 60` — czas rundy 60 minut (trening)
- `mp_freezetime 0` — brak freeze time
- `mp_buy_anywhere 1` — kupowanie wszędzie
- `mp_buytime 9999` — nieograniczony czas na zakup
- `bot_kick` — usuwa boty
- `bot_add` — dodaje bota
- `god` — nieśmiertelność
- `noclip` — przenikanie przez ściany i latanie
- `sv_infinite_ammo 1` — nieskończona amunicja
- `sv_grenade_trajectory 1` — pokazuje trajektorię granatów
- `sv_showimpacts 1` — pokazuje ślady trafień kul
- `cl_showpos 1` — pokazuje pozycję, prędkość i kąt gracza
- `mp_respawn_on_death_ct 1` / `mp_respawn_on_death_t 1` — natychmiastowy respawn

## HUD i interfejs

- `cl_hud_color 0` — kolor HUD (0=biały, 1=biały, 2=jasnoniebieski...)
- `cl_showloadout 1` — pokazuje loadout na dole ekranu
- `hud_scaling 0.95` — skala HUD
- `safezonex/y` — bezpieczna strefa HUD (dla ultrawide)

## Ping i FPS

- `net_graph 1` — wyświetla FPS, ping, loss, choke w rogu ekranu
- `net_graphpos 2` — pozycja net_graph
- Ping poniżej 30 ms = idealny, 30–60 = OK, 60+ = przewaga wroga w timing
- `cl_showfps 1` — prostszy licznik FPS
