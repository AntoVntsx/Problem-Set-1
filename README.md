# Problem-Set-1
Corso algoritmi e Strutture Dati, 2 anno informatica, Tor Vergata
# Problema parentesi k-bilanciate

Si consideri una sequenza di parentesi aperte e chiuse. La sequenza è detta **bilanciata** se ogni parentesi aperta ha una corrispondente parentesi chiusa e le coppie di parentesi sono correttamente annidate. Esempi di sequenze di parentesi bilanciate sono:

- `(()(()()))`
- `(()(()()))`

mentre esempi di sequenze **non bilanciate** sono:

- `)(`
- `()())`

Ora, una sequenza è detta **k-bilanciata** se, aggiungendo **k** parentesi aperte all’inizio della sequenza e **k** parentesi chiuse alla fine della sequenza, si ottiene una sequenza bilanciata. Alcuni esempi:

- La sequenza `)(` è **1-bilanciata**, poiché la sequenza `()()` è bilanciata.
- La sequenza `()())((` è **2-bilanciata** ma non **1-bilanciata**.
- La sequenza `()())` non è **k-bilanciata** per nessun **k ≥ 0**.

## Algoritmo richiesto

Progettare un algoritmo che, data una sequenza lunga **n** di parentesi aperte e chiuse, calcola il minimo valore di **k** per cui la sequenza è **k-bilanciata**, o restituisce `+∞` se non è possibile mai bilanciarla. L’algoritmo deve avere complessità temporale **O(n)** e usare **memoria ausiliaria costante**.

## Argomentazione sulla correttezza

L'algoritmo deve essere progettato in modo che possa determinare il minimo valore di **k** in tempo lineare, utilizzando una sola passata sulla sequenza. La correttezza dell'algoritmo può essere argomentata attraverso l'analisi della gestione delle parentesi aperte e chiuse, monitorando costantemente l'equilibrio della sequenza durante il processo.

# Problema Il posto fisso

Ti hanno recentemente assunto come unico impiegato al piccolo ufficio postale del tuo quartiere. Il lavoro non ti piace e lo fai controvoglia. Però, come dice tua madre, è un posto fisso e il posto fisso è perfetto per te che, come sottolinea sempre lei, sei una persona pigra.

Ogni giorno devi servire un certo numero di clienti, diciamo **n**. Visto che l'ufficio è piccolo e tu sei l'unico impiegato, i clienti devono prenotarsi con una apposita app. Così tu sai quando verranno. Il cliente i-esimo arriva a tempo **tᵢ**.

Questo non vuol dire che un cliente venga servito subito. Infatti, se il cliente arriva e trova lo sportello occupato da altri clienti, si mette in coda e aspetta il suo turno.

Le pratiche sono sempre le stesse e sono tutte uguali. Se lavorassi alla massima velocità, ogni pratica richiederebbe **∆** minuti. Ma tu, come sai perché tua madre non perde occasione per ricordartelo, sei pigro e vuoi lavorare il più lentamente possibile. Diciamo che puoi scegliere un regime giornaliero di velocità, ovvero puoi scegliere un valore intero **∆′ ≥ ∆** che rappresenta il numero di minuti che impiegherai per evadere ogni singola pratica della giornata.

Ovviamente, essendo pigro, vuoi massimizzare **∆′**. Il tuo unico vincolo è non essere licenziato. Tua madre ne soffrirebbe troppo. Per questo devi assicurarti di evadere tutte le pratiche entro il tempo **M** di chiusura.

## Algoritmo richiesto

Progettate un algoritmo che calcola il massimo valore **∆′** ammissibile in tempo **O(nM)**. Si discuta la correttezza e la complessità dell'algoritmo.

## Argomentazione sulla correttezza

L'algoritmo deve essere progettato in modo che possa determinare il massimo valore di **∆′** in tempo lineare, monitorando l'ordine di arrivo dei clienti e calcolando la quantità di tempo che ciascun cliente deve attendere prima di essere servito, senza superare il tempo di chiusura **M**.
