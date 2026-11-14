# flyinggooner.github.io

Startsida för mina appar: **[flyinggooner.github.io](https://flyinggooner.github.io/)**.

| App | Vad den gör |
|---|---|
| [Simple nutrition](https://flyinggooner.github.io/simple-nutrition/) | Vanor först – kalorier som stöd när du vill. |
| [Budget buddy](https://flyinggooner.github.io/budget-buddy/) | Planera ekonomin månad för månad. |
| [Football, not soccer](https://flyinggooner.github.io/Football-not-soccer/) | Tabellen, matcherna och ditt lag. |
| [Stress kontroll](https://flyinggooner.github.io/Stress-control/) | Skriv ner det som snurrar – och släpp det. |

**[Grunder och filosofi](https://flyinggooner.github.io/presentation.html)** – hela presentationen om varför apparna finns och vad de delar.

### Varför appen ber om ett lösenord direkt

Apparna har inget konto och ingen server – datan finns bara i telefonen. Backup-filen är därför det enda som räddar den om telefonen tappas eller webbläsaren rensas. Lösenordet är ingen inloggning: det skickas ingenstans, det är bara nyckeln som låser backup-filen. Appen ber om det från start så att backup sedan blir ett enda tryck.

**Så går backupen till**
1. **Första start:** tryck *Skapa slumpmässigt lösenord* (eller skriv ett eget) och spara det i din lösenordshanterare. Telefonen kommer ihåg det. Har du redan en backup kan du läsa in den i stället.
2. **Spara:** Inställningar → Data → *Spara backup-fil*. Filen är krypterad (AES-256) – lägg den i molnet, mejlen eller på datorn.
3. **Påminnelse:** appen säger till varje månad.
4. **Ny telefon:** *Läs in backup-fil*, skriv lösenordet, kontrollera sammanfattningen och tryck *Ersätt*. Ångra finns direkt efteråt.

Lösenordet finns aldrig i filen. Utan det går backupen inte att öppna.

Alla appar är byggda från samma mall: ingen inloggning, ingen server, din data stannar i telefonen och backupen är låst med lösenord.

Sidan är ren HTML/CSS/JS utan beroenden. Texten om mallen kommer från `template/docs/standard.html`.
