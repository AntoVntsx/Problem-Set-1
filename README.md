# Problem-Set-1
Corso algoritmi e Strutture Dati, 2 anno informatica, Tor Vergata
# Problema delle sequenze di parentesi bilanciate

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
