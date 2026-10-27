# GPT AMG Workspace

Kanał wydań aplikacji macOS łączącej oficjalny widok ChatGPT z lokalnym klientem Codex app-server.

Wymagania: macOS 14 lub nowszy, Apple Silicon albo Intel. Rozmowy Codexa wymagają zainstalowanego oficjalnego Codexa i logowania na własnym koncie. ChatGPT wymaga ręcznego logowania w aplikacji i włączenia widoku witryny.

Paczki instalacyjne są dostępne w sekcji Releases. Repozytorium nie zawiera historii rozmów, ustawień, danych logowania ani prywatnych kluczy podpisujących.

Od kompilacji 13 aplikacja automatycznie pobiera zgodne aktualizacje. Obok numeru wersji pokazuje ich stan. Pobrana wersja jest instalowana po zwykłym zamknięciu aplikacji; kolejne uruchomienie używa nowej wersji. Aktualizator weryfikuje podpisy EdDSA kanału i paczki.

Obecne wydanie ma lokalny podpis ad hoc i nie jest notaryzowane przez Apple. Pierwsza instalacja na innym Macu może wymagać ręcznego zatwierdzenia przez właściciela komputera. Podpis EdDSA aktualizacji nie zastępuje certyfikatu Developer ID. Nie zmieniaj globalnych zabezpieczeń macOS.

Aplikacja jest niezależnym projektem i nie jest oficjalnym klientem OpenAI. Zakres funkcji Codexa jest rozwijany; pełna zgodność z aplikacją OpenAI nie jest deklarowana.
