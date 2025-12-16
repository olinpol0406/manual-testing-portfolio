
Test Case ID: TC-API-002  
Nazwa: Logowanie z błędnym hasłem
Endpoint: /login  
Metoda: POST  
Narzędzie: Postman  

Dane wejściowe:
{
  "username": "testerolga2025",
  "password": "Test123xd"
}

Kroki:
1. Otworzyć Postmana
2. Ustawić metodę POST
3. Wprowadzić endpoint /login
4. Wysłać żądanie z błędnym hasłem

Oczekiwany rezultat:
- Status HTTP: 200
- Komunikat o błędnych danych logowania

Rzeczywisty rezultat:
- Status HTTP: 200
- Komunikat błędu zwrócony w odpowiedzi

Status testu:
PASS

