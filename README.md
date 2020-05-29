Questo repository contiene i grafici delle misure effettuate in locale e su cluster dei tempi di esecuzione di Hadoop MapReduce,
Hive e Spark per i vari punti del primo progetto di Big Data del 2020.
---
Considerazioni aggiuntive sul codice caricato e sul progetto:
- la parte java contiene solo i packages con le classi e il pom; ho utilizzato java 1.8
- per il cluster ho utilizzato la configurazione presentata nelle slide con 3 nodi m5.xlarge
- molti test su cluster li ho dapprima effettuati usando la cli, poi l'interfaccia grafica e il pannello di gestione del cluster.
Nei casi in cui l'output non veniva catturato adeguatamente nei log stdout (hive/spark)
si sono usati come riferimenti i tempi relativi a "elapsed time" per i vari step dall'interfaccia grafica
Avrei voluto introdurre delle ottimizzazioni al codice (come in hive provare ad usare un bucket map side join o il partizionamento
sull'anno, specialmente per la terza query con i soli 3 anni), ma è stato un progetto lungo.
