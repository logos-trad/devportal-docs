# Attributi

### service\_name

{% tabs %}
{% tab title="Definizione" %}


<table data-header-hidden><thead><tr><th width="164"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Nome del servizio visualizzato in app</td></tr><tr><td>Tipo</td><td>Stringa</td></tr><tr><td>Obbligatorio</td><td>Sì</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
"Carta d'Identità Elettronica"

"TARI"
{% endtab %}
{% endtabs %}

### **organization\_name**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Nome ente che eroga il servizio</td></tr><tr><td>Tipo</td><td>Stringa</td></tr><tr><td>Obbligatorio</td><td>Sì</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
“Comune di Milano”
{% endtab %}
{% endtabs %}

### **organization\_fiscal\_code**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Codice fiscale dell’ente che eroga il servizio.</td></tr><tr><td>Tipo</td><td>Stringa</td></tr><tr><td>Obbligatorio</td><td>Sì</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
“00907501001”
{% endtab %}
{% endtabs %}

### **department\_name**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Nome dell‘Unità Operativa dell’ente che eroga il servizio</td></tr><tr><td>Tipo</td><td>Stringa</td></tr><tr><td>Obbligatorio</td><td>Sì</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
“Anagrafe”
{% endtab %}
{% endtabs %}

### **authorized\_cidrs**

{% hint style="info" %}
Di default non sono applicate restrizioni, è obbligatorio inserire le restrizioni ip prima del passaggio in produzione.
{% endhint %}

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Lista ip/subnet autorizzate per richiamare il servizio.</td></tr><tr><td>Tipo</td><td>Lista di stringhe</td></tr><tr><td>Obbligatorio</td><td>Sì</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
1.2.3.4/32;2.3.4.5/32
{% endtab %}
{% endtabs %}

### **is\_visible**

{% hint style="warning" %}
In fase di test, è importante impostare il valore a `false`.
{% endhint %}

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Flag che modifica la visibilità del servizio in app. </td></tr><tr><td>Tipo</td><td>Booleano</td></tr><tr><td>Obbligatorio</td><td>Sì</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
false
{% endtab %}
{% endtabs %}

### **max\_allowed\_payment\_amount**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Importo massimo autorizzato nei messaggi associati ad un avviso di pagamento pagoPA. L’importo è inteso in centesimi di euro, cioè come parte intera più due cifre decimali. Ad esempio per impostare una soglia di pagamento di 1500,00 € inserire il valore <code>150000</code>.</td></tr><tr><td>Tipo</td><td>Intero</td></tr><tr><td>Obbligatorio</td><td>Sì, se il servizio prevede l’invio di avvisi di pagamento pagoPA.</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
1000000
{% endtab %}
{% endtabs %}

### **version**

{% hint style="info" %}
Il versionamento è automaticamente gestito dall’infrastruttura di IO e non è necessario inviare questo campo.
{% endhint %}

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Numero di versione del servizio. </td></tr><tr><td>Tipo</td><td>No</td></tr><tr><td>Obbligatorio</td><td>Intero</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
1
{% endtab %}
{% endtabs %}

### **require\_secure\_channels**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td><p>Flag che permette di anonimizzare le notifiche inviate agli utenti (push e email). Il valore predefinito è <code>false</code>.</p><p></p><p><span data-gb-custom-inline data-tag="emoji" data-code="1f514">🔔</span> <strong>Notifica Push</strong></p><p>Se <code>true</code>, il contenuto è generico: "Hai un nuovo messaggio"</p><p></p><p><span data-gb-custom-inline data-tag="emoji" data-code="2709">✉</span> <strong>Email</strong></p><p>Se <code>true</code>, non viene inviata alcuna email, a prescindere dalle preferenze dell'utente.</p></td></tr><tr><td>Tipo</td><td>Booleano</td></tr><tr><td>Obbligatorio</td><td>No</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
false
{% endtab %}
{% endtabs %}

### **service\_id**

{% hint style="info" %}
Questa proprietà non è modificabile ed è considerata in sola lettura.
{% endhint %}

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Identificativo del servizio. È il riferimento da usare come parametro nel path della richiesta per invocare i servizi come <code>Update Service</code> e <code>Upload Service Logo</code>.</td></tr><tr><td>Tipo</td><td>Stringa</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
“01EXPKTF05Z2AWEN0PN99QZE79”
{% endtab %}
{% endtabs %}

### **id**

{% hint style="info" %}
Questa proprietà non è modificabile ed è considerata in sola lettura.
{% endhint %}

{% hint style="warning" %}
Questa proprietà non va inviata nelle request e sarà aggiornata in automatico ad ogni modifica del servizio.
{% endhint %}

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Identificativo versionato del servizio: è la composizione di <code>"service_id"+"version"</code> con zero fill.</td></tr><tr><td>Tipo</td><td>Stringa</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
“01EXPKTF05Z2AWEN0PN99QZE79-0000000000000001”
{% endtab %}
{% endtabs %}

### **authorized\_recipients**

{% hint style="warning" %}
Alla creazione di un servizio è possibile inviare messaggi soltanto al cittadino di test con codice fiscale AAAAAA00A00A000A. Se l’utente è abilitato all’invio a qualsiasi codice fiscale questa restrizione non si applica.
{% endhint %}

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Lista dei codici fiscali a cui il servizio può inviare messaggi.</td></tr><tr><td>Tipo</td><td>Lista di stringhe</td></tr><tr><td>Obbligatorio</td><td>No</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
“AAAAAA00A00A000A”
{% endtab %}
{% endtabs %}

### **primary\_key**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Chiave primaria del servizio da inviare nell’header Ocp-Apim-Subscription-Key. Tramite l’api XXXX sarà generata una nuova chiave primaria. Chiave primaria e secondaria sono equivalenti e sono duplicate per poter effettuare il cambio delle chiavi senza interruzione del servizio.</td></tr><tr><td>Tipo</td><td>stringa</td></tr><tr><td>Obbligatorio</td><td>n.a.</td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
”\_\_YOUR\_API\_KEY\_\_”
{% endtab %}
{% endtabs %}

### **secondary\_key**

{% tabs %}
{% tab title="Definizione" %}
<table data-header-hidden><thead><tr><th width="165"></th><th></th></tr></thead><tbody><tr><td>Descrizione</td><td>Chiave secondaria del servizio da inviare in alternativa alla chiave primaria nell’header Ocp-Apim-Subscription-Key. Tramite l’api XXXX sarà generata una nuova chiave secondaria. Chiave primaria e secondaria sono equivalenti e sono duplicate per poter effettuare il cambio delle chiavi senza interruzione del servizio.</td></tr><tr><td>Tipo</td><td>stringa</td></tr><tr><td>Obbligatorio</td><td></td></tr></tbody></table>
{% endtab %}

{% tab title="Esempio" %}
\_\_YOUR\_API\_KEY\_\_”
{% endtab %}
{% endtabs %}



