# Wyświetl terminarz

- **ID:** PU_06_WYSWIETL_TERMINARZ
- **Aktorzy:** Użytkownik, Administrator / Trener
- **Warunki wstępne:** Terminarz może zawierać zero lub więcej meczów.

## Scenariusz podstawowy
1. Aktor otwiera terminarz.\n2. Interfejs wysyła GET /api/matches.\n3. API odczytuje mecze z SQLite.\n4. Interfejs pokazuje przeciwnika, datę, godzinę, miejsce i wynik.

## Scenariusze alternatywne / błędy
Gdy terminarz jest pusty, system pokazuje informację o braku meczów.

## Warunek końcowy
Dane zostały przedstawione lub zmodyfikowane zgodnie z wybraną operacją.
