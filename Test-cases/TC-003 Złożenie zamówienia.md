TC-003 — Złożenie zamówienia (Place Order)

APLIKACJA: https://www.demoblaze.com

TESTOWANA FUNKCJONLNOŚĆ: Usuwanie produktu z koszyka

ŚRODOWISKO: Przeglądarka: Google Chrome 141.0.7390.124 System: Windows 10 Home, 64 bit Tryb: normalny Urządzenie: Laptop/Desktop

DATA: 2025-11-24

TESTER: Olga

Identyfikator TC-003


Cel testu
Zweryfikować poprawność procesu złożenia zamówienia: dodanie produktu do koszyka, otwarcie formularza Place Order, wypełnienie danych, złożenie zamówienia i potwierdzenie transakcji.


 Warunki wstępne (Preconditions)
- Strona Demoblaze jest dostępna.  
- Użytkownik ma co najmniej jeden produkt w koszyku.


Kroki testowe (Steps)
1. Otwórz stronę https://www.demoblaze.com  
2. Na liście produktów wybierz produkt (np. Samsung Galaxy S6) i kliknij "Add to cart".  
3. Kliknij w górnym menu "Cart" (Koszyk).  
4. Kliknij przycisk "Place Order".  
5. W formularzu zamówienia wypełnij wymagane pola.
6. Kliknij "Purchase".  
7. Poczekaj na okno potwierdzenia z informacją o transakcji (np. numer zamówienia, kwota).  
8. Zrób screenshot potwierdzenia.  
9. Zamknij okno potwierdzenia.  
10. Sprawdź stan koszyka (powinien być pusty).


Oczekiwany rezultat (Expected result)
- Formularz zamówienia pojawia się po kliknięciu "Place Order".  
- Po kliknięciu "Purchase" pojawia się potwierdzenie zawierające id zamówienia i kwotę.  
- Kwota w potwierdzeniu odpowiada sumie produktów w koszyku.  
- Po zamknięciu potwierdzenia koszyk jest pusty.


Rzeczywisty rezultat = Oczekiwany rezultat


Status PASS
