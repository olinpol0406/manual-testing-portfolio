TC-002 — Zakładanie nowego konta użytkownika

APLIKACJA: https://www.demoblaze.com  

TESTOWANA FUNKCJONALNOŚĆ: Rejestracja nowego użytkownika  

ŚRODOWISKO: Przeglądarka: Google Chrome 141.0.7390.124, System: Windows 10 Home, 64 bit, Tryb: normalny, Urządzenie: Laptop/Desktop  

DATA: 2025-12-03  

TESTER: Olga  

Identyfikator TC: TC-002

Warunki wstępne (preconditions):

- Strona Demoblaze jest dostępna (https://www.demoblaze.com).  
- Użytkownik jest na stronie głównej.  
- Użytkownik nie posiada jeszcze konta z danym loginem.  

Kroki testowe (steps):

1. Otwórz stronę https://www.demoblaze.com  
2. Kliknij „Sign up” w prawym górnym rogu.  
3. W oknie modalnym wpisz unikalną nazwę użytkownika (np. test_user_2025)  
4. Wpisz poprawne hasło (np. Test1234!).  
5. Kliknij przycisk „Sign up”.  
6. Zatwierdź komunikat potwierdzający (OK).  

Oczekiwany rezultat (expected result):

- Wyświetla się komunikat potwierdzający pomyślną rejestrację („Sign up successful”).  
- Po ponownym otwarciu okna „Sign up” login nie może być użyty ponownie (np. komunikat „This user already exists”).

Rzeczywisty rezultat (actual result):

- Rejestracja przebiega prawidłowo, użytkownik otrzymuje komunikat potwierdzający.

Status: PASS  

Uwagi / kroki dodatkowe:

- Sprawdzić w DevTools (F12 → Network), czy wysyłane jest poprawne zapytanie signup.  
- W przypadku FAIL należy zweryfikować, czy login jest naprawdę unikalny.

Priorytet / Severity:

- Priorytet: High  
- Severity: Major  

Linki / dodatkowe pliki:

- Zrzut ekranu — Bug-reports/BR-002 Rejestracja.png
