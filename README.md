*English version below ([jump to it](#automotivemastermindcom---cosmetic-bugs)).*

# automotivemastermind.com - kosmetyczne bugi

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

---

# automotivemastermind.com - cosmetic bugs

I tested the site on Chrome and Safari. The product runs in the US market, where Safari accounts for 54% of mobile and 30% of desktop traffic, so how it behaves there actually matters.

## Landing page

**1. Animated slides.** The text and buttons overlap during a slide change, both on the interval and after clicking the stepper. Fix: add a short pause (~0.25s) between the old copy/buttons fading out and the next ones appearing.

![Video](https://github.com/dlipinski/automotivemastermind-frontend-bugs/raw/refs/heads/main/Landing%20page/Slide%20show.mov)

**2. Video player.** The video isn't centered. Minor, visible in Safari on the first frame.

![Off-center video in Safari](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Landing%20page/Video%20player.png?raw=true)

## Platform overview

**1. Tabs.** The active element hides behind the one above it / in the parent. Fix: correct the `z-index`.

![Tab hidden behind the parent element](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Tabs.png?raw=true)

**2. Image not loading.** "Failed to load image", especially in Safari. Fix: correct the file / image path.

<table>
<tr>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Image-1.png?raw=true" width="100%"></td>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Image-2.png?raw=true" width="100%"></td>
</tr>
</table>

**3. Form.** The `select` field has a different height than the other inputs in Safari. Fix: Safari handles padding on `select` differently, so it's worth giving it a fixed `height`. The form appears on several pages, so it's worth a look.

![Select with a different height than the inputs in Safari](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Platform%20overview/Form.png?raw=true)

## Dealer case studies

**1. Tabs.** Inconsistent left padding between tabs. Fix: make it uniform.

<table>
<tr>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Dealer%20case%20studies/Tab-1.png?raw=true" width="100%"></td>
<td><img src="https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Dealer%20case%20studies/Tab-2.png?raw=true" width="100%"></td>
</tr>
</table>

## Blog post

**1. Photos.** Extra whitespace around the photos and you can't click them. Fix still to be worked out, but simple.

![Photos with extra whitespace](https://github.com/dlipinski/automotivemastermind-frontend-bugs/blob/main/Blog%20post/Post%20photos.png?raw=true)
