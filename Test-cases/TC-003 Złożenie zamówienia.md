TC-003 — Złożenie zamówienia (Place Order)



---

## 🎯 Cel testu
Zweryfikować poprawność i kompletność procesu złożenia zamówienia: dodanie produktu do koszyka, otwarcie formularza Place Order, wypełnienie danych, złożenie zamówienia i potwierdzenie transakcji.

---

## 🧩 Warunki wstępne (Preconditions)
- Strona Demoblaze jest dostępna.  
- Użytkownik ma co najmniej jeden produkt w koszyku (jeśli nie — dodać produkt przed krokiem 1).

---

## 📝 Kroki testowe (Steps)
1. Otwórz stronę https://www.demoblaze.com  
2. Na liście produktów wybierz produkt (np. Samsung Galaxy S6) i kliknij *Add to cart* → potwierdź alert.  
3. Kliknij w górnym menu *Cart* (Koszyk).  
4. Kliknij przycisk *Place Order*.  
5. W formularzu zamówienia wypełnij pola: *Name*, *Country*, *City*, *Credit card*, *Month*, *Year* (np. Jan Kowalski / Poland / Warsaw / 4111 1111 1111 1111 / 12 / 2026).  
6. Kliknij *Purchase*.  
7. Poczekaj na modal/okno potwierdzenia z informacją o transakcji (np. numer zamówienia, kwota).  
8. Zrób screenshot potwierdzenia (dla archiwum).  
9. Zamknij modal potwierdzenia.  
10. Sprawdź stan koszyka (powinien być pusty lub zgodnie z oczekiwaniami aplikacji).

---

## ✔ Oczekiwany rezultat (Expected result)
- Formularz zamówienia pojawia się po kliknięciu *Place Order*.  
- Po kliknięciu *Purchase* pojawia się potwierdzenie zawierające id zamówienia i kwotę.  
- Kwota w potwierdzeniu odpowiada sumie produktów w koszyku.  
- Po zamknięciu potwierdzenia koszyk jest pusty (o ile aplikacja tak zakłada).

---

## ❌ Rzeczywisty rezultat (Actual result)
- (wypełnić podczas testu)

*Status:*
(TBD — PASS / FAIL)

---

## 🧪 Uwagi / Kroki dodatkowe
- Przy problemach zanotuj komunikaty błędów i logi z DevTools (Console/Network).  
- Jeśli formularz nie waliduje poprawnie pól, zapisz które pola akceptują niepoprawne dane.  
- Dołącz screenshot potwierdzenia do raportów.

---

## 🔥 Priorytet / Severity
- *Priority:* High  
- *Severity:* Major / Critical
