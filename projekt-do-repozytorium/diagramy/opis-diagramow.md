# Opis diagramów

## Diagram przypadków użycia
Pokazuje funkcje dostępne użytkownikowi i administratorowi/trenerowi. Diagram rozszerzony grupuje operacje zarządzania zawodnikami i meczami oraz przedstawia walidację i zapis/odczyt danych.

## ERD — schemat bazy danych
Diagram odzwierciedla tabele `players` i `matches` utworzone przez `server.js`. Pola `id` są kluczami głównymi. W obecnym kodzie nie ma klucza obcego ani relacji między tabelami — nie należy ich dopisywać do ERD bez zmiany schematu.

## Diagram klas
Przedstawia role, warstwę systemu, bazę danych oraz modele `Player` i `Match` jako logiczny widok architektury aplikacji.

## Diagramy aktywności
Pokazują główne przepływy: pobranie listy zawodników, dodanie, edycję i usunięcie zawodnika oraz operacje na terminarzu.

## Diagramy sekwencji
Przedstawiają kolejność komunikacji pomiędzy użytkownikiem, interfejsem WWW, API Express i bazą SQLite dla głównych operacji.

## Uwaga
Diagramy są dokumentacją projektową odtworzoną na podstawie dostarczonego kodu i istniejących plików Markdown. Diagram sekwencji zarządzania meczami jest uogólniony dla operacji CRUD; szczegóły odpowiedzi mogą zależeć od implementacji endpointu.
