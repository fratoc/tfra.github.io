# Privacy Policy di Alertino

Ultimo aggiornamento: 29 maggio 2026

## Titolare del trattamento

Alertino e un'app Android sviluppata e pubblicata da Francesco Toccafondi, email toccafondifrancesco@gmail.com, che funge da titolare del trattamento dei dati personali. L'utente puo contattare il titolare a questo indirizzo email per esercitare i propri diritti o per qualsiasi richiesta relativa alla privacy.

## Descrizione del servizio

Alertino e un'app per la gestione di appuntamenti con promemoria SMS automatici. L'app consente di creare appuntamenti, associarli a contatti della rubrica e inviare SMS di promemoria dalla SIM dell'utente prima dell'appuntamento programmato. L'app funziona interamente in locale sul dispositivo dell'utente.

## Dati personali trattati e finalita

### Dati salvati localmente sul dispositivo

Tutti i dati dell'app sono conservati esclusivamente nella memoria interna del dispositivo dell'utente tramite un database locale (SQLite/Room). Nessun dato viene trasmesso a server remoti, cloud o terze parti. I dati trattati includono:

- **Appuntamenti**: titolo, descrizione, data/ora, durata, note e impostazioni del promemoria SMS. Questi dati sono necessari per fornire la funzionalita principale dell'app.
- **Contatti**: nome, cognome e numero di telefono dei contatti creati dall'utente all'interno dell'app. Sono necessari per associare un destinatario agli appuntamenti e per l'invio degli SMS di promemoria.
- **Log SMS**: registro degli SMS inviati (destinatario, messaggio, stato di invio/consegna, data/ora). Necessario per consentire all'utente di verificare lo storico dei promemoria inviati.
- **Preferenze**: impostazioni dell'app (template SMS, anticipo promemoria, stato permessi). Salvate localmente tramite DataStore.

### Dati letti dal dispositivo (non conservati)

- **Calendario del dispositivo** (permesso READ_CALENDAR): l'app puo leggere gli eventi dal calendario del dispositivo esclusivamente per consentire all'utente di importarli come appuntamenti. Gli eventi del calendario vengono letti solo su richiesta esplicita dell'utente e non vengono conservati separatamente; solo gli eventi che l'utente sceglie di importare vengono salvati come appuntamenti nel database locale dell'app.
- **Rubrica del dispositivo** (permesso READ_CONTACTS): l'app puo leggere i contatti del dispositivo esclusivamente per consentire all'utente di importarli nell'app. I contatti della rubrica vengono letti solo su richiesta esplicita dell'utente.

## Permessi richiesti e relative finalita

Alertino richiede i seguenti permessi Android, ciascuno per una finalita specifica e limitata:

| Permesso | Finalita |
|----------|----------|
| **SEND_SMS** | Invio automatico di SMS promemoria dalla SIM dell'utente al contatto associato a un appuntamento. L'SMS viene inviato solo se l'utente ha abilitato il promemoria per quello specifico appuntamento. |
| **READ_PHONE_STATE** | Verifica della disponibilita della SIM per l'invio SMS. |
| **READ_CALENDAR** | Lettura degli eventi dal calendario del dispositivo per l'importazione volontaria nell'app. |
| **READ_CONTACTS** | Lettura della rubrica del dispositivo per l'importazione volontaria dei contatti nell'app. |
| **POST_NOTIFICATIONS** | Visualizzazione di notifiche locali relative allo stato di invio dei promemoria SMS (Android 13+). |
| **SCHEDULE_EXACT_ALARM / USE_EXACT_ALARM** | Programmazione di sveglie precise per l'invio dei promemoria SMS al momento prestabilito. |
| **RECEIVE_BOOT_COMPLETED** | Riprogrammazione delle sveglie per i promemoria SMS dopo il riavvio del dispositivo. |
| **WAKE_LOCK** | Mantenimento attivo del dispositivo durante l'invio dell'SMS per garantirne l'affidabilita. |

Tutti i permessi sono richiesti all'utente al momento dell'uso della relativa funzionalita, non al primo avvio dell'app. L'utente puo revocare qualsiasi permesso dalle impostazioni del dispositivo in qualsiasi momento; la revoca disabilita la funzionalita correlata ma non pregiudica il funzionamento delle altre parti dell'app.

## Invio SMS

L'invio di SMS avviene direttamente dalla SIM dell'utente tramite le API native di Android. Alertino non utilizza servizi SMS di terze parti, gateway online o server intermedi. L'SMS viene inviato dal numero di telefono dell'utente e il costo dell'SMS e a carico del piano tariffario dell'utente. Lo sviluppatore non ha accesso al contenuto degli SMS inviati ne ai numeri di telefono dei destinatari.

## Raccolta dati da parte dello sviluppatore

Alertino **non raccoglie, trasmette, ne condivide alcun dato personale** con lo sviluppatore o con terze parti. L'app:

- Non utilizza servizi di analytics (es. Google Analytics, Firebase Analytics)
- Non utilizza servizi di crash reporting (es. Firebase Crashlytics)
- Non utilizza servizi pubblicitari (es. Google AdMob)
- Non effettua chiamate di rete di alcun tipo
- Non contiene tracker o SDK di terze parti che raccolgono dati

Tutti i dati risiedono esclusivamente sul dispositivo dell'utente e sotto il suo pieno controllo.

## Backup e trasferimento dati

Se l'utente ha abilitato il backup automatico di Android (Google Backup), i dati dell'app (database appuntamenti e preferenze) possono essere inclusi nel backup del dispositivo gestito da Google. L'utente puo controllare questa funzionalita dalle impostazioni di sistema del dispositivo. Lo sviluppatore non ha accesso ai backup.

## Condivisione dei dati con terze parti

Alertino **non condivide, vende, affitta ne trasferisce dati personali a terze parti** in nessuna circostanza. Non esistono accordi di condivisione dati con fornitori di servizi, inserzionisti o altri soggetti.

## Sicurezza dei dati

I dati dell'app sono protetti dalle misure di sicurezza native di Android (sandboxing delle applicazioni, crittografia del filesystem). L'accesso ai dati e limitato all'app stessa e non e accessibile ad altre applicazioni installate sul dispositivo.

## Conservazione dei dati

I dati vengono conservati sul dispositivo dell'utente fino a quando l'utente non li elimina manualmente dall'app o disinstalla l'applicazione. La disinstallazione dell'app comporta la cancellazione completa di tutti i dati locali.

## Diritti degli utenti

Gli utenti hanno i seguenti diritti in materia di protezione dei dati personali:

- **Diritto di accesso**: tutti i dati sono visibili direttamente nell'app (appuntamenti, contatti, log SMS, impostazioni).
- **Diritto di rettifica**: l'utente puo modificare qualsiasi dato direttamente dall'app.
- **Diritto alla cancellazione**: l'utente puo eliminare singoli appuntamenti, contatti o tutti i dati disinstallando l'app. Puo inoltre contattare lo sviluppatore per assistenza.
- **Diritto di limitazione e opposizione**: poiche i dati sono trattati esclusivamente in locale e sotto il controllo dell'utente, questi diritti sono esercitabili direttamente tramite le funzionalita dell'app e le impostazioni dei permessi del dispositivo.
- **Diritto alla portabilita**: l'utente puo richiedere i propri dati contattando lo sviluppatore.
- **Revoca del consenso**: l'utente puo revocare qualsiasi permesso concesso all'app dalle impostazioni del dispositivo in qualsiasi momento.

**Diritti aggiuntivi per residenti in California (CCPA/CPRA)**: Alertino non raccoglie, vende ne condivide dati personali con terze parti. Non esistono categorie di dati venduti o condivisi. Gli utenti californiani possono comunque contattare lo sviluppatore per esercitare qualsiasi diritto previsto dalla legge.

Per esercitare i propri diritti o per qualsiasi domanda, l'utente puo contattare il titolare del trattamento all'indirizzo email indicato nella sezione "Contatti".

## Minori

Alertino non e rivolta a bambini di eta inferiore ai 16 anni. L'app non raccoglie consapevolmente dati personali da minori. Se un genitore o tutore ritiene che un minore abbia utilizzato l'app, puo contattare lo sviluppatore per richiedere la cancellazione dei dati. Conformemente alle normative COPPA (USA) e al GDPR (UE), invitiamo gli utenti minori di 16 anni a non utilizzare l'app senza il consenso di un genitore o tutore.

## Modifiche alla Privacy Policy

Lo sviluppatore si riserva il diritto di aggiornare questa Privacy Policy. In caso di modifiche sostanziali, la data di "Ultimo aggiornamento" in cima a questa pagina verra aggiornata. L'utente e invitato a consultare periodicamente questa pagina. L'uso continuato dell'app dopo la pubblicazione di eventuali modifiche costituisce accettazione delle stesse.

## Contatti

Per qualsiasi richiesta relativa alla privacy o per esercitare i diritti di cui sopra, scrivere a: **toccafondifrancesco@gmail.com**. Questa email e l'unico contatto ufficiale per questioni di privacy.
