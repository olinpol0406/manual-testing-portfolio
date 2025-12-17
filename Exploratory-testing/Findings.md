ET-001 – Test eksploracyjny: Logowanie użytkownika

Obserwacja 1: – brak walidacji po stronie UI
Formularz logowania umożliwia wysłanie pustych danych
bez wcześniejszej walidacji po stronie interfejsu użytkownika.

Obserwacja 2: – mało precyzyjny komunikat
Komunikat błędu po nieudanym logowaniu nie informuje,
czy problem dotyczy loginu czy hasła.

Ryzyko – brak limitu prób logowania
Brak widocznego mechanizmu ograniczającego liczbę nieudanych prób logowania,
co w realnej aplikacji może prowadzić do prób ataków brute force.

Pomysł na dalsze testy
Sprawdzenie zachowania aplikacji po wielu nieudanych próbach logowania
oraz analiza odpowiedzi API w takich przypadkach.




ET-002 - Test eksploracyjny: Proces zakupowy

Obserwacja 1: – brak walidacji danych w formularzu zamówienia
Formularz składania zamówienia umożliwia wysłanie pustych lub
niekompletnych danych bez wcześniejszej walidacji po stronie interfejsu użytkownika.

Obserwacja 2 – brak jednoznacznego potwierdzenia złożenia zamówienia
Po zatwierdzeniu zamówienia komunikat potwierdzający nie zawiera
szczegółowych informacji dotyczących zamówienia, takich jak lista produktów
czy całkowita kwota.

Obserwacja 3 – możliwość wielokrotnego zatwierdzenia zamówienia
Wielokrotne kliknięcie przycisku potwierdzającego zamówienie
może prowadzić do niejednoznacznego zachowania aplikacji.

Ryzyko – niepoprawne przetwarzanie zamówień
Brak walidacji danych oraz jednoznacznego potwierdzenia zamówienia
może w realnej aplikacji prowadzić do błędnych lub zdublowanych zamówień.

Pomysł na dalsze testy
Sprawdzenie zachowania aplikacji przy wielokrotnym składaniu zamówienia
oraz analiza odpowiedzi API odpowiedzialnych za tworzenie zamówień.




ET003 - Test eksploracyjny: Nawigacja UX

Obserwacja 1: - brak wyraźnej informacji o aktualnym kontekście
Podczas nawigacji między kategoriami produktów nie zawsze jest jasne,
w jakiej kategorii aktualnie znajduje się użytkownik.

Obserwacja 2 – Ograniczona informacja zwrotna po akcjach użytkownika
Po wykonaniu niektórych akcji (np. przejście między widokami)
aplikacja nie zawsze dostarcza jednoznacznej informacji,
że akcja została wykonana poprawnie.

Obserwacja 3 – Utrata kontekstu po odświeżeniu strony
Po odświeżeniu strony użytkownik może utracić aktualny kontekst nawigacyjny,
co może powodować dezorientację.

Ryzyko – Gorsze doświadczenie użytkownika
Brak spójnej nawigacji i czytelnej informacji zwrotnej
może w realnej aplikacji prowadzić do frustracji użytkownika
oraz trudności w realizacji podstawowych celów.

Pomysł na dalsze testy
Sprawdzenie zachowania aplikacji w różnych przeglądarkach
oraz analiza nawigacji z perspektywy użytkownika mobilnego.


