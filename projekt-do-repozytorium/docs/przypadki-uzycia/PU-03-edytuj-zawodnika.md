# Edytuj zawodnika

- **ID:** PU_03_EDYTUJ_ZAWODNIKA
- **Aktorzy:** Administrator / Trener
- **Warunki wstępne:** Zawodnik istnieje w bazie danych.

## Scenariusz podstawowy
1. Aktor wybiera zawodnika.\n2. Zmienia dane.\n3. Interfejs wysyła PUT /api/players/:id.\n4. API aktualizuje rekord o wskazanym ID.\n5. Interfejs odświeża dane.

## Scenariusze alternatywne / błędy
Jeśli ID nie istnieje, aktualizacja nie zmieni rekordu; obecny backend wymaga dopracowania odpowiedzi dla takiego przypadku.

## Warunek końcowy
Dane zostały przedstawione lub zmodyfikowane zgodnie z wybraną operacją.
