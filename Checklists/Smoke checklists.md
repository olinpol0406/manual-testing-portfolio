META: 
project: Demoblaze 
typ dokumentu: Smoke Checklist 
zakres: Kluczowe funkcje aplikacji 
tester: Olga (olinpol0406) 
data: 2025-12-04 
czas: 30 minutes

UI Checklist — Demoblaze

Celem testów smoke jest szybkie sprawdzenie, czy aplikacja działa w podstawowym zakresie
i czy można ją poddać dalszym testom.

1. Strona główna
- [v ] Strona główna otwiera się bez błędów
- [v ] Lista produktów wyświetla się poprawnie
- [v ] Można przejść do szczegółów produktu

2. Nawigacja
- [v ] Wszystkie linki w menu działają
- [v ] Logo przenosi na stronę główną

3. Koszyk
- [v ] Można dodać produkt do koszyka
- [v ] Licznik koszyka aktualizuje się poprawnie
- [v ] Można wyświetlić zawartość koszyka

4. Zakup / Checkout
- [v ] Przycisk „Place Order” otwiera formularz
- [v ] Można wpisać dane do formularza
- [v ] Można wysłać formularz (Place Order)

5. Login / Signup
- [v ] Formularz Signup otwiera się
- [v ] Można wpisać dane
- [v ] Można wysłać formularz Signup
- [v ] Formularz Login otwiera się
- [v ] Login działa poprawnie z istniejącymi danymi (konto testowe)
- [v ] Niepoprawne dane wyświetlają błąd (alert)

6. Podstawowa stabilność
- [v ] Brak błędów 404 podczas nawigacji
- [v ] Brak błędów JavaScript w konsoli (F12 → Console)

Status testów smoke:
- [v ] Aplikacja stabilna  
- [ ] Aplikacja niestabilna — wymaga zgłoszenia błędów
      
