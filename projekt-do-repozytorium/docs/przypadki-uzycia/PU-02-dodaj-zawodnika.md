# Dodaj zawodnika

- **ID:** PU_02_DODAJ_ZAWODNIKA
- **Aktorzy:** Administrator / Trener
- **Warunki wstępne:** Aktor ma otwartą aplikację.

## Scenariusz podstawowy
1. Aktor otwiera formularz.\n2. Wprowadza imię i nazwisko, numer, pozycję oraz opcjonalne statystyki.\n3. Interfejs sprawdza wymagane pola.\n4. Wysyła POST /api/players.\n5. API zapisuje zawodnika w SQLite i zwraca utworzony rekord.

## Scenariusze alternatywne / błędy
Brak imienia, numeru lub pozycji powoduje komunikat walidacyjny. Błąd bazy powinien zostać zgłoszony jako błąd API.

## Warunek końcowy
Dane zostały przedstawione lub zmodyfikowane zgodnie z wybraną operacją.
