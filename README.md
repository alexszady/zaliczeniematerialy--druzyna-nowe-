# Football Manager — system zarządzania drużyną piłkarską

Aplikacja internetowa do ewidencji zawodników, prezentowania statystyk, prowadzenia terminarza spotkań i wyświetlania tabeli strzelców.

## Technologie

HTML5, CSS3, JavaScript, Node.js, Express.js i SQLite.

## Uruchomienie

Wymagany Node.js 18+ oraz npm.

```bash
npm install
npm start
```

Otwórz `http://localhost:3000`. Baza `database.db` oraz tabele tworzą się automatycznie. Przykładowe dane dodawane są tylko wtedy, gdy odpowiednia tabela jest pusta.

## Funkcje interfejsu

- Dashboard: liczba zawodników, gole, asysty i mecze.
- Zawodnicy: wyświetlanie, dodawanie i usuwanie.
- Terminarz: wyświetlanie, dodawanie i usuwanie meczów.
- Strzelcy: ranking według liczby goli.

Backend udostępnia ponadto endpointy `PUT` do aktualizacji zawodnika i meczu, ale aktualny interfejs WWW nie ma formularzy edycji.

## API

| Metoda | Endpoint | Działanie |
|---|---|---|
| GET | `/api/players` | Lista zawodników |
| POST | `/api/players` | Dodanie zawodnika |
| PUT | `/api/players/:id` | Aktualizacja zawodnika (API) |
| DELETE | `/api/players/:id` | Usunięcie zawodnika |
| GET | `/api/matches` | Lista meczów |
| POST | `/api/matches` | Dodanie meczu |
| PUT | `/api/matches/:id` | Aktualizacja meczu (API) |
| DELETE | `/api/matches/:id` | Usunięcie meczu |

## Dokumentacja i diagramy

- `docs/wymagania.md` — wymagania funkcjonalne i niefunkcjonalne.
- `docs/aktorzy.md` — aktorzy i ograniczenia ról.
- `docs/przypadki-uzycia/` — scenariusze przypadków użycia.
- `diagramy/png/` — diagramy w PNG i SVG.
- `diagramy/zrodla_dot/` — edytowalne źródła diagramów Graphviz.
- `diagramy/sekwencje/` — diagramy sekwencji Mermaid.
- `docs/` — architektura, instalacja, instrukcja użytkownika i plan testów.

## Struktura

`server.js` — backend i API; `public/` — frontend; `database.db` — lokalna baza generowana przy uruchomieniu.

Nie dodawaj do repozytorium `node_modules/` ani lokalnego pliku `database.db`.
