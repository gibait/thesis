# Sviluppo prototipale di una soluzione survivable per autenticatori hardware FIDO

Il Single Sign-On è un protocollo utilizzato per migliorare e semplificare il processo di autenticazione. Esso alleggerisce i servizi Web che lo utilizzano dall'onere di gestire la moltitudine di credenziali degli utenti, con i meccanismi di protezione necessari che ne conseguono. I protocolli di SSO consentono l'autenticazione passwordless degli utenti: grazie ad essi l'utente è in grado di eseguire operazioni di autenticazione basate su crittografia asimmetrica tramite un token hardware. Questo permette allo stesso tempo di semplificare e irrobustire il processo complessivo di autenticazione. Il limite principale risiede nella centralizzazione del protocollo SSO, che non è in grado di tollerare intrusioni nell'infrastruttura che lo esegue.
Infatti, come mostrano attacchi recenti, attaccanti che riescono a compromettere l'infrastruttura di SSO sono in grado di impersonare utenti arbitrari.
Per mitigare questa problematica sono nati gli studi sulla cosiddetta SSO survivability. Tale filone si pone l'obiettivo di sviluppare un approccio distribuito e replicato per il protocollo SSO. Si prevede un numero di attori malevoli di cui è possibile tollerare l'intromissione, numero da cui dipende il livello di sicurezza.

L'esigenza di questa tesi nasce dal fatto che i protocolli esistenti in ambito SSO survivable non permettono di modificare il livello di sicurezza una volta che è stato stabilito durante la fase di creazione dell'infrastruttura. Questo impedisce ai vari servizi Web di richiedere alla stessa infrastruttura SSO livelli di sicurezza adeguati alle caratteristiche del servizio offerto. Si è affrontato dunque il problema dell'integrazione del livello di sicurezza all'interno dei protocolli Passwordless e SSO preesistenti. A tal fine, si è reso necessario implementare modifiche al codice di un autenticatore open source, cui hanno fatto seguito verifiche delle performance di autenticazione e un breve studio di fattibilità per l'implementazione su hardware reale.

## Repository
- Codice Solo: [solo1](https://github.com/gibait/solo1) 
- Codice Server (*privato*): [survivable-fido](https://github.com/Fedma123/survivable-fido)
