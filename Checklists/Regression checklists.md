META:
project: DemoBlaze
typ dokumentu: Regression Checklist
zakres: Kluczowe funkcjonalności po zmianach
tester: Olga (olinpol0406)
data: 2025-12-15
czas: 30 minut
narzędzia: Przeglądarka, DevTools

Regression Checklist – DemoBlaze

Celem testów regresji jest sprawdzenie, czy po zmianach w aplikacji
dotychczasowe funkcjonalności działają poprawnie.

1. Strona główna
- [v] Strona główna ładuje się poprawnie
- [v] Lista produktów wyświetla się poprawnie
- [v] Kliknięcie produktu otwiera jego szczegóły

2. Nawigacja
- [v] Menu działa poprawnie
- [v] Linki prowadzą do właściwych podstron
- [v] Logo przenosi na stronę główną
- [v] Brak błędów 404 podczas nawigacji

3. Produkty
- [v] Dane produktu są poprawne (nazwa, cena, opis)
- [v] Zdjęcia produktów ładują się poprawnie
- [nie dotyczy] Filtrowanie produktów
- [nie dotyczy] Sortowanie produktów

4. Koszyk
- [v] Można dodać produkt do koszyka
- [v] Koszyk aktualizuje licznik produktów
- [v] Zawartość koszyka wyświetla się poprawnie
- [v] Ceny i suma zamówienia liczą się poprawnie

5. Checkout
- [v] Formularz zamówienia otwiera się poprawnie
- [v] Można wypełnić dane w formularzu
- [v] Można złożyć zamówienie (Place Order)

6. Login / Signup
- [v] Formularz rejestracji działa poprawnie
- [v] Formularz logowania działa poprawnie
- [v] Poprawne dane umożliwiają logowanie
- [v] Niepoprawne dane wyświetlają komunikat błędu

7. Stabilność aplikacji
- [v] Brak błędów JavaScript w konsoli
- [v] Aplikacja nie zawiesza się podczas podstawowych akcji

Status testów regresji:
- [v] Brak regresji – kluczowe funkcjonalności działają poprawnie
