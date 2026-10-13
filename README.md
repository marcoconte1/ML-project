# ML-project
L’identificazione accurata della dinamica dei manipolatori industriali ad alto carico e fondamentale per lo sviluppo di schemi di controllo avanzati e per il monitoraggio 
dello stato della macchina. Tuttavia, la modellazione fisica classica
si scontra spesso con non linearita strutturali complesse e diffi- cilmente parametrizzabili, quali attriti dissipativi e giochi meccanici (backlash). Questo lavoro presenta un’analisi comparativa
basata interamente sui dati (black-box) per l’identificazione della
dinamica di un robot industriale KUKA KR300, confrontando
tre diverse architetture neurali: un modello autoregressivo con
ingressi esogeni (NNARX), una rete neurale ricorrente standard
(RNN) e una rete a cancelli Gated Recurrent Unit (GRU). Le
prestazioni sono studiate sia nel task di dinamica diretta (τ → q),
valutato nella severa modalita di simulazione libera ( ` free-run),
sia nel task di dinamica inversa (q → τ ). I risultati sperimentali
evidenziano che, mentre la RNN classica fallisce a causa del
fenomeno del vanishing gradient, l’architettura GRU e il modello
NNARX superano nettamente la baseline lineare. In particolare,
la GRU incrementa l’accuratezza nel task diretto portando il
coefficiente R2
oltre il 50%, mentre nel task inverso entrambi
i modelli superano l’83% di R2. L’introduzione di tecniche
come lo Scheduled Sampling nell’architettura NNARX dimostra
inoltre un’elevata robustezza all’accumulo ricorsivo dell’errore,
delineando soluzioni promettenti per il disaccoppiamento computazionale dei giunti nei futuri sistemi di controllo robotico.
