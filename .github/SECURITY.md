# Security

Zgłoszenia podatności: **mik.jed2003@gmail.com** (nie otwieraj publicznego issue).

W produktach z danymi klientów (Detailflow) obowiązuje dodatkowo:

- sekrety tylko w GitHub Actions secrets / env serwera, nigdy w git
- tokeny KSeF i klucze Stripe szyfrowane at rest
- Stripe webhook weryfikowany podpisem
- izolacja tenantów (`studioId`) jest błędem P0, nie „później”
