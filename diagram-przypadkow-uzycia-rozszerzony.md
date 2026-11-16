# Rozszerzony diagram przypadków użycia — Football Manager

![Rozszerzony diagram przypadków użycia](diagramy/png/02_przypadki_uzycia_rozszerzony.png)

Diagram rozróżnia użytkownika interfejsu WWW oraz klienta REST API. Operacje aktualizacji zawodnika i meczu są dostępne jako endpointy `PUT`, lecz nie są obsługiwane formularzami w interfejsie WWW.

Relacja `<<include>>` przy dodawaniu oznacza sprawdzenie wymaganych danych. Odczyt danych z SQLite jest wspólnym krokiem przypadków prezentujących dane.

**Ograniczenie:** brak logowania i mechanizmu ról. Każdy, kto ma dostęp do aplikacji/API, może wywołać udostępnione operacje.
