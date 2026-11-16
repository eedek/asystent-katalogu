# asystent-katalogu
# AsystentKatalogu_kacperluszcz (v1.0)

## 1. Opis i cel aplikacji
Wewnętrzne narzędzie przeznaczone wyłącznie na potrzeby własnego konta Allegro. Służy do standaryzacji nazw produktów, marek oraz weryfikacji parametrów katalogowych po kodach EAN/GTIN na potrzeby zarządzania ofertami.

## 2. Zakres funkcjonalny aplikacji
- Wyszukiwanie produktów w katalogu Allegro na podstawie kodów GTIN/EAN.
- Pobieranie ustandaryzowanych nazw, marek, kategorii oraz podstawowych parametrów technicznych produktów.

## 3. Sposób połączenia z Allegro
Aplikacja komunikuje się z Allegro REST API jako skrypt serwerowy, wykorzystując uwierzytelnianie OAuth 2.0 (Client Credentials / Authorization Code).

## 4. Wykorzystanie Allegro API i wymagane uprawnienia
| Scope | Funkcja aplikacji | Wykorzystanie |
| :--- | :--- | :--- |
| `allegro:api:sale:offers:read` | Weryfikacja katalogu produktów | Odczyt danych produktowych i ofertowych w celu dopasowania asortymentu po kodzie EAN/GTIN. |

## 5. Dostęp i bezpieczeństwo danych
Dostęp do aplikacji oraz kluczy API (`Client ID`, `Client Secret`, tokeny OAuth) posiada wyłącznie właściciel konta. Poświadczenia przechowywane są w zabezpieczonych zmiennych środowiskowych na prywatnym serwerze i nie są udostępniane podmiotom trzecim.

## 6. Dane kontaktowe
W sprawach związanych z działaniem integracji prosimy o kontakt: **luszczkacper42@gmail.com**
