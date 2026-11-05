# HostFlow PMS
Bookingsystem for mindre overnattingsvirksomheter. Kalender, kunder, rapporter og WordPress-integrasjon.

HostFlow - Installasjon på C-panel
1. Last opp filer
Last opp hele mappen `hostflow` til `public_html` (eller en undermappe).
2. Opprett database
Gå til C-panel → MySQL-databaser
Opprett en ny database (f.eks. `hostflow`)
Opprett en bruker og gi den ALLE rettigheter til databasen
Gå til phpMyAdmin, velg den nye databasen, og importer filen `database.sql`
3. Konfigurer database

Åpne `includes/config.php` og endre:
```php
define('DB_HOST', 'localhost');
define('DB_NAME', 'hostflow');
define('DB_USER', 'ditt_brukernavn');
define('DB_PASS', 'ditt_passord');
```
4. Logg inn
Gå til `https://ditt-domene.no/login.php`
Standard innlogging:
E-post: `admin@example.com`
Passord: `admin123`
Bytt passord med en gang!

Funksjoner i denne versjonen
- Om plassen
- Overnatting (rom, hytter, campingplasser, bobilplasser)
- Bestillingsoversikt
- Kalender (21 dager)
- Ny ordre / manuell booking
- Kunderegister
- Enkel rapport

Si ifra hvilke funksjoner du vil ha lagt til eller endret!
