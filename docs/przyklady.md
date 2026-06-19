# Praktyczny podręcznik komend i cykl pracy

## 📊 Ściągawka z podstawowych poleceń Gita

Poniższa tabela przedstawia zestawienie kluczowych komend terminala Git, które są niezbędne do codziennego zarządzania projektem deweloperskim.

| Komenda | Opis działania | Kiedy stosować? |
| :--- | :--- | :--- |
| `git init` | Inicjalizuje nowe, puste repozytorium lokalne. | Raz na początku tworzenia projektu. |
| `git status` | Wyświetla stan przestrzeni roboczej i listę zmodyfikowanych plików. | Regularnie, aby kontrolować stan prac. |
| `git add <plik>` | Dodaje wybrane pliki do obszaru przejściowego (Staging Area). | Przed każdym zatwierdzeniem zmian. |
| `git commit -m "opis"` | Trwale zapisuje zmiany w lokalnej historii z krótkim komentarzem. | Po zakończeniu logicznej części pracy. |
| `git push` | Wysyła lokalne commity na serwer zdalny (GitHub). | Gdy chcemy udostępnić swoją pracę zespołowi. |
| `git pull` | Pobiera i scala najnowsze zmiany z serwera do lokalnego folderu. | Zawsze przed rozpoczęciem edycji plików! |

---

💻 Praktyczny przykład: Klasyczny cykl pracy zespołowej

Poniższy scenariusz prezentuje prawidłową sekwencję komend w terminalu Git Bash podczas codziennej pracy nad wspólnym plikiem tekstowym, minimalizującą ryzyko wystąpienia konfliktów.

```bash
KROK 1: Zawsze zacznij od pobrania zmian od zespołu
git pull origin main

KROK 2: Wprowadź zmiany w plikach tekstowych (np. w edytorze VS Code)
[Tutaj następuje edycja plików i zapisanie zmian skrótem Ctrl + S]
KROK 3: Sprawdź, które pliki zostały zmodyfikowane
git status

KROK 4: Dodaj zmodyfikowany plik do poczekalni
git add docs/teoria.md

KROK 5: Zatwierdź zmiany z jasnym, opisowym komentarzem
git commit -m "docs: uzupelnienie przykladow o sekcje kodu z cyklem pracy"

KROK 6: Wypchnij gotową pracę bezpiecznie na serwer GitHub
git push origin main