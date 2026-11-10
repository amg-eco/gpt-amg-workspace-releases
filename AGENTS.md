# Polityka GitHub Actions (amg-eco, 10.11.2026)

Te same zasady użycia GitHub Actions co w SuperSpedytorze (`AMG-Trans/AMG_Fracht`, `AGENTS.md`, blok B970 z 3.11.2026). Wprowadził je Jacek Palęcki, właściciel organizacji `amg-eco`, 10.11.2026. Zmiana tego bloku wymaga jego jawnej zgody.

## Koszt GitHub Actions
- Żadnych automatycznych triggerów: `push`, `pull_request`, `pull_request_target`, `workflow_run`, `merge_group`. Dozwolone tylko `workflow_dispatch` (ręcznie) oraz `schedule` nie częściej niż raz na dobę.
- Żadnych runnerów macOS (`macos-*`) ani większych runnerów bez osobnej zgody Jacka.
- Testy, lint, typecheck i buildy kontrolne uruchamiasz LOKALNIE, nie w Actions.
- Nie uruchamiaj ręcznie testów w GitHub Actions ani dodatkowych buildów bez wyraźnego polecenia użytkownika. Wynik Actions nie jest weryfikacją zmiany.
- Nie twórz łańcuchów workflowów (`workflow_run`, automatycznie wywoływane `workflow_call`).
- Push na gałąź odpala workflowy z pliku NA TEJ GAŁĘZI. Zanim pushniesz na starą gałąź, sprawdź jej `.github/workflows` i usuń automatyczne triggery.

## Testy lokalne
- Testy oraz lint wykonuj lokalnie, w izolowanym środowisku projektu, przed przekazaniem zmiany do review i przed scaleniem.
- Dobieraj testy do zmiany. Nie powtarzaj zaliczonych testów bez nowej zmiany, błędu lub konkretnego powodu.
- Jeżeli test lokalny jest zablokowany, wskaż przyczynę i napraw lokalne środowisko. Nie zastępuj go testami w chmurze.

## Workflowy
- `.github/workflows/` zmieniasz tylko w zgodzie z tym blokiem i za jawną zgodą Jacka. Nie dodawaj workflowów z automatycznymi triggerami.
