# Instrukcja użytkownika – Football Manager

## 1. Uruchomienie aplikacji

Aby uruchomić system, należy:
1. Zainstalować Node.js.
2. Otworzyć terminal w katalogu projektu.
3. Wykonać polecenie `npm install`.
4. Uruchomić aplikację poleceniem `npm start`.
5. Otworzyć przeglądarkę internetową.
6. Wpisać adres `http://localhost:3000`.

## 2. Panel główny

Po uruchomieniu aplikacji użytkownik widzi panel główny zawierający:
- liczbę zawodników;
- liczbę zdobytych goli;
- liczbę asyst;
- liczbę meczów.

## 3. Przeglądanie zawodników

Należy wybrać zakładkę „Zawodnicy”.

System wyświetli listę zawodników wraz z ich numerami, pozycjami oraz statystykami.

## 4. Dodawanie zawodnika

1. Otworzyć zakładkę „Zawodnicy”.
2. Kliknąć przycisk „Dodaj zawodnika”.
3. Wprowadzić imię i nazwisko.
4. Wprowadzić numer zawodnika.
5. Wybrać pozycję.
6. Uzupełnić statystyki.
7. Kliknąć „Zapisz”.

Po zapisaniu zawodnik zostanie dodany do bazy danych.

## 5. Usuwanie zawodnika

1. Otworzyć zakładkę „Zawodnicy”.
2. Odszukać zawodnika na liście.
3. Kliknąć przycisk „Usuń”.
4. Potwierdzić usunięcie.

System usunie wybranego zawodnika z bazy danych.

## 6. Obsługa terminarza

Po wybraniu zakładki „Terminarz” użytkownik może przeglądać zapisane spotkania.

Aby dodać mecz:
1. Kliknąć „Dodaj mecz”.
2. Wprowadzić nazwę przeciwnika.
3. Wybrać datę.
4. Wprowadzić godzinę.
5. Wprowadzić miejsce spotkania.
6. Wprowadzić wynik lub pozostawić wartość domyślną.
7. Kliknąć „Zapisz”.

Aby usunąć mecz, należy kliknąć przycisk „Usuń mecz” i potwierdzić operację.

## 7. Tabela strzelców

Zakładka „Strzelcy” prezentuje ranking zawodników według liczby zdobytych bramek. Lista jest automatycznie sortowana malejąco.

## 8. Zakończenie pracy

Aby zakończyć korzystanie z aplikacji, należy zamknąć kartę przeglądarki oraz zatrzymać serwer w terminalu za pomocą kombinacji `CTRL + C`.
