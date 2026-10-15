# Jako turysta-podróżnik wybierający się do punktu Lon2, Lat2 chciałbym wiedzieć gdzie znajduje się najbliższy hotel.

- identyfikator testu: Jako uzytkownik, aplikacja nie zwrocila mi zadnego hotelu
- warunki wejściowe: uruchom aplikacje
- kroki testowe:
  - zaloguj sie do aplikcji podajac dolaczony do dokumentacji klucz api
  - poczekaj na zaladowanie sie mapy
  - w polach filtracji typu "checkbox" odznacz wszystkie niepotrzebne opcje (zaznaczony powinien byc tylko hotel)
  - kliknij w losowy punkt na mapie
- oczekiwany rezultat
  - aplikacja nie zwrocila zadnego punktu, powniewaz w danym obszarze (pokrytym przez zadeklarowany w dokumentacji promien r) faktycznie nie ma zadnego hotelu
