TC-002 — Usuwanie produktu z koszyka


APLIKACJA: https://www.demoblaze.com


TESTOWANA FUNKCJONLNOŚĆ: Usuwanie produktu z koszyka


ŚRODOWISKO: Przeglądarka: Google Chrome 141.0.7390.124 System: Windows 10 Home, 64 bit Tryb: normalny Urządzenie: Laptop/Desktop


DATA: 2025-11-24


TESTER: Olga


Identyfikator TC-002



Cel testu Sprawdzić, czy użytkownik może usunąć produkt dodany wcześniej do koszyka.

Warunki wstępne (preconditions)

Strona Demoblaze jest dostępna (https://www.demoblaze.com).
Użytkownik dodał przynajmniej jeden produkt do koszyka np. Samsung Galaxy S6.

Kroki testowe (steps)

Otwórz stronę https://www.demoblaze.com
Na liście produktów kliknij produkt np. Samsung Galaxy S6.
Na stronie produktu kliknij przycisk Add to cart.
Potwierdź OK, (jeśli się pojawi).
Kliknij w górnym menu Cart (Koszyk).
Na liście produktów w koszyku kliknij "Delete" lub "Usuń"
Jeśli nie nastąpiła automatyczna aktualizacja odśwież stronę
Sprawdź listę produktów w koszyku.


Oczekiwany rezultat (expected result)

Produkt zostaje usunięty z koszyka.
Cena i ilość produktu aktualizują się.
Po odświeżeniu produkt nie jest widoczny w koszyku.


Rzeczywisty rezultat (actual result)

Po kliknięciu "Add to cart" pojawia się alert "Product added" ale produkt nie pojawia się w koszyku.
Status FAIL

Uwagi / kroki dodatkowe

Jeśli alert nie pojawił się, otwórz DevTools (F12) → Console i Network i sprawdź błędy.
W DevTools - Console pojawił się błąd: Uncaught SyntaxError: Unexpected token '<'.
Błąd pojawia się natychmiast po naciśnięciu przycisku "Add to cart".
Po odświeżeniu strony problem nadal występuje — produkt nie dodaje się do koszyka.
Priorytet / Severity

Priorytet: High
Severity: Critical
Linki / dodatkowe pliki

Zrzut ekranu - Bug-reports/BR-001 Błąd koszyka.png
