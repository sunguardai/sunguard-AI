# sunguard-AIAssistente intelligente per la consulenza degli occhiali da sole

SunGuard è un assistente virtuale progettato per supportare una prima
consulenza orientativa nella scelta degli occhiali da sole. Attraverso
una conversazione, raccoglie informazioni sulle caratteristiche visive
dichiarate dall’utente, sulle sue abitudini e sugli ambienti in cui
utilizza gli occhiali, per elaborare suggerimenti personalizzati sulle
lenti solari.

> **Nota:** SunGuard fornisce indicazioni informative e orientative.
> Non effettua diagnosi, non sostituisce una valutazione professionale e
> non rilascia prescrizioni ottiche.

────────

📌 Demo del progetto

• Prova la chat SunGuard: [INSERISCI QUI IL LINK ALLA CHAT]
• Guarda il video dimostrativo: [INSERISCI QUI IL LINK AL VIDEO]

Sostituisci i due segnaposto con i link effettivi prima di pubblicare il
repository.

────────

🎯 Obiettivo

L’obiettivo del progetto è realizzare un agente AI in grado di guidare
l’utente nella scelta orientativa di occhiali da sole, tenendo conto di:

• Ametropia dichiarata: miopia, ipermetropia, astigmatismo o
presbiopia.
• Valori della prescrizione, se disponibili.
• Abitudini quotidiane e tempo trascorso all’aperto.
• Ambienti di utilizzo, come città, mare, montagna o guida.
• Sensibilità dichiarata alla luce e all’abbagliamento.
• Preferenze e necessità relative alle caratteristiche delle lenti.

✨ Funzionalità

L’assistente è progettato per:

1. Dialogare con l’utente e raccogliere le informazioni necessarie
tramite domande progressive.
2. Considerare l’ametropia dichiarata, senza formulare diagnosi o
modificare i valori della prescrizione.
3. Spiegare la risposta dell’occhio alla luce, includendo il ruolo
della pupilla, della retina, dei coni e dei bastoncelli e
dell’adattamento luminoso.
4. Illustrare le categorie dei filtri solari dalla categoria 0 alla
categoria 4 e i relativi intervalli di trasmissione luminosa.
5. Valutare le caratteristiche delle lenti, come polarizzazione,
fotocromia, specchiatura e colorazione.
6. Considerare la protezione UV, distinguendola dalla categoria del
filtro solare.
7. Elaborare una proposta orientativa coerente con le informazioni
raccolte.
8. Generare una scheda riepilogativa da sottoporre a un ottico
qualificato.

🧠 Tecnologie e componenti

Il workflow è pensato per essere realizzato con n8n, piattaforma per
la creazione di automazioni e flussi di lavoro.

────────

Componente                          Funzione

────────

Chat Trigger                        Riceve i messaggi inviati
dall’utente e avvia la
conversazione.

AI Agent                            Gestisce il dialogo, interpreta le
risposte e prepara la consulenza.

Chat Model                          Fornisce il modello linguistico
utilizzato dall’agente.

Memory                              Può mantenere il contesto della
conversazione tra i messaggi.

Knowledge Base                      Può contenere documentazione tecnica di riferimento su ottica, fisiologia visiva e filtri solari.

> I componenti elencati descrivono l’architettura prevista. Indica come
> effettivamente implementati soltanto quelli presenti nel workflow del
> progetto.

⚙️ Come funziona

Il processo di consulenza segue queste fasi:

1. L’utente avvia la chat.
2. Il Chat Trigger riceve il primo messaggio.
3. L’AI Agent presenta il servizio e pone alcune domande.
4. L’utente comunica, se li conosce, il proprio difetto visivo e i
valori della prescrizione, oltre alle abitudini e agli ambienti di
utilizzo.
5. L’agente considera le informazioni raccolte e le conoscenze
disponibili sui filtri solari e sulle caratteristiche delle lenti.
6. L’assistente propone una soluzione orientativa e ne spiega le
motivazioni.
7. Al termine, genera una scheda riepilogativa da portare all’ottico
per la verifica.

🕶️ Categorie dei filtri solari

Le categorie dei filtri solari sono definite in base alla quantità di
luce visibile trasmessa dalla lente.

────────

Categoria                    Trasmissione luminosa Indicazione generale

────────

0                                   80–100% circa Lenti molto chiare,
per luminosità molto
contenuta.

1                                    43–80% circa Lenti chiare, per
luminosità ridotta.

2                                    18–43% circa Lenti medio-scure,
per luminosità solare
normale.

3                                     8–18% circa Lenti scure, per
forte luminosità.

4                                      3–8% circa Lenti molto scure, per luminosità estrema; non adatte alla guida.

Gli intervalli sono indicativi e devono essere verificati rispetto alla
norma tecnica applicabile e alle specifiche del prodotto.

Attenzione: la categoria del filtro descrive la trasmissione della
luce visibile e non determina, da sola, il livello di protezione dai
raggi ultravioletti. La protezione UVA e UVB deve essere verificata
separatamente attraverso le caratteristiche dichiarate e la conformità
del prodotto.

👁️ Argomenti di ottica considerati

Ametropie

• Miopia: difficoltà nella visione da lontano.
• Ipermetropia: può richiedere uno sforzo accomodativo, in
particolare nel lavoro da vicino.
• Astigmatismo: può causare visione sfocata o distorta ed è
corretto considerando il potere cilindrico e il relativo asse.
• Presbiopia: riduzione progressiva della capacità di
accomodazione, legata all’età.

Fisiologia e luce

L’assistente considera alcuni principi di base:

• La pupilla si restringe in presenza di molta luce (miosi) e si
dilata in condizioni di scarsa illuminazione (midriasi).
• I coni contribuiscono alla percezione dei colori e dei dettagli in
condizioni di buona illuminazione.
• I bastoncelli sono importanti per la visione in condizioni di scarsa
illuminazione.
• L’occhio necessita di tempo per adattarsi ai cambiamenti di
luminosità.
• La riduzione della luminosità visibile non equivale automaticamente
alla protezione dai raggi UV.

Tipologie di lenti

L’agente può considerare, in base alle esigenze dichiarate:

• Polarizzate: riducono determinati riflessi provenienti da
superfici come acqua e asfalto.
• Fotocromatiche: variano la propria trasmissione luminosa in
risposta alle condizioni ambientali; il comportamento può cambiare
all’interno dell’automobile.
• Specchiate: presentano un trattamento superficiale riflettente;
la specchiatura non sostituisce la protezione UV.
• Degradanti: presentano una colorazione che varia lungo la lente.
• Colorazioni grigie, marroni e verdi: possono offrire diverse
caratteristiche di percezione cromatica e contrasto, da valutare in
base all’utilizzo.

📄 Esempio di scheda finale

Al termine della conversazione, l’assistente prepara una scheda
riepilogativa strutturata in questo modo:

Scheda di consulenza occhiali da sole

────────

Sezione                             Informazioni

────────

Dati del cliente                    Nome facoltativo e ametropia
dichiarata

Prescrizione                        SPH, CYL, AX ed eventuale ADD, se
forniti

Abitudini                           Attività quotidiane e ambienti di
utilizzo

Filtro solare                       Categoria suggerita e trasmissione
luminosa

Colorazione                         Tipologia di colore suggerita e
motivazione

Caratteristiche                     Lenti graduate, polarizzate,
fotocromatiche o specchiate

Protezione UV                       Da verificare sulle specifiche del
prodotto

Indicazioni per l’ottico            Parametri da controllare e aspetti da approfondire

I valori non comunicati dall’utente devono essere indicati come “Da
verificare con l’ottico”. L’assistente non deve inventare né calcolare
una prescrizione.

🛡️ Sicurezza e limiti

SunGuard è uno strumento di supporto informativo e non sostituisce il
lavoro dei professionisti della vista.

• Non formula diagnosi.
• Non stabilisce autonomamente un’ametropia.
• Non modifica e non inventa valori refrattivi.
• Non sostituisce una prescrizione aggiornata.
• Non confonde la categoria del filtro con la protezione UV.
• Non consiglia filtri di categoria 4 per la guida.
• Invita l’utente a rivolgersi a un professionista in caso di sintomi
visivi nuovi, importanti o persistenti.
• La scelta definitiva delle lenti e la verifica della prescrizione
spettano a un professionista qualificato.

📚 Riferimenti tecnici

Per la documentazione e l’aggiornamento delle conoscenze del progetto,
fare riferimento a fonti tecniche affidabili, tra cui:

• Norma EN ISO 12312-1, relativa agli occhiali da sole per uso
generale.
• Documentazione tecnica dei produttori di lenti e filtri solari.
• Materiale didattico e testi di ottica oftalmica, fisiologia oculare
e optometria.

Verificare sempre l’edizione vigente delle norme e le specifiche dei
singoli prodotti prima di utilizzare i dati in una consulenza.

────────

🚀 Conclusione

SunGuard unisce intelligenza artificiale e conoscenze di ottica per
rendere più semplice e accessibile la fase iniziale di orientamento
nella scelta degli occhiali da sole.

Il progetto mostra come un agente AI realizzato con n8n possa
raccogliere esigenze, organizzare informazioni tecniche e produrre un
riepilogo utile per il successivo confronto con l’ottico.

────────

Progetto SunGuard — Assistente intelligente per la consulenza degli
occhiali da sole.
