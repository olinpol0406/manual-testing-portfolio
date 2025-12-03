BR-001 Błąd dodawania produktu do koszyka


ID błędu: BR-001
Moduł: Koszyk / Add to cart
Aplikacja: https://www.demoblaze.com
Data: 2025-11-19
Zgłaszający: Olga
Status: Otwarte (Open)


Opis błędu
Po kliknięciu przycisku "Add to cart" na stronie produktu, pojawia się alert „Product added”, jednak produkt zostaje zapisany w koszyku i nie pojawia się w zakładce "Cart".
W DevTools pojawia się błąd JavaScript: "Uncaught SyntaxError: Invalid or unexpected token".


Środowisko
Przeglądarka: Google Chrome 141.0.7390.124
System: Windows 10 Home, 64 bitTryb: normalny
Urządzenie: Laptop/Desktop


Warunki wstępne
Strona Demoblaze jest dostępna.
Użytkownik jest na stronie głównej.


Kroki do reprodukcji
Otwórz stronę https://www.demoblaze.com
Na liście produktów wybierz produkt, np. Samsung Galaxy S6
Na stronie produktu kliknij przycisk "Add to cart"
Potwierdź OK
Przejdź do zakładki "Cart"
Sprawdź listę produktów w koszyku


Oczekiwany rezultat
Produkt zostaje poprawnie dodany do koszyka
Produkt jest widoczny w zakładce "Cart"
Wyświetlają się prawidłowe dane: nazwa, cena, ilość


Rzeczywisty rezultat
Alert „Product added” pojawia się, ale produkt nie jest dodawany do koszyka
Koszyk pozostaje pusty
W DevTools → Console pojawia się błąd:
"Uncaught SyntaxError: Invalid or unexpected token"


Severity / Priority
Severity (Ważność): Critical – błąd uniemożliwia kluczową funkcję aplikacji
Priority (Priorytet): High – wymaga szybkiej naprawy


Załączniki
Screenshot błędu z konsoli:
BR-001 Błąd koszyka.png

Powiązany test case:
TC-001 Dodanie produktu do koszyka.md
