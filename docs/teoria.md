Podstawy teoretyczne systemów kontroli wersji
🌐 Wprowadzenie do systemów kontroli wersji (VCS)
System kontroli wersji (ang. Version Control System) to oprogramowanie służące do śledzenia modyfikacji wprowadzanych w plikach oraz zarządzania historią tych zmian. W projektach zespołowych kluczowe znaczenie ma rozproszony system kontroli wersji (DVCS), którego najpopularniejszym przedstawicielem jest Git. W architekturze rozproszonej każdy uczestnik projektu posiada na swoim lokalnym dysku pełną kopię repozytorium wraz z całą jego historią, co zapewnia niezależność pracy i bezpieczeństwo danych.

🏛️ Różnica między Git a GitHub
Częstym błędem jest utożsamianie tych dwóch pojęć. 
Git to lokalne narzędzie (działające w wierszu poleceń), które dba o historię plików na Twoim komputerze.
GitHub to platforma chmurowa, która pozwala na przechowywanie lokalnych repozytoriów w sieci, ułatwiając współpracę, zarządzanie uprawnieniami oraz automatyzację projektów.

---

📥 Sekcja 1: Zapisywanie zmian i wysyłanie na serwer

💾 Operacja: Commit
Commit (zatwierdzenie) to podstawowa jednostka w historii Gita. Można go porównać do „migawki” (ang. snapshot) stanu całego projektu w danym momencie. Każdy commit tworzy trwały punkt w historii, do którego można w każdej chwili powrócić. Dobrą praktyką jest tworzenie małych, logicznych commitów opatrzonych jasnym komentarzem opisującym wprowadzane zmiany.

🛰️ Operacja: Push
Push (wypchnięcie) to proces synchronizacji lokalnych zmian z repozytorium zdalnym (np. na platformie GitHub). Wykonanie komendy push przesyła nowo utworzone lokalnie commity na serwer, dzięki czemu stają się one widoczne i dostępne dla pozostałych członków zespołu deweloperskiego.

---

📤 Sekcja 2: Pobieranie projektu i synchronizacja zmian

🧪 Operacja: Clone
Clone (klonowanie) to operacja wykonywana zazwyczaj tylko raz na początku pracy z projektem. Służy do pobrania kompletnego repozytorium z serwera zdalnego (GitHub) na lokalny dysk twardy komputera. W przeciwieństwie do zwykłego pobrania archiwum ZIP, operacja clone konfiguruje automatyczne połączenie z serwerem i pobiera pełną historię wszystkich dotychczasowych commitów oraz gałęzi.

🔄 Operacja: Pull
Pull (pobranie zmian) to kluczowa komenda w pracy wieloosobowej. Służy do pobrania najnowszych modyfikacji wprowadzonych przez innych członków zespołu z serwera zdalnego i automatycznego scalenia ich z lokalną wersją roboczą. Regularne wykonywanie operacji pull przed rozpoczęciem pracy jest fundamentalną zasadą pozwalającą unikać konfliktów w kodzie.