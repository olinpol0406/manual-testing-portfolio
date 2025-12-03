BR-003 — Nieczytelny komunikat błędu przy logowaniu niepoprawnymi danymi

Identyfikator: BR-003  
Zgłosił: Olga  
Data: 2025-12-03

---

## Aplikacja:
https://www.demoblaze.com

## Środowisko:
- Przeglądarka: Google Chrome 141.0.7390.124  
- System: Windows 10 Home, 64 bit  
- Urządzenie: Laptop/Desktop  
- Tryb: normalny  

---

## Opis błędu:
Podczas próby logowania nieistniejącym użytkownikiem aplikacja wyświetla zbyt ogólny komunikat: *„User does not exist.”*  
Komunikat nie określa, czy błąd dotyczy loginu, hasła, czy obu pól, co jest niezgodne z dobrymi praktykami UX.

---

## Kroki do reprodukcji (steps to reproduce):
1. Otwórz https://www.demoblaze.com  
2. Kliknij *“Log in”*  
3. Wpisz login: fake_user_123  
4. Wpisz hasło: Test1234!  
5. Kliknij przycisk *“Log in”*  
6. Zaobserwuj alert i zachowanie UI  

---

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
