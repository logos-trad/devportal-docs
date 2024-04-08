# Residenza

Erogare il servizio tramite l'app IO permette agli enti di:

* fornire alle cittadine e ai cittadini un riferimento per la ricezione delle comunicazioni riguardanti le richieste di residenza e di cambio di residenza;
* monitorare e gestire tempestivamente le richieste, le comunicazioni e i pagamenti per l’erogazione del servizio.

[**Scopri tutti i benefici di integrarsi con IO →** ](https://docs.pagopa.it/manuale-servizi/lapp-io/cose-io-e-qual-e-il-suo-obiettivo)

## Scheda servizio <a href="#scheda-servizio" id="scheda-servizio"></a>

<table data-header-hidden><thead><tr><th width="373"></th><th></th></tr></thead><tbody><tr><td><strong>Nome servizio</strong></td><td>Residenza</td></tr><tr><td><strong>Argomento</strong></td><td>Servizi anagrafici e civici</td></tr><tr><td><strong>Descrizione del servizio</strong></td><td><p>Il servizio riguarda le richieste di residenza e di cambio di residenza.<br><br>Tramite IO potrai:</p><ul><li>ricevere comunicazioni e aggiornamenti sulle richieste presentate;</li><li>ricevere altre comunicazioni.</li></ul></td></tr><tr><td><strong>Pulsante</strong></td><td>Vai alla modulistica</td></tr></tbody></table>

## Ciclo di vita del servizio

<figure><img src="../.gitbook/assets/Servizi anagrafici_Residenza.png" alt=""><figcaption><p><strong>Ciclo di vita ed eventi del servizio Residenza</strong></p></figcaption></figure>

## Messaggi del servizio

{% hint style="success" %}
**Il servizio ideale**

L'insieme di tutti i messaggi rappresenta il servizio ideale. L'ente che intende erogare questo servizio può valutare quali e quanti messaggi inviare, in base alle proprie possibilità di integrazione. L'obiettivo finale rimane quello di inviarli tutti, rilasciando in maniera iterativa versioni del servizio sempre più complete.
{% endhint %}

## Richiesta di residenza, cambio di residenza, cancellazione di residenza

### Analisi documentazione

<details>

<summary>Richiesta di residenza, cambio, cancellazione: avviamento del procedimento</summary>

**🖋 Titolo del messaggio:** \<Cambio/Cancellazione/Richiesta> di residenza in corso

🗒 **Testo del messaggio**:&#x20;

Abbiamo avviato il procedimento per la tua richiesta di \<cambio/cancellazione/residenza>.

Il numero di pratica è: \<nnnn>.

**🪄 Pulsante**: Gestisci la tua richiesta

***

**Destinatari**: Tutte le persone che hanno presentato richiesta, cambio o cancellazione di residenza.

**Quando inviarlo**: Quando l’ente prende in carico la pratica e avvia il procedimento.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

<details>

<summary>Richiesta di residenza, cambio, cancellazione: integrazione documentazione</summary>

**🖋 Titolo del messaggio:** Richiesta di integrazione

🗒 **Testo del messaggio**:&#x20;

Per elaborare la tua \<richiesta di cambio/richiesta di cancellazione/richiesta> di residenza, abbiamo bisogno di ricevere entro il \<gg/mm/aaaa> altri documenti.

Consulta il riepilogo della tua richiesta, \[visita questo sito]\(URL).

**🪄 Pulsante**: Aggiungi documenti

***

**Destinatari**: Tutte le persone che hanno presentato richiesta, cambio o cancellazione di residenza.

**Quando inviarlo**: Quando l’ente ha bisogno di ulteriori documenti per l’elaborazione della richiesta.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

### Chiusura pratica

<details>

<summary>Avvenuto cambio di residenza (da altro comune o dall’estero)</summary>

**🖋 Titolo del messaggio:** Avvenuto cambio di residenza

🗒 **Testo del messaggio**:&#x20;

Ti diamo il benvenuto nel Comune di \<Comune>.

Nei prossimi \<nn> giorni un messo comunale o un agente della Polizia locale verrà presso la tua abitazione per l’accertamento della residenza.

Se non lo hai già fatto, aggiorna la tua dichiarazione TARI (Tassa sui Rifiuti). Per farlo, \[visita questo sito]\(URL).

Per ulteriori informazioni, \[visita questo sito]\(URL).

**🪄 Pulsante**: n/a

***

**Destinatari**: Tutte le persone che hanno presentato richiesta e cambio di residenza.

**Quando inviarlo**: Quando l’ente effettua l’iscrizione anagrafica.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

<details>

<summary>Avvenuta cancellazione di residenza</summary>

**🖋 Titolo del messaggio:** Avvenuta cancellazione di residenza

🗒 **Testo del messaggio**:&#x20;

Il \<gg/mm/aaaa> abbiamo provveduto a cancellare la tua residenza presso il Comune di \<Comune>.

Se non lo hai già fatto, aggiorna la tua dichiarazione TARI (Tassa sui Rifiuti). Per aggiornare la dichiarazione TARI \[visita questo sito]\(URL).

Per ulteriori informazioni, \[visita questo sito]\(URL).

**🪄 Pulsante**: n/a

***

**Destinatari**: Tutte le persone che hanno presentato richiesta di cancellazione residenza.

**Quando inviarlo**: Quando l’ente effettua l’iscrizione anagrafica.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

<details>

<summary>Richiesta di residenza, cambio, cancellazione: non accolta</summary>

**🖋 Titolo del messaggio:** Richiesta di \<cambio/cancellazione/residenza> non accolta

🗒 **Testo del messaggio**:&#x20;

La tua \<richiesta di cambio/richiesta di cancellazione/richiesta> di residenza non è stata accolta.

Per ulteriori informazioni, \[visita questa pagina]\(URL).

**🪄 Pulsante**: n/a

***

**Destinatari**: Tutte le persone che hanno presentato richiesta, cambio o cancellazione di residenza.

**Quando inviarlo**: Quando l’ente identifica ragioni ostative al completamento della richiesta.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

***

## Residenza temporanea

### Iscrizione

<details>

<summary>Richiesta di residenza temporanea: accolta</summary>

**🖋 Titolo del messaggio:** Iscrizione della residenza temporanea

🗒 **Testo del messaggio**:&#x20;

La tua richiesta di residenza temporanea presso il Comune di \<Comune> è stata accolta.

Per ulteriori informazioni, \[visita questa pagina]\(URL).

**🪄 Pulsante**: n/a

***

**Destinatari**: Tutte le persone che hanno presentato richiesta di iscrizione al registro dell’anagrafe temporanea.

**Quando inviarlo**: Quando l’ente comunica l’iscrizione al registro dell’anagrafe temporanea.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

<details>

<summary>Richiesta di residenza temporanea: non accolta</summary>

**🖋 Titolo del messaggio:** Richiesta di residenza non accolta

🗒 **Testo del messaggio**:&#x20;

La tua richiesta di residenza temporanea non è stata accolta.

Per ulteriori informazioni, \[visita questa pagina]\(URL).

**🪄 Pulsante**: n/a

***

**Destinatari**: Tutte le persone che hanno presentato richiesta di iscrizione al registro dell’anagrafe temporanea.

**Quando inviarlo**: Quando l’ente identifica ragioni ostative al completamento della richiesta.

**User story**: Come cittadino voglio ricevere aggiornamenti sullo stato della mia richiesta.

</details>

***

{% hint style="success" %}
**Lo sapevi?**\
IO è integrata con SEND - Servizio Notifiche Digitale, per l'invio di comunicazioni a valore legale.

[**Scopri di più su SEND**](https://notifichedigitali.pagopa.it/) [**-->**](https://www.pagopa.it/it/prodotti-e-servizi/piattaforma-notifiche-digitali)
{% endhint %}

{% hint style="info" %}
**Un modello da personalizzare**

Le procedure di questo servizio variano molto da ente a ente. Consigliamo di utilizzare i testi dei messaggi come un punto di partenza e di aggiungere ulteriori informazioni.&#x20;

Il modello è un esempio che non ha carattere vincolante per l’ente e sul quale la Società declina qualsiasi responsabilità, avendo valore esemplificativo.

Puoi copiare i testi dei messaggi da personalizzare da questo documento:

{% file src="../.gitbook/assets/IO - Template servizi - Residenza.xlsx" %}
{% endhint %}
