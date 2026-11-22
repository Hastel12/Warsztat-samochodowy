## Zarejestruj zlecenie

**Scenariusz główny:**

1. Pracownik biura otwiera formularz nowego zlecenia.
2. Wprowadza dane kontaktowe klienta (telefon lub e-mail), dane samochodu i opis usterki.
3. System weryfikuje kompletność pól obowiązkowych.
4. System zapisuje zlecenie, nadaje mu unikalny numer i ustawia status „Przyjęte”.

**Scenariusz alternatywny:**

* 3a. Brakuje pola obowiązkowego. System nie zapisuje zlecenia i wyświetla komunikat przy każdym brakującym polu. Przypadek wraca do kroku 2.


 ## Przygotuj i wyślij wycenę
**Scenariusz główny:**

1. Pracownik biura otwiera zlecenie o statusie „Zdiagnozowane” i widzi diagnozę, listę części i szacowany czas pracy.
2. Przygotowuje wycenę (koszt części i robocizny) i ją zatwierdza.
3. System wybiera kanał wysyłki zgodnie z danymi kontaktowymi klienta: Usługę SMS (telefon) lub Usługę e-mail (adres e-mail).
4. System przekazuje treść wyceny wybranej usłudze.
5. Usługa potwierdza wysłanie wiadomości.
6. System zmienia status zlecenia na „Wycena wysłana” i zapisuje datę oraz godzinę wysyłki w historii zlecenia.

**Scenariusze alternatywne:**

* 3a. Klient ma podane tylko jedno dane kontaktowe. System używa jedynej dostępnej usługi.
* 5a. Usługa zgłasza błąd lub jest niedostępna. System wyświetla pracownikowi biura komunikat o błędzie, nie zmienia statusu zlecenia i umożliwia ponowienie wysyłki (powrót do kroku 3).

## Sprawdź dostępność i wydaj części

**Scenariusz główny:**

1. Magazynier otwiera zgłoszenie części powiązane ze zleceniem.
2. System wyświetla dla każdej pozycji aktualny stan magazynowy i oznacza, czy część jest dostępna.
3. Wszystkie części są na stanie, więc magazynier potwierdza ich wydanie.
4. System zmniejsza stan magazynowy o wydane ilości.
5. System zapisuje wydanie w zleceniu.
6. System powiadamia mechanika, że części są gotowe do odbioru

**Scenariusze alternatywne:**

* 3a. Stan magazynowy jest mniejszy niż żądana ilość. System blokuje wydanie i wyświetla komunikat o niewystarczającym stanie. Zlecenie przechodzi w status „Oczekuje na części”, a magazynier zamawia brakującą część.
* 3b. Po przyjęciu dostawy stan magazynowy rośnie, a przypadek wraca do kroku 3.