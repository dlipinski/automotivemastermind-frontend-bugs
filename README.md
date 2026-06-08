# Bugi frontendowe – automotiveMastermind

Żeby wyróżnić się wśród kandydatów, przejrzałem frontend produktu pod kątem błędów, udokumentowałem je i tam, gdzie poprawka jest prosta, zaproponowałem rozwiązanie.

Stronę sprawdziłem na Chrome i Safari. Produkt działa na rynku USA, gdzie z Safari pochodzi 54% ruchu mobilnego i 30% desktopowego, więc zachowanie w tej przeglądarce ma tu realne znaczenie.

## Landing page

**1. Animowane slajdy.** Tekst i przyciski przenikają się podczas zmiany slajdu, zarówno z interwału, jak i po kliknięciu w stepper. Rozwiązanie: dodać krótką przerwę (~0,25 s) między zniknięciem a pojawieniem się kolejnego napisu i przycisków.

![Video](https://github.com/dlipinski/automotivemastermind-frontend-bugs/raw/refs/heads/main/Landing%20page/Slide%20show.mov)

**2. Odtwarzacz wideo.** Wideo nie jest wycentrowane. Mało istotne, widoczne w Safari na pierwszej klatce.

![Niewycentrowane wideo w Safari](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Landing%20page/Video%20player.png?raw=true)

## Platform overview

**1. Zakładki (tabs).** Aktywny element chowa się pod elementem wyżej / w rodzicu. Rozwiązanie: poprawić `z-index`.

![Zakładka chowająca się pod elementem nadrzędnym](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Tabs.png?raw=true)

**2. Nieładujący się obrazek.** "Failed to load image", widoczne szczególnie w Safari. Rozwiązanie: poprawić plik / ścieżkę do obrazka.

<table>
<tr>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Image-1.png?raw=true" width="100%"></td>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Image-2.png?raw=true" width="100%"></td>
</tr>
</table>

**3. Formularz.** Pole `select` ma inną wysokość niż pozostałe inputy na Safari. Rozwiązanie: Safari inaczej liczy padding przy `select`, więc warto ustawić mu sztywną wysokość (`height`). Formularz występuje na wielu stronach, więc poprawka jest warta uwagi.

![Select o innej wysokości niż inputy na Safari](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Form.png?raw=true)

## Dealer case studies

**1. Zakładki (tabs).** Różny lewy padding między zakładkami. Rozwiązanie: ujednolicić.

<table>
<tr>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Dealer%20case%20studies/Tab-1.png?raw=true" width="100%"></td>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Dealer%20case%20studies/Tab-2.png?raw=true" width="100%"></td>
</tr>
</table>

## Blog post

**1. Zdjęcia.** Dodatkowy whitespace wokół zdjęć i brak możliwości kliknięcia w nie. Rozwiązanie do opracowania, ale proste.

![Zdjęcia z dodatkowym whitespace](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Blog%20post/Post%20photos.png?raw=true)
