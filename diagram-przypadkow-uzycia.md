# Diagram przypadków użycia — Football Manager

Diagram obejmuje funkcje dostępne w aktualnym interfejsie WWW: przeglądanie zawodników, dodawanie i usuwanie zawodników, podgląd statystyk, terminarz, dodawanie i usuwanie meczów oraz tabelę strzelców.

![Diagram przypadków użycia](diagramy/png/01_przypadki_uzycia.png)

**Aktor:** Użytkownik aplikacji. Projekt nie posiada logowania ani autoryzacji, dlatego nie rozróżnia technicznie ról użytkownika i administratora.

## Zakres dostępny wyłącznie przez API

Endpointy `PUT /api/players/:id` i `PUT /api/matches/:id` istnieją w backendzie, ale aktualny interfejs WWW nie zawiera formularzy edycji. Z tego powodu pokazano je osobno jako operacje inicjowane przez klienta REST API na diagramie rozszerzonym.
