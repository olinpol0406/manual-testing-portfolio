TC-API-002 – Logowanie z błędnym hasłem

Test Case ID: TC_API_02  
Nazwa: Logowanie użytkownika – błędne hasło  
Endpoint: /login  
Metoda: POST  
Narzędzie: Postman  

Dane wejściowe:
{
  "username": "test_user",
  "password": "wrong_password"
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

