# Dokumentacja techniczna systemu Football Manager

## 1. Architektura systemu

System został zbudowany w architekturze klient-serwer.

Frontend odpowiada za prezentację danych i obsługę działań użytkownika. Backend przetwarza żądania HTTP, komunikuje się z bazą danych i zwraca odpowiedzi w formacie JSON.

## 2. Frontend

Frontend znajduje się w katalogu `public`.

Główne pliki:

- `index.html` – struktura strony i formularze.
- `style.css` – wygląd aplikacji.
- `script.js` – logika działania interfejsu.

JavaScript wykorzystuje funkcję `fetch()` do komunikacji z serwerem.

## 3. Backend

Backend znajduje się w pliku `server.js`.

Wykorzystuje:
- Express.js do obsługi serwera;
- CORS do obsługi żądań między źródłami;
- SQLite3 do komunikacji z bazą danych;
- moduł path do obsługi ścieżek plików.

Domyślny port serwera to 3000.

## 4. Endpointy API

### Zawodnicy

| Metoda | Endpoint | Działanie |
|---|---|---|
| GET | /api/players | Pobranie zawodników |
| POST | /api/players | Dodanie zawodnika |
| PUT | /api/players/:id | Aktualizacja zawodnika |
| DELETE | /api/players/:id | Usunięcie zawodnika |

### Mecze

| Metoda | Endpoint | Działanie |
|---|---|---|
| GET | /api/matches | Pobranie terminarza |
| POST | /api/matches | Dodanie meczu |
| PUT | /api/matches/:id | Aktualizacja meczu |
| DELETE | /api/matches/:id | Usunięcie meczu |

Uwaga: operacje PUT są dostępne w API, ale formularze edycji nie są obecnie dostępne w interfejsie użytkownika.

## 5. Baza danych

Baza SQLite jest tworzona automatycznie podczas uruchamiania serwera.

Plik bazy danych nosi nazwę `database.db`.

Podczas pierwszego uruchomienia system tworzy tabele `players` i `matches`. Jeżeli tabele są puste, dodawane są przykładowe rekordy.

## 6. Obsługa błędów

Backend zwraca odpowiedzi HTTP informujące o powodzeniu lub niepowodzeniu operacji.

Przykładowe kody:
- 200 – poprawne wykonanie operacji;
- 201 – poprawne utworzenie rekordu;
- 400 – nieprawidłowe dane wejściowe;
- 500 – błąd serwera lub bazy danych.

## 7. Ograniczenia techniczne

Aktualna wersja nie posiada:
- systemu autoryzacji;
- systemu rejestracji użytkowników;
- rozbudowanej walidacji wszystkich pól;
- historii zmian danych;
- edycji rekordów bezpośrednio z poziomu interfejsu.

## 8. Podsumowanie

Zastosowana architektura umożliwia oddzielenie warstwy prezentacji, logiki serwerowej i przechowywania danych. Dzięki temu aplikacja może być rozwijana poprzez dodawanie kolejnych funkcjonalności bez konieczności przebudowy całego systemu.
