# ComfyUI StabilityAI Suite

Questo fork della repository ufficiale di StabilityAI contiene una serie di migliorie e implementazioni.

## Image Core + Style Preset

Nella versione ufficiale non è presente l'opzione per impostare uno dei __stili__ disponibili. In questo fork il nodo è stato aggiornato: contiene un nuovo switch vero/falso per attivare gli stili, e il relativo selettore.

![Image Core + Style Preset](/images/image_core_style.png)

## Creative Upscale Recover File

Il nodo per l'uspcale creativo esegue due passaggi: la generazione e il recupero dell'immagine generata. Se malauguratamente il PC ha un blocco o manca improvvismente la connessione internet, la seconda fase non può completarsi e rischiate di perdere l'immagine generata e i crediti utilizzati. Per fortuna le immagini vengono archiviate per 24 ore da StabilityAI.

Grazie a una modifica del codice generale, gli __id univoci__ vengono salvati automaticamente all'interno del file __log.txt__. Questo file viene automaticamente creato e salvato nella stessa cartella del custom node. Segui ora questo passaggi:

- Apri il file e copia l'id desiderato.
- Incolla l'id nel nodo __Creative Upscale Recover File__ per recuperare l'immagine persa.

![Creative Upscale Recover File](/images/creative_upscale_recover_file.png)