TC-001 — Dodanie produktu do koszyka

APLIKACJA: https://www.demoblaze.com  

TESTOWANA FUNKCJONLNOŚĆ: Dodawanie produktu do koszyka  

ŚRODOWISKO:
Przeglądarka: Google Chrome 141.0.7390.124 
System: Windows 10 Home, 64 bit
Tryb: normalny
Urządzenie: Laptop/Desktop 

DATA: 2025-11-19  

TESTER: Olga


Identyfikator
TC-001

Cel testu
Sprawdzić, czy użytkownik może dodać produkt do koszyka i czy produkt widoczny jest w koszyku.

Warunki wstępne (preconditions)
- Strona Demoblaze jest dostępna (https://www.demoblaze.com).  
- Użytkownik jest na stronie głównej.

Kroki testowe (steps)
1. Otwórz stronę https://www.demoblaze.com  
2. Na liście produktów kliknij produkt np. Samsung Galaxy S6.  
3. Na stronie produktu kliknij przycisk Add to cart.  
4. Potwierdź OK, (jeśli się pojawi).  
5. Kliknij w górnym menu Cart (Koszyk).  
6. Sprawdź listę produktów w koszyku.

Oczekiwany rezultat (expected result)
- Po kliknięciu "Add to cart" pojawia się alert potwierdzający (np. "Product added").  
- W koszyku powinna pojawić się pozycja z nazwą wybranego produktu (np. Samsung galaxy s6).  
- Cena i ilość produktu są poprawnie wyświetlone.

Rzeczywisty rezultat (actual result)
- Po kliknięciu "Add to cart" pojawia się alert "Product added" ale produkt nie pojawia się w koszyku.
  
Status
  FAIL 

Uwagi / kroki dodatkowe
- Jeśli alert nie pojawił się, otwórz DevTools (F12) → Console i Network i sprawdź błędy.
- W DevTools - Console pojawił się błąd: Uncaught SyntaxError: Unexpected token '<'.
- Błąd pojawia się natychmiast po naciśnięciu przycisku "Add to cart".
- Po odświeżeniu strony problem nadal występuje — produkt nie dodaje się do koszyka.

Priorytet / Severity
- Priorytet: High 
- Severity: Critical

Linki / dodatkowe pliki
- Zrzut ekranu - Bug-reports/BR-001 Błąd koszyka.png
