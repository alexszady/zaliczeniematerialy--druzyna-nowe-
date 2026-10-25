# Wyświetl zawodników

- **ID:** PU_01_WYSWIETL_ZAWODNIKOW
- **Aktorzy:** Użytkownik, Administrator / Trener
- **Warunki wstępne:** Lista zawodników jest dostępna w bazie danych.

## Scenariusz podstawowy
1. Aktor otwiera sekcję zawodników.\n2. Interfejs wysyła GET /api/players.\n3. API pobiera rekordy z SQLite.\n4. Interfejs prezentuje listę.

## Scenariusze alternatywne / błędy
W przypadku błędu API aplikacja wyświetla komunikat o braku połączenia.

## Warunek końcowy
Dane zostały przedstawione lub zmodyfikowane zgodnie z wybraną operacją.
