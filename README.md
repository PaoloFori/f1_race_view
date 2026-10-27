# F1 Race View

Dashboard da affiancare allo streaming: mappa del circuito con piloti (posizione + sigla), classifica con gomme e pit stop, passo gara, strategia, velocità e previsioni. Dati: [OpenF1](https://openf1.org) (gare dal 2023; live con abbonamento sponsor).

Funziona su PC, telefono e TV dallo stesso link.

## Pubblicarla su GitHub Pages (5 minuti, gratis)

1. Su github.com → **New repository** → nome `f1-race-view` → **Public** → *Create repository*.
2. Nella pagina del repo: **Add file → Upload files** → trascina **tutti i file di questa cartella** (index.html, manifest.webmanifest, sw.js, icon.svg, icon-192.png, icon-512.png) → *Commit changes*.
3. **Settings → Pages** → *Source: Deploy from a branch* → Branch `main`, cartella `/ (root)` → *Save*.
4. Dopo 1–2 minuti l'app è su `https://<tuo-utente>.github.io/f1-race-view/`.

Per aggiornarla basta ricaricare i file (stesso procedimento del punto 2).

## Telefono

- **Android (Chrome):** apri il link → menu ⋮ → *Installa app* / *Aggiungi a schermata Home*.
- **iPhone (Safari):** apri il link → Condividi → *Aggiungi alla schermata Home*.
- Si apre a schermo intero come un'app. In verticale: mappa, poi classifica, poi analisi; tocca un grafico per i valori.

## TV

- **Samsung / LG / altre smart TV:** apri il browser della TV e vai al link (salvalo nei preferiti). La modalità TV si attiva da sola; se non succede, premi il pulsante **📺 TV** oppure apri il link con `?tv=1` alla fine.
- **Android TV / Google TV / Chromecast con Google TV:** usa un browser (es. TV Bro) col link, oppure installala come app (vedi sotto).
- **Fire TV:** browser Silk o Amazon Internet col link.
- **Telecomando:** frecce = sposti la selezione · OK = conferma · Indietro = chiude finestre / deseleziona il pilota · Play/Pausa, ⏩ e ⏪ se il telecomando li ha. Sulla barra del tempo ← → saltano di 30 s, sullo slider del ritardo di 1 s.
- Consiglio: TV con lo streaming e la dashboard su un secondo schermo (tablet, PC o una seconda TV), oppure picture-in-picture se la TV lo supporta.

## Gara, Qualifiche, Live

In alto scegli **Gara**, **Qualifiche** o **Live**.

- **Qualifiche:** scegli il weekend e premi *Carica*. Classifica con tempo, mescola e stato (PUSH / OUT / IN / BOX), linee di eliminazione Q1/Q2/Q3, mappa con solo le auto in pista (le altre sono semitrasparenti). Schede: **Tempi** (Q1/Q2/Q3 per pilota), **Settori** (migliori settori e giro ideale), **Evoluzione pista** (tutti i giri lanciati nel tempo), **Tentativi & gomme**, **Velocità**. I pulsanti Q1/Q2/Q3 in basso saltano alla fase e le pause tra le fasi vengono saltate da sole.
- **Live:** mostra il conto alla rovescia della prossima sessione (prove, qualifiche o gara) con il calendario del weekend. L'app si collega da sola 15 minuti prima dell'inizio, basta tenerla aperta.

Il live richiede l'abbonamento sponsor di OpenF1 (9,90 €/mese, si gestisce da openf1.org): al primo accesso inserisci username e password (o un token). Senza credenziali puoi usare *Solo conto alla rovescia*. Regola **Ritardo sullo streaming** finché la mappa coincide con le immagini di Sky/NOW (di solito 30–60 s). Sulla TV puoi spuntare *Ricorda le credenziali*: vengono salvate solo su quel dispositivo, quindi fallo solo su dispositivi tuoi.

Nota: le qualifiche sono state provate solo con dati simulati; sui dati reali di OpenF1 potrebbero servire piccoli ritocchi (per esempio nel riconoscere la fine delle fasi o i giri cancellati).

## Volendo: app vera per Android TV

L'app è una PWA, quindi si può impacchettare come APK senza riscriverla: su [pwabuilder.com](https://www.pwabuilder.com) incolla il link GitHub Pages → *Package for stores → Android* → scarichi l'APK e lo installi sulla TV (es. con *Downloader* o *Send Files to TV*). Per Samsung (Tizen) e LG (webOS) serve il rispettivo SDK: si può fare in un secondo momento partendo da questi stessi file.
