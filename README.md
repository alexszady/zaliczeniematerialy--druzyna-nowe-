 System zarządzania drużyną piłkarską

## 1. Opis projektu

Football Manager to aplikacja internetowa służąca do zarządzania drużyną piłkarską. Jej głównym zadaniem jest ułatwienie prowadzenia ewidencji zawodników, kontrolowania ich statystyk oraz zarządzania terminarzem spotkań.

System umożliwia przeglądanie informacji o drużynie, dodawanie zawodników, usuwanie zawodników, przeglądanie tabeli strzelców oraz zarządzanie informacjami o meczach.

Aplikacja została przygotowana jako projekt zaliczeniowy.

## 2. Cel projektu

Celem projektu jest stworzenie prostego i funkcjonalnego systemu wspomagającego zarządzanie drużyną piłkarską.

System ma za zadanie:
- przechowywać dane zawodników;
- prezentować statystyki zawodników;
- wyświetlać łączną liczbę goli i asyst;
- umożliwiać prowadzenie terminarza spotkań;
- prezentować tabelę najlepszych strzelców;
- zapewniać dostęp do danych za pomocą interfejsu internetowego.

## 3. Technologie wykorzystane w projekcie

W projekcie wykorzystano następujące technologie:

- **HTML5** – budowa struktury strony internetowej.
- **CSS3** – wygląd i stylizacja interfejsu.
- **JavaScript** – obsługa interakcji użytkownika i komunikacja z API.
- **Node.js** – środowisko uruchomieniowe serwera.
- **Express.js** – obsługa serwera i endpointów API.
- **SQLite** – relacyjna baza danych przechowująca informacje o zawodnikach i meczach.
- **Git i GitHub** – kontrola wersji i przechowywanie kodu źródłowego.

## 4. Funkcjonalności systemu

### 4.1. Panel główny

Panel główny prezentuje podstawowe informacje o drużynie:
- liczbę zawodników;
- łączną liczbę zdobytych goli;
- łączną liczbę asyst;
- liczbę rozegranych lub zapisanych meczów.

### 4.2. Zarządzanie zawodnikami

System umożliwia:
- wyświetlanie listy zawodników;
- dodawanie nowych zawodników;
- usuwanie zawodników;
- przechowywanie numeru zawodnika i jego pozycji;
- przechowywanie statystyk zawodnika.

Dane zawodnika obejmują imię i nazwisko, numer, pozycję, liczbę goli, asyst i występów.

### 4.3. Terminarz meczów

System umożliwia:
- wyświetlanie listy meczów;
- dodawanie nowych spotkań;
- usuwanie spotkań;
- zapisywanie przeciwnika;
- zapisywanie daty i godziny spotkania;
- zapisywanie miejsca rozgrywania meczu;
- przechowywanie wyniku spotkania.

### 4.4. Tabela strzelców

Aplikacja prezentuje zawodników uporządkowanych według liczby zdobytych bramek. Zawodnik z największą liczbą goli znajduje się na pierwszym miejscu.

## 5. Architektura aplikacji

Aplikacja wykorzystuje architekturę klient-serwer.

Składa się z trzech głównych elementów:

1. Frontend – interfejs użytkownika wykonany w HTML, CSS i JavaScript.
2. Backend – serwer Node.js wykorzystujący Express.js.
3. Baza danych – SQLite przechowująca informacje o zawodnikach i meczach.

Komunikacja pomiędzy frontendem a backendem odbywa się za pomocą żądań HTTP i danych w formacie JSON.

## 6. Struktura bazy danych

Baza danych składa się z dwóch tabel.

### Tabela players

| Pole | Typ | Opis |
|---|---|---|
| id | INTEGER | Klucz główny |
| name | TEXT | Imię i nazwisko |
| number | INTEGER | Numer zawodnika |
| position | TEXT | Pozycja |
| goals | INTEGER | Liczba goli |
| assists | INTEGER | Liczba asyst |
| appearances | INTEGER | Liczba występów |

### Tabela matches

| Pole | Typ | Opis |
|---|---|---|
| id | INTEGER | Klucz główny |
| opponent | TEXT | Nazwa przeciwnika |
| match_date | TEXT | Data spotkania |
| match_time | TEXT | Godzina spotkania |
| location | TEXT | Miejsce spotkania |
| result | TEXT | Wynik spotkania |

Obie tabele posiadają własne klucze główne. W aktualnej wersji nie występuje między nimi bezpośrednia relacja.

## 7. Interfejs użytkownika

Aplikacja posiada cztery główne sekcje:

- Dashboard – podstawowe statystyki drużyny.
- Zawodnicy – lista zawodników i formularz dodawania.
- Terminarz – lista spotkań i formularz dodawania meczu.
- Strzelcy – ranking zawodników według liczby zdobytych goli.

## 8. Bezpieczeństwo i walidacja

System wykorzystuje parametryzowane zapytania SQL, co ogranicza ryzyko ataków SQL Injection.

Dane przesyłane do API są przekazywane w formacie JSON.

Podstawowa walidacja formularzy sprawdza obecność wymaganych danych, takich jak imię i nazwisko zawodnika, numer, pozycja oraz przeciwnik i data meczu.

W obecnej wersji nie zaimplementowano systemu logowania ani autoryzacji użytkowników.

## 9. Możliwości rozwoju

W przyszłości aplikacja może zostać rozbudowana o:
- system logowania i rejestracji;
- role użytkowników i administratorów;
- edycję danych zawodników w interfejsie;
- edycję informacji o meczach w interfejsie;
- szczegółowe statystyki poszczególnych spotkań;
- wyszukiwanie zawodników;
- filtrowanie tabeli zawodników;
- eksport statystyk do pliku PDF.

## 10. Podsumowanie

Projekt Football Manager realizuje podstawowe funkcje systemu wspomagającego zarządzanie drużyną piłkarską. Umożliwia przechowywanie informacji o zawodnikach i meczach, prezentowanie statystyk oraz przeglądanie tabeli strzelców.

Zastosowanie technologii internetowych oraz bazy SQLite pozwala na sprawne przechowywanie i prezentowanie danych. Projekt może stanowić podstawę do dalszego rozwoju systemu zarządzania drużyną sportową.
