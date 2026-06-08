# Bugi frontendowe – automotiveMastermind

Żeby wyróżnić się wśród kandydatów, przejrzałem frontend produktu pod kątem błędów, udokumentowałem je i tam, gdzie poprawka jest prosta, zaproponowałem rozwiązanie.

Stronę sprawdziłem na Chrome i Safari. Produkt działa na rynku USA, gdzie z Safari pochodzi 54% ruchu mobilnego i 30% desktopowego, więc zachowanie w tej przeglądarce ma tu realne znaczenie.

## Landing page

**1. Animowane slajdy.** Tekst i przyciski przenikają się podczas zmiany slajdu, zarówno z interwału, jak i po kliknięciu w stepper. Rozwiązanie: dodać krótką przerwę (~0,25 s) między zniknięciem a pojawieniem się kolejnego napisu i przycisków.

<!-- WIDEO: wklej tutaj link do nagrania (GitHub renderuje wgrane pliki .mp4 z URL-a) -->

**2. Odtwarzacz wideo.** Wideo nie jest wycentrowane. Mało istotne, widoczne w Safari na pierwszej klatce.

![Niewycentrowane wideo w Safari](ŚCIEŻKA_DO_ZRZUTU)

## Platform overview

**1. Zakładki (tabs).** Aktywny element chowa się pod elementem wyżej / w rodzicu. Rozwiązanie: poprawić `z-index`.

![Zakładka chowająca się pod elementem nadrzędnym](ŚCIEŻKA_DO_ZRZUTU)

**2. Nieładujący się obrazek.** "Failed to load image", widoczne szczególnie w Safari. Rozwiązanie: poprawić plik / ścieżkę do obrazka.

<table>
<tr>
<td><img src="ŚCIEŻKA_DO_ZRZUTU_1" width="100%"></td>
<td><img src="ŚCIEŻKA_DO_ZRZUTU_2" width="100%"></td>
</tr>
</table>

**3. Formularz.** Pole `select` ma inną wysokość niż pozostałe inputy na Safari. Rozwiązanie: Safari inaczej liczy padding przy `select`, więc warto ustawić mu sztywną wysokość (`height`). Formularz występuje na wielu stronach, więc poprawka jest warta uwagi.

![Select o innej wysokości niż inputy na Safari](ŚCIEŻKA_DO_ZRZUTU)

## Dealer case studies

**1. Zakładki (tabs).** Różny lewy padding między zakładkami. Rozwiązanie: ujednolicić.

<table>
<tr>
<td><img src="ŚCIEŻKA_DO_ZRZUTU_1" width="100%"></td>
<td><img src="ŚCIEŻKA_DO_ZRZUTU_2" width="100%"></td>
</tr>
</table>

## Blog post

**1. Zdjęcia.** Dodatkowy whitespace wokół zdjęć i brak możliwości kliknięcia w nie. Rozwiązanie do opracowania, ale proste.

![Zdjęcia z dodatkowym whitespace](ŚCIEŻKA_DO_ZRZUTU)
