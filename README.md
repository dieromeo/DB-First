# Tabella database auto usate

Modellizzazione di una tabella per la memorizzazione di vari dati di un concessionario, rigurdanti auto usate.

Sono stati scelti i seguenti campi obbligatori:
- Marchio dell'auto e modello, in quanto elementi base e indispensabili.
- Colore dell'auto, facente parte delle informazioni di base
- Prezzo, in quanto indspensabile per la vendita
- Anno di immatricolazione
- Chilometraggio

### Considerazioni

Per la cilindrata e i cavalli sono stati usati smallint in quanto entrambi i valori potrebbero essere superiori a 255.

Per il prezzo è stato considerato l'uso di un decimal, fino a 6 cifre intere e 2 decimali.

Il valore incidentato sarà rappresentato da true o false, impostato di base come false.

Nel caso in cui non venga specificato il numero di proprietari di default sarà almeno 1

Per la targa, essendo alfanumerica, si è usato un tinyint a 7 cifre, in quanto le macchine dovranno essere ritargate europee.

Inoltre il numero di porte è stato impostato di default a 3, così come il cambio a manuale