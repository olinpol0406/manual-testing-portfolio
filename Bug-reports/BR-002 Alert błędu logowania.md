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


Oczekiwany rezultat

Czytelny, precyzyjny komunikat błędu, np.: „Nieprawidłowy login” lub „Użytkownik nie istnieje w systemie”  
UI powinno jasno wskazywać, co użytkownik zrobił źle.  
Brak logowania użytkownika (UI pozostaje bez zmian).  


Rzeczywisty rezultat:

Wyświetlany jest tylko ogólny alert: „User does not exist.” 
Brak wyjaśnienia, co dokładnie jest nieprawidłowe.  
Po zamknięciu alertu UI nie przekazuje dalszych informacji.  
W DevTools → Console widoczne są drobne ostrzeżenia (WARN/VIOLATION), brak poważnych błędów JS.


Severity / Priority

Severity: Minor  
Priorytet: Medium  


Załączniki

Screenshot błędu z konsoli: BR-002 Błąd logowania.png

Powiązany test case: TC-005 Dodanie produktu do koszyka.md













---

## Status:
Open

---

## Proponowane rozwiązanie:
- Ulepszyć komunikat błędu tak, aby był bardziej precyzyjny.  
- Dodać walidację po stronie front-end (komunikat pod polem login/hasło).  
- Usprawnić logowanie błędów po stronie serwera (czytelne odpowiedzi API).
