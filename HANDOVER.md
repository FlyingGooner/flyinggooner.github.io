# Handover – 2026-11-14

Till nästa session. Repon: `Stress-control`, `simple-nutrition`, `Football-not-soccer`, `budget-buddy`, `flyinggooner.github.io` (ny), gärna även `FlyingGooner` (profil-README, skapas av användaren) och mall-repot (`template`).

## Regler som gäller (står i varje repos CLAUDE.md)
- Arbeta direkt på huvudgrenen och pusha dit: `master` i simple-nutrition, `main` i övriga. Skapa eller pusha aldrig `ccr-`-grenar.
- Höj patch-versionen i `version.js` vid varje ändring som påverkar appen. Skriv alltid den nya versionen sist i svaret.
- PowerShell finns inte i molnsessionen. Hjälp-texten (`tools/build-help.ps1`) har byggts med ett Python-skript med samma logik. Kör gärna `build-help.ps1` och `tools/test.ps1` lokalt en gång för att kontrollera.

## Gjort i den här sessionen
**Stress control (0.2.44 → 0.2.54)**
- Inställningar fälls ihop när man lämnar fliken (även simple-nutrition 0.14.9).
- Personer: välj Vem utför per tråd, filter (👤-lista först i filterraden) i Trådar och Arkiv.
- Personer som kort med egna egenskaper (`pfields`, gemensamma för alla; värden i `person.v`), arbetstid `h` tim/vecka (dold för Relation = Barn).
- Ny fältsort Val i lista (`choice`, `opts`) och Dagar (`days`: `[datum, jobbade timmar, ansökt, barn-id?]`).
- Ny typ Försäkringskassan 🛟: Vad (lista med FK-ersättningar + egna val), Dagar med timmar borta = arbetsdag (veckotid ÷ 5) − jobbat, bocka ansökt per dag, välj barn per dag.
- Överblick tätare. Datamodellen är version 6 med migreringar; `docs/DATA.md` och `EXPORT_SCHEMA` uppdaterade.

**Presentationer (alla fyra repon + artifacts)**
- Stress control: egna bilder om trådar, Överblick, personer, Försäkringskassan.
- `docs/standard.html` (Små appar, hög nivå) i alla fyra: Stress control bland apparna; nya bilder "Varför backupen alltid har lösenord" (tabell: 8/10/16 slumpade tecken) och "Säkert utan att vara krångligt"; "lösenordet sparas aldrig" → "finns aldrig i filen – bara i telefonen, om du vill". Samma bilder i varje apps `docs/presentation.html`.
- Tidsuppskattningarna är egna överslag: ~10 000 gissningar/s per toppgrafikkort (PBKDF2 600 000 varv), 56 tecken.

**flyinggooner.github.io (nytt)**
- Startsida = Små appar, hög nivå med appkort (Öppna appen / Presentation), ikoner i `icons/`, färg från Stress (lila). README med tabell.

## Att göra
1. **Mall-repot:** för in ändringarna i `template/docs/standard.html` (Stress control bland apparna, de två lösenordsbilderna, raden om lösenordet). Annars skriver `sync-shared.ps1` över dem. Låt gärna skriptet även kopiera till `flyinggooner.github.io/index.html` (startsidan har egna appkort – kopiera bara bilderna, inte Apparna-bilden).
2. **Pages för flyinggooner.github.io:** kontrollera att den är på (`main`, `/ (root)`) och att alla länkar fungerar live. Länkarna använder reponamnen exakt (`/Stress-control/`, `/budget-buddy/`, `/Football-not-soccer/`, `/simple-nutrition/`); äldre texter skriver `stress-control` och `Budget-buddy` – rätta om skiftläget spelar roll.
3. **Profil-README:** när `FlyingGooner/FlyingGooner` finns, skriv en kort README (vem, de fyra apparna, länk till startsidan).
4. **Gamla `ccr-`-grenar** på GitHub (inkl. `ccr-8d43da4c-x94o4n` i Stress-control) kunde inte tas bort härifrån – användaren tar bort dem.
5. **Tester:** `unit.test.js` och `ui.test.js` har inte körts i molnet (kräver testskripten/Edge). Lägg gärna till tester för personer, `pfields`, `choice`, `days` och migreringarna v3–v6.
6. **Idéer som nämnts:** person per delmål; påminnelse om dagar som inte är ansökta.

## Artifacts
- Små appar, hög nivå: https://claude.ai/artifact/YJaDfV7vv1pSD62ptbEP1v (äldre kopia, ej uppdaterad: https://claude.ai/artifact/8rXDbjM54udmeknkoV2ZpX)
- Stress control – presentation: https://claude.ai/artifact/STTFC4B4rn4EuVnJnRpLjF

# Tillägg – 2026-11-15: språkstöd

- Alla fyra appar är tvåspråkiga (svenska källa, engelska via `i18n.js` + `i18n-en.js`). `i18n.js` är samma fil i alla repon (även här, för presentationerna) – för in den i mall-repot.
- Språket väljs i välkomstrutan (överst, före lösenordet) och under Inställningar. Budget buddy har dessutom valbar hemvaluta (`settings.home`, omräkning med `changeHome`).
- Manualer: `docs/MANUAL.en.md` i varje app → engelsk Hjälp (`help-tpl-en` / `help-en:start` / `card-help-en`). `build-help.ps1` bygger båda språken (ej körd här – kör lokalt en gång).
- Presentationer, `standard.html` och startsidan: engelska som standard, språkknapp på första bilden. Ordlistan `presentation-en.js` är samma i alla repon (nyckel = svensk textbit) – ändras en svensk text måste nyckeln ändras också. För in i mall-repot så att `sync-shared.ps1` inte skriver över.
- Alla README är nu på engelska.
