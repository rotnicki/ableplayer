# Dziennik decyzji redakcyjnych i technicznych

Dokument jest prowadzony chronologicznie. Rozdzielamy **pomysły**, **ustalenia przyjęte** i **zmiany wcześniejszych ustaleń**. Zatwierdzone tłumaczenia trafiają do [`translations/pl.json`](../../translations/pl.json); sam dziennik nie zastępuje tego pliku.

## Reguły dokumentowania

- Każda ważna sprawa ma trwały identyfikator (np. `PL-001`), klucz lub grupę kluczy.
- Zapisujemy **oryginał**, **wersję zastaną**, **warianty**, **argumenty za i przeciw**, **kontekst funkcjonalny**, **decyzję** i **wynik testu**.
- Wpis roboczy nie jest równoznaczny ze zgodą. Do zmiany pliku tłumaczenia wymagamy zatwierdzenia w rozmowie.
- Przy zmianie stanowiska **nie wymazujemy** poprzedniej decyzji. Dopisujemy datowany wpis „zastępuje PL-...”, opis przyczyny i odsyłacz do commita.
- W dyskusjach skupiamy się na faktach językowych i technicznych; cytaty z prywatnej rozmowy publikujemy tylko na wyraźne życzenie.
- Nie oznaczamy klucza jako sprawdzonego, jeżeli potrzebny jest jeszcze test funkcjonalny.

## Etap 0 — ustalenia organizacyjne, 18 października 2026

### PROC-001 — jedna gałąź robocza i czysty pull request

Stan: **wdrożona organizacja pracy** (do modyfikacji w razie wspólnej decyzji).

- Dokumentacja robocza i bieżący przekład są razem na `polish-translation`, żeby nie powstawały rozbieżne warianty.
- Lista kontrolna wyznacza stan recenzji; dziennik wyjaśnia dlaczego; `translations/pl.json` pozostaje jedyną treścią wynikową.
- Oryginalnemu projektowi przedstawimy PR przygotowany z nowej, czystej gałęzi, zawierający tylko potrzebne zmiany tłumaczeń; dokumentację zatrzymamy w forku.
- Powód: rozdzielenie transparentności procesu od minimalnej propozycji dla opiekunów upstream.

### PROC-002 — status pierwszego przeglądu

Stan: **rozpoznanie; brak zatwierdzonych zmian w tłumaczeniu**.

- Pliki `en.json` i `pl.json` zawierają po 170 kluczy.
- W `pl.json` znajduje się 129 niepustych wartości i 41 pustych.
- Wstępne niezgodności opisano w [audycie z 18 października](audit-2026-10-18.md).
- Nie oznaczono jeszcze żadnego tekstu jako zaakceptowanego podczas tej rewizji.

## Wzór następnego zapisu

### PL-001 — nazwa i klucze (DO WYPEŁNIENIA PRZY PIERWSZEJ DECYZJI)

- **Stan:** propozycja / do testu / zatwierdzone / zastąpione.
- **Oryginał angielski:** ...
- **Tekst Stefana (jeżeli istniał):** ...
- **Stan obecny:** ...
- **Rozważone warianty:** ...
- **Argumenty i uwagi z dyskusji:** ...
- **Uzgodnione brzmienie i uzasadnienie:** ...
- **Weryfikacja w kodzie lub interfejsie:** ...
- **Akceptacja:** data i zakres.
- **Wdrożenie:** commit lub „bez zmian”.
- **Dalsze działania:** ...
