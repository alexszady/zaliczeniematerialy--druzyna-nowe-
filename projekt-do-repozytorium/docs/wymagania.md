# Wymagania systemu

## Wymagania funkcjonalne
- WF-01: system udostępnia listę zawodników.
- WF-02: system umożliwia dodanie zawodnika z imieniem i nazwiskiem, numerem oraz pozycją.
- WF-03: system umożliwia aktualizację danych zawodnika.
- WF-04: system umożliwia usunięcie zawodnika.
- WF-05: system przechowuje statystyki zawodnika: gole, asysty i występy.
- WF-06: system wylicza łączną liczbę zawodników, goli, asyst i meczów na pulpicie.
- WF-07: system prezentuje tabelę strzelców posortowaną malejąco według liczby goli.
- WF-08: system udostępnia terminarz meczów z przeciwnikiem, datą, godziną, miejscem i wynikiem.
- WF-09: system udostępnia operacje API do zarządzania meczami.
- WF-10: dane są przechowywane w bazie SQLite.

## Wymagania niefunkcjonalne
- WNF-01: aplikacja działa w przeglądarce internetowej.
- WNF-02: backend udostępnia dane przez HTTP API w formacie JSON.
- WNF-03: dane wejściowe są przesyłane z nagłówkiem `Content-Type: application/json`.
- WNF-04: aplikacja korzysta z Node.js, Express i SQLite.
- WNF-05: błędy komunikacji z serwerem są sygnalizowane użytkownikowi.
- WNF-06: zapytania SQL z parametrami korzystają z wiązanych parametrów, aby ograniczyć ryzyko wstrzyknięcia SQL.

## Ograniczenia / kwestie do dopracowania
- W aktualnym schemacie brak tabeli użytkowników i mechanizmu logowania, więc role „Użytkownik” oraz „Administrator / Trener” są rolami koncepcyjnymi, a nie egzekwowanymi uprawnieniami.
- Tabele `players` i `matches` są niezależne; projekt nie zapisuje szczegółowych statystyk zawodnika przypisanych do konkretnego meczu.
- Przed oddaniem warto zweryfikować, czy wszystkie operacje meczów są dostępne w interfejsie, ponieważ dokumentacja obejmuje również zakres API.
