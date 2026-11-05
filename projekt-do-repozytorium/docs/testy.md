# Plan testów systemu Football Manager

## 1. Cel testowania

Celem testów jest sprawdzenie poprawności działania najważniejszych funkcjonalności systemu zarządzania drużyną piłkarską.

## 2. Przypadki testowe

| ID | Test | Oczekiwany rezultat |
|---|---|---|
| T01 | Uruchomienie aplikacji | Wyświetlenie panelu głównego |
| T02 | Wyświetlenie zawodników | Pojawienie się listy zawodników |
| T03 | Dodanie zawodnika | Zawodnik zostaje zapisany |
| T04 | Dodanie bez imienia | Wyświetlenie komunikatu o błędzie |
| T05 | Usunięcie zawodnika | Zawodnik zostaje usunięty |
| T06 | Wyświetlenie terminarza | Pojawienie się listy meczów |
| T07 | Dodanie meczu | Mecz zostaje zapisany |
| T08 | Dodanie meczu bez przeciwnika | Wyświetlenie komunikatu o błędzie |
| T09 | Usunięcie meczu | Mecz zostaje usunięty |
| T10 | Wyświetlenie tabeli strzelców | Zawodnicy zostają uporządkowani według liczby goli |
| T11 | Wyświetlenie statystyk | Poprawne sumowanie goli i asyst |
| T12 | Brak połączenia z serwerem | Wyświetlenie komunikatu o problemie |

## 3. Przebieg testowania

Testy należy przeprowadzić ręcznie z poziomu przeglądarki internetowej.

Każdy test powinien zostać wykonany poprzez wybranie odpowiedniej funkcji aplikacji i sprawdzenie otrzymanego rezultatu.

## 4. Dokumentowanie wyników

Dla każdego testu należy zapisać:
- identyfikator testu;
- datę wykonania;
- otrzymany rezultat;
- informację, czy test zakończył się powodzeniem;
- ewentualne uwagi.

## 5. Uwagi

Powyższa tabela przedstawia plan testów i oczekiwane rezultaty. Testy należy faktycznie wykonać przed oddaniem projektu, a ich wyniki uzupełnić na podstawie rzeczywistego działania aplikacji.
