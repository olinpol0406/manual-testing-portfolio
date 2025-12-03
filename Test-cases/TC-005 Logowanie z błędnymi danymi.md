TC-005 — Logowanie z błędnymi danymi

APLIKACJA: https://www.demoblaze.com

TESTOWANA FUNKCJONALNOŚĆ: Logowanie — walidacja błędnych danych

ŚRODOWISKO:
Przeglądarka: Google Chrome 141.0.7390.124  
System: Windows 10 Home, 64 bit  
Tryb: normalny  
Urządzenie: Laptop/Desktop

DATA: 2025-12-03  

TESTER: Olga

Identyfikator: TC-005


Warunki wstępne (preconditions):

- Strona https://www.demoblaze.com jest dostępna.
- Użytkownik znajduje się na stronie głównej.
- Użytkownik NIE posiada konta o nazwie testerFake2025.


Kroki testowe (steps):

1. Otwórz stronę https://www.demoblaze.com  
2. Kliknij przycisk "Log in"  
3. Wpisz login: testerFake2025 
4. Wpisz hasło: Test123  
5. Kliknij przycisk "Log in" 
6. Obserwuj komunikat na ekranie oraz zachowanie strony


Oczekiwany rezultat (expected result):

- Powinien pojawić się alert z informacją:  
  "User does not exist"
- System powinien pokazać informacje co jest niepoprawne (login lub hasło)
- Użytkownik NIE zostaje zalogowany.
- W prawym górnym rogu nadal widoczne są przyciski "Log in" / "Sign up".
- Brak przycisku "Log out".


Rzeczywisty rezultat (actual result):

- Zamiast jasnego komunikatu o błędzie, aplikacja wyświetla alert:  
  "User does not exist."
- Komunikat nie precyzuje czy błędny jes login, hasło czy oba pola
- Konsola DevTools pokazuje drobne ostrzeżenia (WAN/VIOLATION), brak poważnych błędów JS.


Status: FAIL


Uwagi / kroki dodatkowe:

- Sprawdzić w DevTools (F12 → Network) request login.  
- Sprawdzić, czy backend zwraca prawidłową odpowiedź.  
- Sprawdzić w Console, czy pojawiają się błędy JS.  
- Zrobić screenshot alertu i konsoli.


Priorytet / Severity:

- Priorytet: Medium  
- Severity: Minor  


Linki / dodatkowe pliki:

- Zrzut ekranu → Bug-reports/BR-003 Logowanie błąd.png
