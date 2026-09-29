# U.S.D. Oratorio San Michele – App presenze (versione locale)

Nessun server e nessun account da configurare: i dati restano nel browser del dispositivo.

## Pubblicare su GitHub Pages
1. Crea un repository su GitHub e carica **tutti** i file di questa cartella.
2. **Settings → Pages → Deploy from a branch → `main` / `(root)` → Save**.
3. Dopo un minuto l'app è su `https://TUO-UTENTE.github.io/NOME-REPO/`.

## Primo avvio
Alla prima apertura l'app chiede di creare l'Admin. Poi da **Utenti** l'Admin crea gli altri profili.

## Impostazioni (solo Admin, icona ⚙ in alto a destra)
- Cambia nome e logo della società.
- Importa l'anagrafica da un file `.xlsx` o `.csv` (colonne Nome, Cognome, Data di nascita, Categoria facoltativa). Dal pulsante "Scarica modello" ottieni un file d'esempio.

## Avviso di nuova versione
L'app controlla il file `version.json` sul sito. Se lì c'è una versione più alta di quella in uso, mostra un banner giallo con versione in uso e nuova versione e il pulsante "Aggiorna ora". Per pubblicare un aggiornamento carica su GitHub tutti i file della nuova versione, `version.json` compreso.

## Cose importanti
- I dati sono **solo su quel dispositivo e quel browser**: un altro telefono vede un'app vuota. Usate un unico dispositivo condiviso (es. un tablet) e fate accedere lì i vari utenti.
- Installa l'app (Android: menù ⋮ → Installa app; iPhone: Condividi → Aggiungi alla schermata Home): riduce il rischio che il browser cancelli i dati.
- **Fai backup spesso**: Admin → "Salva backup" scarica un file; "Ripristina backup" lo ricarica (anche su un altro dispositivo).
- La protezione degli accessi è quella dell'interfaccia: adatta a un uso interno semplice, non a dati sensibili.
- Quando vorrai i dati condivisi tra più telefoni, servirà passare alla versione con Firebase (l'altra cartella).
- Se aggiorni i file, cambia il numero di versione in `sw.js` (es. `osm-local-v1.03`) e in `index.html` (`VER`) e in `version.json`.
