# Usuń zawodnika

- **ID:** PU_04_USUN_ZAWODNIKA
- **Aktorzy:** Administrator / Trener
- **Warunki wstępne:** Zawodnik istnieje w bazie danych.

## Scenariusz podstawowy
1. Aktor wybiera opcję usunięcia.\n2. System powinien poprosić o potwierdzenie.\n3. Interfejs wysyła DELETE /api/players/:id.\n4. API usuwa rekord.\n5. Lista zawodników jest odświeżana.

## Scenariusze alternatywne / błędy
W razie błędu API użytkownik powinien otrzymać komunikat.

## Warunek końcowy
Dane zostały przedstawione lub zmodyfikowane zgodnie z wybraną operacją.
