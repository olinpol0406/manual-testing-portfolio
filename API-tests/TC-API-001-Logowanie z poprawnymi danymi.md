Test Case ID: TC-API-001  
Nazwa: Logowanie z poprawnymi danymi
Endpoint: /login  
Metoda: POST  
Narzędzie: Postman  

Dane wejściowe:
{
  "username": "test_user",
  "password": "correct_password"
}

Kroki:
1. Otworzyć Postmana
2. Ustawić metodę POST
3. Wprowadzić endpoint /login
4. Wysłać żądanie z poprawnymi danymi logowania

Oczekiwany rezultat:
- Status HTTP: 200
- Brak komunikatu błędu
- Użytkownik zostaje zalogowany

Rzeczywisty rezultat:
- Status HTTP: 200
- Odpowiedź zgodna z implementacją DemoBlaze

Status testu:
PASS

