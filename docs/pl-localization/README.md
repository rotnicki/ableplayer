# Polska lokalizacja Able Player — prace robocze

Stan początkowy: 18 października 2026 r. Repozytorium robocze: `rotnicki/ableplayer`, gałąź `polish-translation`.

## Cel

Wspólnie przejrzeć, poprawić, uzupełnić i przetestować polskie komunikaty Able Player 5, zachowując historię rozstrzygnięć. Szanujemy wcześniejszą pracę Stefana Wajdy: [pierwotne dodanie tłumaczenia (14 marca 2024)](https://github.com/ableplayer/ableplayer/commit/6c41745b7b122c2c7e019eaa53e4aba68c6a16ef), [poprawki do 26 marca 2024](https://github.com/ableplayer/ableplayer/commit/2c9a4f367e07f866c7a0e70fbcbe7e463e4291ce).

## Trzy rodzaje zapisów

1. **Tekst wynikowy:** [`translations/pl.json`](../../translations/pl.json) — jedyne źródło obowiązującego tłumaczenia.
2. **Stan przeglądu:** [`checklist.md`](checklist.md) — każdy klucz odhaczany dopiero po przeglądzie i akceptacji.
3. **Przesłanki i wybory:** [`decisions.md`](decisions.md) — proponowane warianty, argumenty, ustalenia, zmiany stanowiska, odsyłacze do commitów.
4. **Zapis punktu wyjścia:** [`audit-2026-10-18.md`](audit-2026-10-18.md) — porównanie z oryginałem angielskim i historią wersji Stefana.

## Przebieg przeglądu

1. Omawiamy niewielki pakiet (około 10–15 kluczy) w obrębie jednego obszaru.
2. Dla problematycznych kluczy porównujemy tekst angielski, polski bieżący i — jeśli istnieje — historyczną propozycję Stefana. Przy niejasnościach sprawdzamy, gdzie komunikat występuje w kodzie i co rzeczywiście robi.
3. Rozdzielamy **obserwację**, **propozycję**, **zatwierdzoną decyzję**, **wdrożenie** i **test**. Nie traktujemy automatycznej propozycji jako zatwierdzenia.
4. Po decyzji użytkownika zapisujemy uzasadnienie w dzienniku, oznaczamy sprawdzone klucze na liście i aktualizujemy `translations/pl.json` (tylko gdy wymagają zmiany).
5. Każdą partię zapisujemy w czytelnym commicie. W dzienniku decyzji dopisujemy numer commita oraz ewentualny wynik testów.
6. Przy powrocie do tematu czytamy najpierw dokumentację w repozytorium, zamiast polegać wyłącznie na pamięci rozmowy.

## Statusy

- **Nieprzejrzane:** puste pole wyboru na liście.
- **Zaakceptowane:** zaznaczone pole wyboru; nie musi oznaczać zmiany istniejącego tekstu.
- **Do dyskusji / do testu:** jawna adnotacja w `decisions.md` lub w opisie pozycji na liście, pozostająca niezaznaczona.
- **Utrzymany angielski świadomie:** decyzja wyjaśniona w dzienniku; pusty ciąg może uruchamiać poprawny angielski fallback.
- **Decyzja zastąpiona:** nie kasujemy wcześniejszego uzasadnienia, ale dopisujemy nowe stanowisko i odsyłacz.

## Gałęzie i zgłoszenie do oryginalnego projektu

- `main`: stara, nienaruszona kopia; nie jest podstawą współczesnych tłumaczeń.
- `develop`: kopia gałęzi rozwojowej autorów, według stanu początkowego.
- `polish-translation`: wspólna gałąź robocza zawierająca `pl.json` **i** dokumentację. Tu utrzymujemy jeden spójny stan roboczy.
- **Nie otwieramy pull requesta bezpośrednio z `polish-translation`**. Na końcu utworzymy nową gałąź PR z aktualnego `develop` autorów i przeniesiemy do niej tylko zaakceptowany `translations/pl.json` (oraz ewentualne inne pliki, jeśli autorzy wyraźnie o nie poproszą). Dziennik pozostanie w naszym forku.

Nowe zmiany upstream nie synchronizują się automatycznie. Przed końcowym zgłoszeniem sprawdzimy aktualny `develop`, różnice i poprawność kluczy.

## Publiczność i redakcja dokumentacji

Repozytorium jest **publiczne**. Zapisujemy techniczne argumenty i świadomie zaakceptowane wnioski, ale nie kopiujemy całej prywatnej rozmowy ani danych osobowych. Parafrazy opinii nie są dosłownymi cytatami użytkownika. Ewentualne cytaty tylko na wyraźne życzenie.

Dokumentacja służy do pracy redakcyjnej i nie jest planowana do dołączenia do pull requesta.

## Źródła porównania

- [Angielski tekst źródłowy](https://github.com/ableplayer/ableplayer/blob/develop/translations/en.json)
- [Polski tekst na gałęzi roboczej](../../translations/pl.json)
- [Kod ustawień i komunikatów](https://github.com/ableplayer/ableplayer/blob/develop/scripts/preference.js)
- [Oficjalne zasady współtworzenia](https://github.com/ableplayer/ableplayer/blob/develop/contributing.md)
- Początkowy commit upstream `develop`: `efed8aaf3a9151d5d9dbc147321f28a2a2830b3d` (15 października 2026).
