META:
project: Demollaze
typ dokumentu: API Checklist
zakres: Podstawowe endpointy API aplikacji
tester: Olga (olinpol0406)
data: 2025-12-15
narzędzia: DevTools (Network), Postman

API Checklist – DemoBlaze

Celem testów API jest sprawdzenie poprawności działania podstawowych endpointów,
ich odpowiedzi, statusów HTTP oraz poprawnej obsługi błędów.

1. Dostępność API
- [ ] Endpoint API odpowiada na żądanie
- [ ] Brak błędów 5xx po stronie serwera
- [ ] Odpowiedzi zwracane są w formacie JSON

2. Statusy HTTP
- [ ] Poprawne żądania zwracają status 200
- [ ] Niepoprawne żądania zwracają status 4xx
- [ ] Brak nieoczekiwanych statusów (np. 500)

3. Autoryzacja / Uwierzytelnienie
- [ ] Rejestracja użytkownika działa poprawnie
- [ ] Logowanie zwraca poprawną odpowiedź
- [ ] Niepoprawne dane logowania zwracają błąd
- [ ] Brak dostępu do chronionych zasobów bez logowania (jeśli dotyczy)

4. Dane odpowiedzi
- [ ] Odpowiedź zawiera wymagane pola
- [ ] Typy danych są poprawne
- [ ] Brak pustych lub nullowych pól (jeśli nie powinny występować)

5. Obsługa błędów
- [ ] API zwraca czytelne komunikaty błędów
- [ ] Brak wrażliwych danych w komunikatach błędów
- [ ] Błędy są spójne (format, treść)

6. Wydajność (podstawowa)
- [ ] Odpowiedzi zwracane są w akceptowalnym czasie
- [ ] Brak znacznych opóźnień przy prostych zapytaniach

7. Spójność danych
- [ ] Dane zwracane przez API są zgodne z danymi w UI
- [ ] Dodane dane są poprawnie zapisywane i zwracane

Status testów API:
- [ ] API działa poprawnie
- [ ] API zawiera błędy wymagające zgłoszenia
