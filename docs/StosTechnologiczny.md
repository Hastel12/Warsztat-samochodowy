### Frontend - Interfejs użytkownika (aplikacja webowa) 

**Technologia: React (JavaScript) + TypeScript**  

Uzasadnienie: Pozwala zrobić osobne widoki dla Biura, Mechanika i Magazyniera z tych samych komponentów (tabele, formularze). Działa w przeglądarce, więc nic nie trzeba instalować. 



### Backend - Serwer aplikacji (API)  

**Technologia: Node.js + Express (JavaScript) + TypeScript**  

Uzasadnienie: Backend w JavaScripcie, tym samym języku co frontend, więc wszystko będzie w jednej technologii. 



### Baza danych  

**Technologia: PostgreSQL **

Uzasadnienie: Dane są relacyjne (klient – pojazd – zlecenie – części), a transakcje chronią stany magazynowe.  



### Logowanie i role  

**Technologia: JWT ** 

Uzasadnienie: Każda rola widzi tylko swoje funkcje. Klient się nie loguje, obsługuje go Biuro. 



### Powiadomienia e-mail i SMS 

**Technologia: Bramka SMS (np. SMSAPI) + Nodemailer (e-mail)**  

Uzasadnienie: Proste API, Moduł Powiadomienia wysyła klientowi wiadomość, np. gdy wycena jest gotowa. SMS na czas projektu może działać w trybie testowym.  



### Repozytorium i praca zespołowa  

**Technologia: Git + GitHub** 

Uzasadnienie: Wymóg zadania: zmiany tylko przez pull request zaakceptowany przez inną osobę z zespołu.. 



### Diagramy  

**Technologia: draw.io** 

Uzasadnienie: Plik źródłowy i eksport do PNG, zgodnie z wymaganiami. 



### Uruchamianie  

**Docker Compose** 

Uzasadnienie: Całe środowisko (API + baza) startuje jedną komendą. 

