# Modul D - Att göra en interaktiv modul

**Tävlingstid för uppgiften: 3h**

![snakegame](/module_D/snake.webp)

I den här modulen skapar du ett interaktivt maskspel. Tanken är densamma som i maskspelet tillverkat av Nokia, men här styr du två maskar samtidigt. Spelet måste se ut och kännas som ett riktigt retrospel.

Spelet ska finnas tillgängligt på URL-adressen: `/spel/maskspel`

## Spelets början

Spelet startar med att man trycker på “Start” -knappen.

## Spelfunktionalitet

I spelet styr spelaren två maskar samtidigt. Den första masken styrs med tangenterna ADWS och den andra med piltangenterna. Masken rör sig i fyra riktningar (uppåt, åt höger, nedåt och åt vänster). I spelet dyker ätbara “äpplen" upp slumpmässigt, genom att äta dem får spelaren poäng och masken växer i längd. När spelaren går över kanten av spelområdet, flyttar masken till motsatt sida av skärmen. Spelet avslutas, när masken stöter på sig själv eller på en annan mask.

## Spelets Slutskärm

Spelet avslutas med en avslutningsskärm, som visar poängen.
Dessutom visas frågan "Vill du spara resultatet?" åt spelaren. Spelaren kan välja "ja" eller "nej":

- Om spelaren väljer "ja", kommer ett namninputfält och en skicka-knapp att visas. Efter att ha angett namnet (obligatoriskt) sparas resultaten i databasen (användarnamn, poäng samt datum och tid), och ett meddelande om framgång visas tillsammans med en "spela igen?" knapp.
- Om spelaren väljer "nej", visas "spela igen?" knappen.

## Hall of Fame Uppdatering

Om spelaren väljer att spara poängen, visas spelarens namn och poäng på spelets Hall of Fame-lista från databasen.

**Vid dagens slut ska du leverera modulerna C och D:**

- En fungerande webbplats som använder en databas.
- Det slutliga GitHub-förrådet.
- En `README.md`-fil som innehåller instruktioner för intranätet och spelet.
