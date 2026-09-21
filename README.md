# -OGD-GTA-V-MODS
My Mods for Grand Theft Auto V
# #OGD GTA V LEGACY MODS PACK — Alpha 1.0

Una raccolta di mod originali **#OGD** per rendere la modalità Storia di **Grand Theft Auto V Legacy** più viva, dettagliata e coinvolgente: popolazione aggiuntiva, danni da collisione, fumo automatico, grafica personalizzata e menu dedicati.

**Versione Alpha:** il progetto è in sviluppo. La compilazione e le verifiche automatiche sono state completate, ma la validazione visiva e del comportamento in gioco è ancora da eseguire. Sono possibili bug, incompatibilità e variazioni delle prestazioni.

## Funzioni principali

- **Traffico e pedoni:** popolazione civile aggiuntiva introdotta gradualmente, con controlli su distanza, spazio e visibilità per limitare ammucchiamenti e apparizioni improvvise.
- **Incidenti:** danni aggiuntivi a carrozzeria e motore in base all'impatto. Il distacco delle ruote precedentemente sperimentato è stato rimosso dalla suite.
- **Sigarette e sigari:** gestione automatica di oggetti, animazioni e fumo durante le sequenze di fumo supportate, senza menu di attivazione. Animazioni maschili per i protagonisti uomini e gestione distinta per gli NPC.
- **Grafica OGD:** preset ReShade e shader originali per nitidezza, colore e contrasto, accompagnati da interventi su illuminazione diurna e notturna, fari ed effetti ambientali.
- **OGD Motors:** menu dedicato ai veicoli.
- **Guardian:** pannello unico per statistiche, FPS, memoria e stato dei componenti.
- **Integrazione DLSS opzionale:** controller e pannello OGD separati, utilizzabili solo con le dipendenze esterne compatibili.

I menu OGD hanno uno sfondo antracite semitrasparente. Fumo, danni ed effetti ambientali sono automatici.

## Comandi

| Comando | Funzione |
| --- | --- |
| **Shift + F10** | Apri/chiudi Guardian |
| **Shift + F11** | Apri il pannello DLSS, se installato |
| **Shift + F12** | Apri il menu veicoli OGD Motors |
| Frecce / Invio | Naviga e seleziona nel menu veicoli |
| Esc / Backspace | Indietro o chiudi nei menu Guardian e veicoli |
| Invio nel pannello DLSS | Richiedi attivazione/disattivazione |
| Esc nel pannello DLSS | Chiudi il pannello |

Il menu veicoli supporta anche mouse e rotellina. I pannelli OGD si escludono a vicenda. La gestione degli input è stata modificata per impedire che la selezione apra il telefono o che Esc apra contemporaneamente la pausa; queste correzioni richiedono ancora conferma in gioco.

## Compatibilità e installazione

La configurazione di riferimento è **GTA V Legacy per PC, versione 1.0.3889.0**, con Script Hook V compatibile, ScriptHookVDotNet 3.7 e ReShade con supporto agli add-on quando richiesto. La compatibilità con altri aggiornamenti non è garantita. Il pacchetto non è destinato a GTA V Enhanced.

1. Chiudi il gioco ed esegui un backup dei file e dei salvataggi.
2. Installa separatamente le dipendenze necessarie dai siti ufficiali elencati sotto, seguendo le istruzioni dei rispettivi progetti.
3. Estrai lo ZIP e copia le cartelle e i file del pacchetto base nella cartella che contiene `GTA5.exe`, mantenendo la struttura. La cartella `scripts` deve trovarsi direttamente nella cartella del gioco.
4. Se aggiorni una vecchia versione OGD, rimuovi il precedente modulo `CrashWheelDetachment.dll` e la relativa configurazione. Non conservare copie di vecchie DLL nelle sottocartelle di `scripts`.
5. Avvia esclusivamente la modalità Storia.

La cartella `OPZIONALE_DLSS_5` contiene un componente facoltativo e istruzioni dedicate: non è necessario installarlo per utilizzare il pacchetto base. Nello ZIP pubblico l'attivazione automatica del controller DLSS è disabilitata.

**Lo ZIP delle mod contiene componenti OGD e documentazione per gli utenti. Le mod e i runtime di terzi devono essere scaricati separatamente.**

## Grafica e integrazione DLSS: limiti

La grafica punta a una resa più naturale e definita entro le possibilità del gioco e degli strumenti impiegati. Non sostituisce il motore di GTA V con Unreal Engine e non introduce automaticamente Lumen o ray tracing reale.

Il nome della cartella opzionale non significa che OGD distribuisca o abbia creato la tecnologia NVIDIA DLSS. Il controller dipende da componenti esterni, hardware e runtime compatibili. Una richiesta di attivazione nel menu non dimostra che il rendering neurale sia effettivamente in funzione. Non sono garantiti risultati equivalenti ai video dimostrativi online. Il controller rifiuta il runtime neurale se la verifica della firma non riesce.

## Crediti e dipendenze

**Progetto, mod originali, menu, preset, shader e componenti di collegamento OGD: #OGD.**

Un ringraziamento agli autori e ai contributori dei seguenti progetti. Ciascun componente esterno rimane di proprietà dei rispettivi titolari ed è soggetto alla propria licenza.

| Progetto e autore | Utilizzo / collegamento ufficiale |
| --- | --- |
| **Script Hook V e ASI Loader — Alexander Blade** | Accesso alle funzioni del gioco e caricamento dei plugin: [sito ufficiale](https://www.dev-c.com/gtav/scripthookv/) |
| **ScriptHookVDotNet — crosire, kagikn e contributori** | Esecuzione degli script .NET: [progetto](https://github.com/scripthookvdotnet/scripthookvdotnet), [build nightly](https://github.com/scripthookvdotnet/scripthookvdotnet-nightly/releases) |
| **ReShade — crosire e contributori** | Post-processing e supporto agli add-on grafici: [sito ufficiale](https://reshade.me/), [sorgenti](https://github.com/crosire/reshade) |
| **RenoDX — clshortfuse e contributori** | Componente esterno della configurazione grafica opzionale: [progetto e istruzioni](https://github.com/clshortfuse/renodx) |
| **DLSS5-Feeder — jlrouzies-fr e contributori** | Add-on e shader di alimentazione della catena opzionale: [progetto](https://github.com/jlrouzies-fr/DLSS5-Feeder) |
| **VORT — Vortigern e contributori** | Vettori di movimento impiegati dalla configurazione opzionale: [vort_Shaders](https://github.com/vortigern11/vort_Shaders) |
| **NVIDIA** | Tecnologia e runtime DLSS esterni: [pagina ufficiale DLSS](https://developer.nvidia.com/rtx/dlss). Consultare disponibilità e requisiti ufficiali; il collegamento non garantisce la disponibilità di ogni runtime richiesto. |
| **Microsoft** | .NET Framework, runtime Visual C++ e strumenti di compilazione. Seguire i requisiti indicati dalla documentazione di ScriptHookVDotNet e degli altri componenti. |

Riferimenti tecnici: [documentazione delle native CitizenFX](https://docs.fivem.net/natives/) e [dati di riferimento GTA V di DurtyFree e contributori](https://github.com/DurtyFree/gta-v-data-dumps). Sono riferimenti di sviluppo, non mod richieste per l'installazione.

Grand Theft Auto V e i relativi marchi appartengono ai rispettivi titolari, tra cui **Rockstar Games e Take-Two Interactive**. Questo è un progetto amatoriale indipendente, non ufficiale e non affiliato o approvato da Rockstar Games, Take-Two Interactive, NVIDIA o dagli autori delle dipendenze. I ringraziamenti non implicano collaborazione o approvazione.

## Esclusione di responsabilità

Il pacchetto è destinato **esclusivamente alla modalità Storia di GTA V Legacy**. **Non deve essere utilizzato in GTA Online.**

Il software viene fornito **“così com'è”, senza garanzie**. L'installazione e l'utilizzo avvengono sotto la responsabilità dell'utente.

**Nei limiti consentiti dalla legge, l'autore declina ogni responsabilità** per problemi presenti o futuri derivanti dall'installazione, dall'utilizzo o dalla rimozione del pacchetto, inclusi crash, incompatibilità, perdita o corruzione di file e salvataggi, malfunzionamenti del gioco, del sistema operativo o del PC.

Nei medesimi limiti, l'autore non risponde di **ban, sospensioni, limitazioni dell'account o altre sanzioni**, anche qualora l'accesso a GTA Online con le mod installate avvenga accidentalmente. **I controlli integrati non garantiscono protezione dai ban** e non rendono sicuro l'uso online di un'installazione modificata.

Eseguire sempre un backup e utilizzare **un'installazione separata, priva di mod, per GTA Online**.

## Segnalazione dei problemi

Per segnalare un problema su GitHub, indica versione del gioco e del pacchetto, dipendenze installate, altre mod presenti, passaggi per riprodurlo e comportamento osservato. Allega eventuali log pertinenti dopo aver rimosso informazioni personali. Per problemi grafici, indica anche scheda video e configurazione utilizzata.
