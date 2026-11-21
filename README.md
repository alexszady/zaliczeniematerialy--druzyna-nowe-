# System zarządzania drużyną piłkarską

Aplikacja webowa do prowadzenia listy zawodników, statystyk, tabeli strzelców i terminarza meczów. Projekt wykorzystuje Node.js, Express i SQLite.

## Wymagania zaliczeniowe
1. Repozytorium i opis projektu — `README.md`.
2. Przypadki użycia — pliki `diagram-przypadkow-uzycia*.md` oraz `docs/przypadki-uzycia/`.
3. Diagramy aktywności — `diagramy/png/` i źródła Graphviz.
4. Diagramy sekwencji — `diagramy/png/` i źródła Graphviz.
5. Diagram klas — `diagramy/png/04_diagram_klas.png`.
6. Diagram ERD — `diagramy/png/03_erd_baza_danych.png`.
7. Dokumentacja — `docs/Dokumentacja_projektu.pdf`, `.docx` i `.md`.

## Uruchomienie
W katalogu z `package.json` wykonaj:
```bash
npm install
npm start
```
Następnie otwórz `http://localhost:3000`.

Baza `database.db` tworzy się automatycznie. Nie dodawaj `node_modules/` ani `database.db` do repozytorium.

## Ważne ograniczenia
- Brak logowania i autoryzacji.
- Edycja zawodników i meczów jest dostępna przez API PUT, ale nie przez formularz WWW.
- Tabele `players` i `matches` są niezależne — nie mają relacji ani kluczy obcych.
- Testy opisane w dokumentacji są planem; wyniki należy uzupełnić po faktycznym wykonaniu.
