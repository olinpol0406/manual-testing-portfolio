
Test Case ID: TC-API-003  
Nazwa: Rejestracja ustniejącego uzytkownika
Endpoint: /signup  
Metoda: POST  
Narzędzie: Postman  

Dane wejściowe:
{
  "username": "testerOlga2025",
  "password": "123456"
}

Kroki:
1. Otworzyć Postmana
2. Ustawić metodę POST
3. Wprowadzić endpoint /signup
4. Wysłać żądanie z loginem, który już istnieje

Oczekiwany rezultat:
- Status HTTP: 200
- Komunikat informujący, że użytkownik już istnieje

Rzeczywisty rezultat:
- Status HTTP: 200
- Komunikat błędu zwrócony w odpowiedzi

Status testu:
PASS
