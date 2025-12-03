BR-002 Nieczytelny komunikat błędu przy logowaniu niepoprawnymi danymi


Identyfikator: BR-001 
Moduł: Logowanie / Login form 
Aplikacja: https://www.demoblaze.com 
Data: 2025-12-03
Zgłaszający: Olga 
Status: Otwarte (Open)


Opis błędu

Podczas próby logowania nieistniejącym użytkownikiem aplikacja wyświetla zbyt ogólny komunikat: *„User does not exist.”*  
Komunikat nie określa, czy błąd dotyczy loginu, hasła, czy obu pól, co jest niezgodne z dobrymi praktykami UX


Środowisko

Przeglądarka: Google Chrome 141.0.7390.124
System: Windows 10 Home, 64 bit
Tryb: normalny
Urządzenie: Laptop/Desktop


Warunki wstępne

Strona Demoblaze jest dostępna.
Użytkownik jest na stronie głównej.


Kroki do reprodukcji

Otwórz https://www.demoblaze.com  
Kliknij “Log in”* 
Wpisz login: testerFake2025
Wpisz hasło: Test123  
Kliknij przycisk “Log in” 
Zaobserwuj alert i zachowanie interfejsu użytkownika 


Rzeczywisty rezultat

Alert „Product added” pojawia się, ale produkt nie jest dodawany do koszyka

Koszyk pozostaje pusty

W DevTools → Console pojawia się błąd: "Uncaught SyntaxError: Invalid or unexpected token"

Severity / Priority

Severity (Ważność): Critical – błąd uniemożliwia kluczową funkcję aplikacji

Priority (Priorytet): High – wymaga szybkiej naprawy

Załączniki

Screenshot błędu z konsoli: BR-001 Błąd koszyka.png

Powiązany test case: TC-001 Dodanie produktu do koszyka.md


mmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmm








## Oczekiwany rezultat:
- Czytelny, precyzyjny komunikat błędu, np.:  
  - „Nieprawidłowy login”  
  - „Użytkownik nie istnieje w systemie”  
- UI powinno jasno wskazywać, co użytkownik zrobił źle.  
- Brak logowania użytkownika (UI pozostaje bez zmian).  

---

## Rzeczywisty rezultat:
- Wyświetlany jest tylko ogólny alert: *„User does not exist.”*  
- Brak wyjaśnienia, co dokładnie jest nieprawidłowe.  
- Po zamknięciu alertu UI nie przekazuje dalszych informacji.  
- W DevTools → Console widoczne są drobne ostrzeżenia (WARN/VIOLATION),  
  ale *brak poważnych błędów JS*.

---

## Załączniki / Dowody:
- Screenshot alertu → Bug-reports/BR-003 Logowanie błąd alert.png  
- Screenshot DevTools (opcjonalnie)  

---

## Priorytet / Severity:
- *Priorytet:* Medium  
- *Severity:* Minor  

---

## Status:
Open

---

## Proponowane rozwiązanie:
- Ulepszyć komunikat błędu tak, aby był bardziej precyzyjny.  
- Dodać walidację po stronie front-end (komunikat pod polem login/hasło).  
- Usprawnić logowanie błędów po stronie serwera (czytelne odpowiedzi API).
