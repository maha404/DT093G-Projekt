# Projekt DT093G - Bloggportal

### Välkommen till mitt projekt i kursen DT093G :wave:
Detta projekt skapades som avslutande projekt i kursen DT093G vid Mittuniversitetet. Syftet med projektet var att skapa en Bloggportal med PHP. 
 
### :open_book: Projektöversikt 
Detta repo innehåller en Bloggportal som är designad för både stora och små skärmar. 

### :rocket: Funktioner 
+ **Startsida**: Visar en översikt över de fem senaste inläggen som publicerats på webbplatsen och en lista med användare.
+ **Registrera**: Registrering av en användarkonto sker på denna undersida. 
+ **Inloggning**: Inloggning sker på denna undersida. 
+ **Enskilda inlägg**: Enskilda inlägg går att läsa på en egen undersida där bild och hela texten syns i sin helhet. 
+ **Profil / Användarvy**: Här kan användaren skriva sina inlägg. 
+ **Andra användare vy**: Vid klick på en användare i listan på startsidan kommer den användarens alla inlägg att visas i en egen vy. 

### :wrench: Teknologier och Verktyg 
+ **PHP**: För att bygga upp webbplatsen och kunna kommunicera med databasen. 
+ **MYSQL**: Användes som databas för lagring av användare och blogginlägg.
+ **CSS**: För att designa webbplatsen och skapa responsivitet. 
+ **JavaScript**: För att kunna skapa extra funktionallitet för att gömma eller visa lösenordet vid registrering och inloggning.

### :file_folder: Struktur 
+ **css**: Innehåller en stilfil.
+ **includes/classes**: Innehåller klass-filer för att skapa databas tabellerna. 
+ **js**: Innehåller js-fil för extra funktionallitet.
+ **rotmappen**: php-filer för alla undersidor.

### :star: Vidareutveckling / Förbättrnignar 
+ Lägga till funktionallitet för att kunna kategorisera inläggen.
+ Implementation av något frontend-ramverk.
+ Omstrukturering av filer & mappar.
+ Skapa en mer utförlig profil för användarna (Ändra lösenord, profilbild m.m). 
+ Lägga till kommentar funktion.
+ Lägga till lika & dela funktion.

### :gear: Installation och körning 
För att köra projektet lokalt, följ dessa steg:
1. Klona ner repot:

    `git clone https://github.com/maha404/Webbutvecklings-programmet/tree/main/DT093G/Projekt`

2. Se till att XAMPP eller en liknande Apache-distribution finns installerad.Detta krävs för att kunna köra Apache-servern och MySQL-databasen.

3. Flytta den klonade projektmappen till htdocs-mappen i din XAMPP-installation. 

4. Öppna XAMPP Control Panel och starta Apache och MySQL.

5. Öppna "phpMyAdmin" och skapa en användarprofil för databasen. Döp profilen och tillhörande databas till "blogportal".

6. Kör sedan installations filer som finns för databastabellerna: 
    + http://localhost/DT093G/Projekt/includes/classes/blogpost.class.php
    + http://localhost/DT093G/Projekt/includes/classes/user.class.php

7. Skriv sedan: `ALTER TABLE blog ADD FOREIGN KEY (user_id) REFERENCES user(user_id)` i phpMyAdmin under "SQL".

Webbplatsen finns nu tillgänglig på `http://localhost/DT093G/Projekt/`.