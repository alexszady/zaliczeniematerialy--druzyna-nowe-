# Instalacja i konfiguracja Football Manager

## 1. Wymagania

Do uruchomienia projektu potrzebne są:
- system Windows, Linux lub macOS;
- Node.js;
- npm;
- przeglądarka internetowa;
- dostęp do plików projektu.

## 2. Pobranie projektu

Należy pobrać repozytorium z GitHub lub skopiować pliki projektu do wybranego katalogu.

## 3. Instalacja zależności

W terminalu należy przejść do katalogu zawierającego plik `package.json` i wykonać:

```bash
npm install
```

Polecenie zainstaluje wymagane biblioteki:
- express;
- cors;
- sqlite3.

## 4. Uruchomienie

Aplikację uruchamia się poleceniem:

```bash
npm start
```

Serwer powinien uruchomić się na porcie 3000.

## 5. Dostęp do aplikacji

Po uruchomieniu serwera należy otworzyć:

```text
http://localhost:3000
```

## 6. Baza danych

Baza danych SQLite jest inicjalizowana automatycznie przez serwer. Nie ma potrzeby ręcznego tworzenia tabel.

## 7. Rozwiązywanie problemów

Jeżeli aplikacja się nie uruchamia:
- należy sprawdzić, czy Node.js jest zainstalowany;
- sprawdzić, czy wykonano `npm install`;
- sprawdzić, czy port 3000 nie jest zajęty;
- sprawdzić komunikaty błędów w terminalu.
