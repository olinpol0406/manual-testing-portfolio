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
- [v] Endpoint API odpowiada na żądanie
- [v] Brak błędów 5xx po stronie serwera
- [v] Odpowiedzi zwracane są w formacie JSON (lub puste response - zgodnie z implementacją Demoblaze)

2. Statusy HTTP
- [v] Poprawne żądania zwracają status 200
- [v] Brak statusow 4xx dla błędnego logowania, zgodnie z implementacją Demoblaze
- [v] Brak nieoczekiwanych statusów (np. 500)

3. Autoryzacja / Uwierzytelnienie
- [v] Rejestracja użytkownika działa poprawnie
- [v] Logowanie zwraca poprawną odpowiedź (status 200, zgodnie z implementacją)
- [v] Niepoprawne dane logowania zwracają Komunikat błędu (status 200, zgodnie z implementacją)
- [nie dotyczy] Brak dostępu do chronionych zasobów bez logowania 

4. Dane odpowiedzi
- [v] Odpowiedź zawiera wymagane pola (lub jest pusta, zgodnie z implementacją)
- [v] Typy danych są poprawne
- [nie dotyczy] Brak pustych lub nullowych pól
  
5. Obsługa błędów
- [v] API zwraca czytelne komunikaty błędów
- [v] Brak wrażliwych danych w komunikatach błędów
- [v] Błędy są spójne (format, treść)

6. Wydajność (podstawowa)
- [v] Odpowiedzi zwracane są w akceptowalnym czasie
- [v] Brak znacznych opóźnień przy prostych zapytaniach

7. Spójność danych
- [v] Dane zwracane przez API są zgodne z danymi w UI
- [v] Dodane dane są poprawnie zapisywane i zwracane

Status testów API:
- [v] API działa poprawnie

