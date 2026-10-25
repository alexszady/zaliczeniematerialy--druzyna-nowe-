# System zarządzania drużyną piłkarską

Aplikacja webowa do prowadzenia listy zawodników, statystyk i terminarza meczów. Projekt wykorzystuje Node.js, Express i SQLite.

## Wymagania

- Node.js 18 lub nowszy (zalecany LTS)
- npm

## Uruchomienie lokalne

1. Otwórz terminal w katalogu, w którym znajduje się `package.json`.
2. Zainstaluj zależności:

   ```bash
   npm install
   ```

3. Uruchom serwer:

   ```bash
   npm start
   ```

4. Otwórz w przeglądarce `http://localhost:3000`.

Baza `database.db` utworzy się automatycznie przy pierwszym uruchomieniu, a przykładowi zawodnicy i mecze zostaną dodani, jeśli tabele są puste. Plik bazy jest lokalny i nie należy go dodawać do repozytorium.

## Funkcje

- wyświetlanie zawodników oraz statystyk,
- dodawanie, edytowanie i usuwanie zawodników,
- wyświetlanie terminarza,
- dodawanie, edytowanie i usuwanie meczów,
- podsumowanie liczby zawodników, goli, asyst i meczów.

## API

| Metoda | Endpoint | Działanie |
|---|---|---|
| GET | `/api/players` | lista zawodników |
| POST | `/api/players` | dodanie zawodnika |
| PUT | `/api/players/:id` | edycja zawodnika |
| DELETE | `/api/players/:id` | usunięcie zawodnika |
| GET | `/api/matches` | lista meczów |
| POST | `/api/matches` | dodanie meczu |
| PUT | `/api/matches/:id` | edycja meczu |
| DELETE | `/api/matches/:id` | usunięcie meczu |

## Struktura

- `server.js` — serwer Express i API,
- `public/index.html` — interfejs aplikacji,
- `public/style.css` — style,
- `public/script.js` — logika interfejsu,
- `diagramy/png/` — diagramy w PNG,
- `diagramy/zrodla_dot/` — edytowalne źródła diagramów,
- `diagramy/opis-diagramow.md` — opis diagramów,
- pozostałe pliki Markdown — dokumentacja zaliczeniowa.

## Wgranie do GitHub

Rozpakuj archiwum i skopiuj **zawartość** folderu do głównego katalogu repozytorium (tam, gdzie jest `package.json`). Zatwierdź i wypchnij pliki. Nie dodawaj `node_modules/` ani `database.db`.

Samo opublikowanie kodu w GitHub nie uruchamia aplikacji — do działania potrzebne jest środowisko Node.js. Na komputerze uruchom ją poleceniami powyżej. Do hostingu wybierz usługę obsługującą Node.js i trwały dysk, ponieważ SQLite zapisuje dane do pliku.
