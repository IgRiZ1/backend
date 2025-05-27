Laravel Gastenboek
Beschrijving
Dit is een Laravel-gebaseerd gastenboekproject waarin gebruikers zich kunnen registreren, inloggen, berichten (posts) kunnen aanmaken, wijzigen, verwijderen en beheerders nieuwe gebruikers kunnen aanmaken. Het project maakt gebruik van Laravel's authenticatie- en autorisatiefuncties, een MySQL-database en volgt het MVC-patroon.
Functionaliteiten

Gebruikersregistratie: Nieuwe gebruikers kunnen zich registreren met een naam, e-mailadres en wachtwoord.
Inloggen: Geregistreerde gebruikers kunnen inloggen met hun e-mailadres en wachtwoord.
Berichtenbeheer:
Gebruikers kunnen nieuwe berichten aanmaken in het gastenboek.
Gebruikers kunnen hun eigen berichten wijzigen.
Gebruikers kunnen hun eigen berichten verwijderen.


Gebruikersbeheer (voor beheerders):
Beheerders kunnen nieuwe gebruikers aanmaken via een beveiligd admin-paneel.


Beveiliging: Authenticatie en autorisatie met Laravel's ingebouwde systemen (bijv. middleware en policies).

Vereisten

PHP >= 8.1
Composer
MySQL of een andere compatibele database
Node.js en NPM (voor frontend-assets)
Laravel >= 10.x

Installatie

Clone de repository:
git clone https://github.com/jouw-gebruikersnaam/laravel-gastenboek.git
cd laravel-gastenboek


Installeer afhankelijkheden:
composer install
npm install


Configureer de omgeving:

Kopieer .env.example naar .env:cp .env.example .env


Stel je databaseverbinding in in het .env-bestand:DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=gastenboek
DB_USERNAME=jouw_gebruikersnaam
DB_PASSWORD=jouw_wachtwoord




Genereer een applicatiesleutel:
php artisan key:generate


Voer database-migraties uit:
php artisan migrate


(Optioneel) Seed de database:

Voor testdata kun je de database seeden:php artisan db:seed




Compileer frontend-assets:
npm run dev


Start de ontwikkelingsserver:
php artisan serve

Open de applicatie in je browser op http://localhost:8000.


Gebruik

Registreren: Ga naar /register om een nieuw account aan te maken.
Inloggen: Ga naar /login om in te loggen.
Berichten aanmaken: Na inloggen kun je op de gastenboekpagina een nieuw bericht plaatsen.
Berichten wijzigen/verwijderen: Gebruikers zien opties om hun eigen berichten te bewerken of te verwijderen.
Gebruikersbeheer: Beheerders kunnen inloggen en via /admin/users nieuwe gebruikers aanmaken.

Projectstructuur

app/Models: Bevat de modellen zoals User en Post.
app/Http/Controllers: Bevat controllers voor authenticatie, berichten en gebruikersbeheer.
resources/views: Bevat Blade-templates voor de frontend.
database/migrations: Bevat migraties voor de database (gebruikers en berichten).
routes/web.php: Definieert de web-routes voor de applicatie.

Technologieën

Backend: Laravel, PHP
Frontend: Blade, Tailwind CSS (optioneel, afhankelijk van implementatie)
Database: MySQL
Authenticatie: Laravel Breeze of Laravel Sanctum
Autorisatie: Laravel Gate/Policies voor admin-functionaliteiten

Bijdragen

Fork de repository.
Maak een nieuwe branch (git checkout -b feature/nieuwe-functionaliteit).
Commit je wijzigingen (git commit -m 'Nieuwe functionaliteit toegevoegd').
Push naar de branch (git push origin feature/nieuwe-functionaliteit).
Maak een pull-verzoek.

Licentie
Dit project is gelicentieerd onder de MIT-licentie.
Contact
Voor vragen of suggesties, neem contact op via dalil.bellahcen@student.ehb.be.
