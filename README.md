# Ping Pong

Gioco del ping pong minimale, da giocare da soli contro il computer o in 2 sullo stesso dispositivo.

## Come si gioca

Apri `index.html` nel browser e gioca: non serve installare niente.

- Dal menu scegli **1 giocatore** (contro il computer, che sta in alto) o **2 giocatori**.
- Campo verticale: il Giocatore 1 sta in basso, il Giocatore 2 (o il computer) in alto.
- Si gioca fino a 11 con 2 punti di scarto. Il servizio cambia ogni 2 punti, e a ogni punto dal 10-10.
- Il tasto di servizio serve solo a battere; durante lo scambio la palla rimbalza da sola sulle racchette.
- Il punto in cui la palla colpisce la racchetta decide l'angolo, e la palla accelera a ogni colpo.

**Con la tastiera:** ogni giocatore ha tre tasti, sinistra, destra e servizio, che si cambiano dal menu (clicca il tasto e premi quello nuovo). Predefiniti: Giocatore 1 `A` / `D` / `W`, Giocatore 2 `←` / `→` / `↓`. `Esc` torna al menu.

**Con il touch:** trascina il dito nella tua metà del campo per muovere la racchetta e sollevalo per servire. Il pulsante Menu (o il tasto Indietro su Android) torna al menu.

## App Android

La cartella `android/` contiene una piccola app che mostra il gioco a schermo intero.
GitHub Actions compila l'APK a ogni modifica:

- su `main` l'APK viene pubblicato nella release [apk](../../releases/tag/apk), da cui si scarica direttamente dal telefono;
- su ogni pull request l'APK si trova tra gli artifact della build.

Per installarlo bisogna permettere l'installazione da origini sconosciute. Per compilarlo in locale serve l'Android SDK: `gradle -p android assembleDebug`.
