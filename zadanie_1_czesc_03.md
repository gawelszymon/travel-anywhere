## Jako turysta*podróżnik wybierający się do punktu Lon1, Lat1 chciałbym wiedzieć gdzie znajduje się najbliższe
## lotnisko i najbliższa wypożyczalnia samochodów (względem mojego miejsca docelowego). 

### tablica 2x2 skladajaca sie z kolumn
* znajduje najblizsze lotnisko i najblizsza wyporzyczalnie
* znajduje nablizasze ltonisko i nie znajduje najblizszej wyporzyczlanie
* nie znajduje najblizszsego lotniska i znajduja najblizsza wyporzyczalnie
* nie znajduje najblizszego lotnika i nie znajduje najblizszej wyporzyczalnie

---

* identyfikator: znajduje najblizsze lotnisko i najblizsza wyporzyczalnie
* warunki wejściowe: uruchom aplikacje
* kroki testowe:
  * zaloguj sie do aplikcji podajac dolaczony do dokumentacji klucz api
  * poczekaj na zaladowanie sie mapy
  * w polach filtracji typu "checkbox" odznacz wszystkie niepotrzebne opcje (zaznaczony powinien byc lotnisko i wypozyczalnie samochodow)
  * kliknij w losowy punkt na mapie
* oczekiwany rezultat
  * aplikacja zwraca zarowno punkty dla lotniska i wyporzyczalni (pokrytym przez zadeklarowany w dokumentacji promien r), poprzez analize api lub google maps weryfikujemy czy zaznaczone punkty faktycznie sa najblizsze

---
 
* identyfikator: znajduje nablizasze ltonisko i nie znajduje najblizszej wyporzyczlanie
* warunki wejściowe: uruchom aplikacje
* kroki testowe:
	* zaloguj sie do aplikcji podajac dolaczony do dokumentacji klucz api
	* poczekaj na zaladowanie sie mapy
	* w polach filtracji typu "checkbox" odznacz wszystkie niepotrzebne opcje (zaznaczony powinien byc lotnisko i wypozyczalnie samochodow)
	* kliknij w losowy punkt na mapie
* oczekiwany rezulta:
	* aplikacja zwraca tylko punkt dla lotniska (pokrytym przez zadeklarowany w dokumentacji promien r), poprzez analize api lub google maps weryfikujemy czy zaznaczony punkt faktycznie jest najblizszy, natomiast dla wyporzyczalni aplikacja nie zwraca zadnego punktu lub wyswietla komunikat o braku wynikow w promieniu r

---

* identyfikator: nie znajduje najblizszsego lotniska i znajduja najblizsza wyporzyczalnie
* warunki wejściowe: uruchom aplikacje
* kroki testowe:
	* zaloguj sie do aplikcji podajac dolaczony do dokumentacji klucz api
	* poczekaj na zaladowanie sie mapy
	* w polach filtracji typu "checkbox" odznacz wszystkie niepotrzebne opcje (zaznaczony powinien byc lotnisko i wypozyczalnie samochodow)
	* kliknij w losowy punkt na mapie
* oczekiwany rezultat
	* aplikacja zwraca tylko punkt dla wyporzyczalni (pokrytym przez zadeklarowany w dokumentacji promien r), poprzez analize api lub google maps weryfikujemy czy zaznaczony punkt faktycznie jest najblizszy, natomiast dla lotniska aplikacja nie zwraca zadnego punktu lub wyswietla komunikat o braku wynikow w promieniu r

---

* identyfikator: nie znajduje najblizszego lotnika i nie znajduje najblizszej wyporzyczalnie
* warunki wejściowe: uruchom aplikacje
* kroki testowe:
	* zaloguj sie do aplikcji podajac dolaczony do dokumentacji klucz api
	* poczekaj na zaladowanie sie mapy
	* w polach filtracji typu "checkbox" odznacz wszystkie niepotrzebne opcje (zaznaczony powinien byc lotnisko i wypozyczalnie samochodow)
	* kliknij w losowy punkt na mapie
* oczekiwany rezultat
	* aplikacja nie zwraca zadnych punktow na mapie ani dla lotniska, ani dla wyporzyczalni, poprzez analize api lub google maps weryfikujemy czy w zadeklarowanym w dokumentacji promieniu r faktycznie nie znajduje sie zaden z tych obiektow (aplikacja moze wyswietlic komunikat o braku wynikow wyszukiwania)
Jeśli chcesz, możemy teraz do tych przypadków dopisać asercje techniczne API (np. oczekiwane kody statusów HTTP lub strukturę JSON) albo stworzyć przypadki negatywne, np. dla sytuacji, gdy użytkownik poda błędny klucz API lub współrzędne spoza zakresu geograficznego. Nad czym pracujemy dalej?
