# Lista przeglądu polskiej lokalizacji

Stan początkowy: 18 października 2026 r. **0 z 170 kluczy zatwierdzonych w naszej rewizji.**

## Jak odhaczać

- `[ ]` — klucz niezatwierdzony; także wtedy, gdy polskie tłumaczenie istnieje.
- `[x]` — użytkownik zatwierdził brzmienie lub świadomy brak tłumaczenia po analizie.
- „Puste” opisuje plik wyjściowy; nie przesądza, czy trzeba tłumaczyć (np. niezmieniane angielskie nazwy klawiszy).
- „Uwaga” to problem wstępnie wykryty, a nie rozstrzygnięta zmiana.
- Treść tłumaczenia zawsze sprawdzamy w [`translations/pl.json`](../../translations/pl.json); nie duplikujemy jej tutaj, by uniknąć rozjazdu.
- Istotne uzasadnienia i zmiany zdania zapisujemy w [dzienniku](decisions.md).

## 01. Sterowanie i identyfikacja odtwarzacza (37)

- [ ] `playerHeading`
- [ ] `audioPlayer` — puste
- [ ] `videoPlayer` — puste
- [ ] `faster`
- [ ] `slower`
- [ ] `play`
- [ ] `pause`
- [ ] `restart` — puste
- [ ] `prevTrack`
- [ ] `nextTrack`
- [ ] `rewind` — uwaga: brakuje w polskim tłumaczeniu parametru %1 (liczba sekund)
- [ ] `forward` — uwaga: brakuje w polskim tłumaczeniu parametru %1 (liczba sekund)
- [ ] `captions`
- [ ] `showCaptions`
- [ ] `hideCaptions`
- [ ] `captionsOff`
- [ ] `showTranscript`
- [ ] `hideTranscript`
- [ ] `turnOnDescriptions`
- [ ] `turnOffDescriptions`
- [ ] `chapters`
- [ ] `language`
- [ ] `sign`
- [ ] `showSign`
- [ ] `hideSign`
- [ ] `seekbarLabel` — uwaga: warto sprawdzić podstawianie %1 i brzmienie etykiety
- [ ] `mute`
- [ ] `unmute` — uwaga: „Pogłośnij” nie oddaje przywrócenia dźwięku po wyciszeniu
- [ ] `volume`
- [ ] `volumeUpDown`
- [ ] `preferences`
- [ ] `enterFullScreen`
- [ ] `exitFullScreen`
- [ ] `speed`
- [ ] `on` — puste
- [ ] `off` — puste
- [ ] `spacebar`

## 02. Statusy i komunikaty o odtwarzaniu (11)

- [ ] `transcriptTitle`
- [ ] `lyricsTitle`
- [ ] `autoScroll`
- [ ] `statusPlaying`
- [ ] `statusPaused`
- [ ] `statusStopped`
- [ ] `statusBuffering`
- [ ] `statusEnd`
- [ ] `selectedTrack`
- [ ] `alertDescribedVersion`
- [ ] `alertNonDescribedVersion`

## 03. Menu i informacje o audiodeskrypcji (18)

- [ ] `prefMenuCaptions`
- [ ] `prefVoicedCaptions` — uwaga: pozostawiony angielski tekst „Spoken Captions”
- [ ] `prefMenuDescriptions`
- [ ] `prefMenuKeyboard`
- [ ] `prefMenuTranscript`
- [ ] `prefTitleCaptions`
- [ ] `prefTitleDescriptions`
- [ ] `prefTitleKeyboard`
- [ ] `prefTitleTranscript`
- [ ] `prefIntroDescription1`
- [ ] `prefDescription1`
- [ ] `prefDescription2` — uwaga: rozbieżność między en.json a działającym kodem preference.js
- [ ] `prefDescription3` — uwaga: rozbieżność między en.json a działającym kodem preference.js
- [ ] `prefDescriptionNone` — uwaga: literówka w wyrazie „audiodeskrypcji”
- [ ] `prefDescFormatOption1` — puste; uwaga: puste, choć występowało w tłumaczeniu Stefana
- [ ] `prefDescFormatOption2` — puste; uwaga: puste, choć występowało w tłumaczeniu Stefana
- [ ] `prefIntroDescription3` — uwaga: błąd gramatyczny „formularza poniższej”
- [ ] `prefIntroDescription4`

## 04. Obsługa klawiatury i skróty (13)

- [ ] `prefIntroKeyboard1`
- [ ] `prefIntroKeyboard2`
- [ ] `prefIntroKeyboard3`
- [ ] `prefHeadingKeyboard1`
- [ ] `prefHeadingKeyboard2`
- [ ] `prefHeadingDescription`
- [ ] `prefHeadingTextDescription`
- [ ] `prefAltKey` — puste
- [ ] `prefCtrlKey` — puste
- [ ] `prefShiftKey` — puste
- [ ] `prefNoKeyShortcuts` — puste
- [ ] `escapeKey` — puste
- [ ] `escapeKeyFunction`

## 05. Odczytywanie audiodeskrypcji i transkrypcje (14)

- [ ] `prefDescPause`
- [ ] `prefDescVisible`
- [ ] `prefDescVoice`
- [ ] `prefDescRate` — puste
- [ ] `prefCaptionRate` — puste
- [ ] `prefDescPitch`
- [ ] `prefDescPitch1`
- [ ] `prefDescPitch2`
- [ ] `prefDescPitch3`
- [ ] `prefDescPitch4`
- [ ] `prefDescPitch5`
- [ ] `sampleDescriptionText`
- [ ] `prefHighlight`
- [ ] `prefTabbable`

## 06. Wygląd i prezentacja napisów (27)

- [ ] `prefCaptionsFont`
- [ ] `prefCaptionsColor`
- [ ] `prefCaptionsBGColor`
- [ ] `prefCaptionsSize`
- [ ] `prefCaptionsOpacity`
- [ ] `prefCaptionsStyle`
- [ ] `serif`
- [ ] `sans`
- [ ] `cursive`
- [ ] `fantasy`
- [ ] `monospace`
- [ ] `white`
- [ ] `yellow`
- [ ] `green`
- [ ] `cyan`
- [ ] `blue`
- [ ] `magenta`
- [ ] `red`
- [ ] `black`
- [ ] `transparent`
- [ ] `solid`
- [ ] `captionsStylePopOn` — uwaga: „Rozwiń” może błędnie określać sposób wyświetlania napisów
- [ ] `captionsStyleRollUp` — uwaga: „Zwiń” może błędnie określać sposób wyświetlania napisów
- [ ] `prefCaptionsPosition`
- [ ] `captionsPositionOverlay`
- [ ] `captionsPositionBelow`
- [ ] `sampleCaptionText`

## 07. Okna, przyciski i komunikaty (20)

- [ ] `prefSuccess`
- [ ] `prefNoChange`
- [ ] `save`
- [ ] `cancel`
- [ ] `dismissButton` — puste
- [ ] `windowButtonLabel`
- [ ] `windowMove`
- [ ] `windowMoveLeft` — puste
- [ ] `windowMoveRight` — puste
- [ ] `windowMoveUp` — puste
- [ ] `windowMoveDown` — puste
- [ ] `windowMoveStopped` — puste
- [ ] `transcriptControls` — puste
- [ ] `signControls` — puste
- [ ] `windowMoveAlert`
- [ ] `windowResize`
- [ ] `windowResizeHeading`
- [ ] `closeButtonLabel`
- [ ] `width`
- [ ] `height`

## 08. Wyszukiwanie i prezentacja czasu (11)

- [ ] `resultsSummary1`
- [ ] `resultsSummary2` — uwaga: polska odmiana po dynamicznej liczbie %1 wymaga kontroli
- [ ] `resultsSummary3`
- [ ] `noResultsFound`
- [ ] `searchButtonLabel`
- [ ] `hour`
- [ ] `minute`
- [ ] `second`
- [ ] `hours`
- [ ] `minutes`
- [ ] `seconds`

## 09. Video Transcript Sorter (VTS) (19)

- [ ] `vtsHeading` — puste
- [ ] `vtsInstructions1` — puste
- [ ] `vtsInstructions2` — puste
- [ ] `vtsInstructions3` — puste
- [ ] `vtsInstructions4` — puste
- [ ] `vtsInstructions5` — puste
- [ ] `vtsSelectLanguage` — puste
- [ ] `vtsSave` — puste
- [ ] `vtsReturn` — puste
- [ ] `vtsCancel` — puste
- [ ] `vtsRow` — puste
- [ ] `vtsKind` — puste
- [ ] `vtsStart` — puste
- [ ] `vtsEnd` — puste
- [ ] `vtsContent` — puste
- [ ] `vtsActions` — puste
- [ ] `vtsNewRow` — puste
- [ ] `vtsDeletedRow` — puste
- [ ] `vtsMovedRow` — puste

