# Modul C - Implementering av ett intranät för webbplatsen

**Tävlingstid för uppgiften: 3h**

I denna modul ska ett intranät/administrationsverktyg implementeras på en tidigare skapad webbplats med användning av en databas. Intranätets huvudsyfte är att hantera Hall of Fame-spel, deras deltagare och resultat. All data måste komma från databasen, och du måste skapa alla nödvändiga databastabeller. Du måste etablera en säker och skyddad databasanslutning, inklusive kryptering med exempelvis Argon2-algoritmen.

Koden måste vara av hög kvalitet och underhållbar för vidareutveckling. Den ska vara koncis, enkel och använda tekniker som gör den lättläst, lätt att analysera och förstå. Se till att du lägger till tydliga instruktioner för att använda intranätet i readme-filen.

Observera att denna modul utförs samtidigt med följande modul och resultaten av denna modul måste levereras i slutet av tävlingsdagen.

- Intranätet är tillgängligt på `/admin`
- Inloggning är tillgänglig på `/login`

## Inloggning

Åtkomst till intranätsidan är endast möjlig genom att logga in via inloggningssidan. Om någon navigerar till intranätets URL utan att logga in, kommer de att omdirigeras till inloggningssidan. När man har loggat in, visas användarnamnet och utloggningsknappen i huvudmenyn. Inloggningsformulärets uppgifter måste valideras innan formuläret skickas.

Följande inloggningsuppgifter ska användas:

- **admin** med lösenordet **taitaja2024** – administratörsroll
- **user** med lösenordet **taitaja2024** – användare med läs-/skrivbehörighet

## Intranät

På intranätet kan administratören se alla registrerade användare och lägga till, redigera och ta bort användare. Dessutom kan administratörer se alla Hall of Fame-spel och evenemang samt lägga till och redigera spel/evenemang. Användare kan se sin egen profil och de spel de har rätt att ändra.

## Användarroller

- admin (superanvändare)
- användare med skriv-/läsbehörigheter (user)

**Admin Kan:**

- logga in och ut
- lägga till nya användare
  - standardlösenordet för en ny användare är 'taitaja2024'
- redigera användarlösenord
- ta bort användare
- lägga till nya spel/evenemang
  - nödvändig information vid skapande av ett nytt spel är titel (obligatorisk), bild (valfri), standardtidsstämpel vid skapande för datum och antalet resultat som visas på Hall of Fame-sidan
- redigera speltitel, bild, datum och antalet visade resultat
- lägga till användare till varje spel som har rätt att lägga till och redigera spelresultat

## Användare Kan:

- logga in och ut
- redigera sitt eget lösenord
- lägga till och redigera deltagare, resultat och antalet resultat som visas på spel-/evenemangets Hall of Fame-sida för varje spel
