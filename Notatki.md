# Notatki

  

## Uwagi cz1

- paragraf opisu teoretycznego
- wskazanie miejsca w kodzie gdzie jest podatność
- walidacja danych, XSS
- rozwiązania typu Cors
- konfiguracja cookiesow
- mechanizm autoryzacji użytkowników
- path traversal (23 slajd)
- czy są podejrzane katalogi, ocenić strukturę - aplikacji / architekturę
- content security policy (slajd 33)
- hijacking (slajd 42) - konf osadzania strony w ramkach
- gdzie ta baza danych jest
- rest api? JWT?
- doczytac jak działa SSRF

## Uwagi cz2

- [x] Przepisać na MD? - TAK obowiązkowo MD na GitHubie (napisać w nawiasach co którą częśćopracował)
- Kto ile miał wkładu, kiedy zaczęliśmy - czy systematycznie było robione
- Pamiętajcie, że na jednym punkcie będzie więcej niż 1 rzecz
- [x] WSZYSTKIE REKOMENDACJE NA SPODY DZIAŁÓW
- [ ] REKOMENDACJE ZNACZNIEJ KONKRETNE - muszą być - u nas bardzo biedne)
- [ ] Nie duplikować jak któraś kategoria jest pusta to napisać, że w kategorii np. wcześniejszej już to jest opisane i można podciągnąć też tutaj, ale nie będziemy powtarzać

### Pkt1

problem: dobry

Uwaga: zmienić rekomendacje - Dać na dół (po prostu, żeby kolejność się zgadzała XD)
kluzca... czyli np RSA

Rekomendacje do pojedynczego punktu a nie do kategorii

Per punkt: zastosować ARGON (zamiast zastosować szyfrowanie) (MA BYĆ MOCNO

KONKRETNIE - całkiem konkretnie)

### Pkt2

SHA-256 kiepski na hasło nie jest odporny na brute force (zmienić na BCrypt albo też

ARGON2)

### Pkt3

Należy wykorzystać Prepared statement do mechanizmów SQLowych

to jest mechanizm który filtruje niebezpieczne coś tam i jest odporny na sql injection

### Pkt4

2FA to nie jest tu rozwiązanie (to ok ale jako osobny punkt)

Sam brak faktu 2Fa nie jest nagannych ale by poprawiał - czyli dać fajkę, jest ok

czyli zielona fajeczka i jest ok

Można pozbyć sie tego jako błędu

### Pkt5

czy logi backup są w repo - nie ma to zielona fajeczka

czy w .gitignore są pliki a propos dockera

ZOSTAWMY TAK JAK JEST JEST W PORZĄDKU

ale zaznaczyć, że aplikacja była dostarczona jako kody źródłowe aplikacji, be plików

konfiguracyjnych, serwera bazodanowego ,serwera http itp - nie było dostępu nie można

było sprawdzić

konfiguracja bazy danych

konfiguracja systemu - np firewall

WIĘC GIT - opisać

konfiguracja systemu aplikacji - tomcat

ALE: Tomcata mamy, więc wypadałoby sprawdzić konfiguracje

### Pkt6

Bardzo dobrze, że je wypisaliśmy to na duży plus (o vunerabilities)

-można sprawdzić czy na githubie są jakieś kody do eksploitacji

(wskazać że /czy są skrypty do eksploitacji takiej starej aplikacji na tym githubie) tyle

wystarczy

### Pkt7

Tutaj dobrze, że jest napisany jest ARGON2

(nie ma sensu dublować (tam gdzie brakowało algorytmu chyba pkt2 ))

czyli ok

### Pkt8

OK

Raczej bym dodał, że dobrze by było ją zintegrować z narzędziami monitorującymi

bezpieczeństwo - one nie są wymagane a le znacznie by poprawiło to bezpieczeństwo

### Pkt9

OOOOO jak nie ma logów to zdecydowanie niebezpieczne podnieść ryzyko na 4/5

### Pkt10

Trochę jaśniej opisać

TO co jest opisane tutaj to jest path traversal

Podać jakich bibliotek

UWAGI na koniec

1. Tak czy siak do każdego punktu po paragrafie opisu teoretycznego
2. Jeżeli możemy wskazać w kodzie gdzie jest taka podatność - to podać "Podatnośćznaleziona tu ti tu"
3. Walidacja danych crosside scripting - o tym nic nie znalazł - poszukać XSS
4. Czy są rozwiązania typu CORS
5. Napisać o konfiguracji cookisów
6. Paragraf o w aplikacji autoryzacja jest wykorzystywana za pomocą tego i tego
mechanizmu ( o tych cookisach)
7. Path travelsa 21 slide - ogarnąć (głębokie ukrycie robots.txt i co w nim jest) - sprawdzićczy jest taki plik, czy nie ma podejrzanych plików / folderów
8. Content security policy - czy jest, czy nie ma
9. Click jacking slajd 42 - poprawna konfiguracja osadzania strony w ramkach - opisać
10. Co z tą bazą w końcu
11. Opisać Restow API i JWT- jak działa to JWT każdy endpoint powinien być zabezpieczony
12. Serwer side request forgery - coś o tym

Na razie jest ok ale dodać to i tamto