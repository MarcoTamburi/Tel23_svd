# Tel23_svd
Programmi per lo studio di dati CD a 4 componenti principali.
Il Tel23 si è visto con il primo programma (n_components) avere 4 componenti principali e di conseguenza i fit per la deconvoluzione e ricavo di parametri termodinamici sono stati eseguiti a 4 componenti.
Al fine di runnare i codici su un container di docker è necessario seguire l'ordine logico dei programmi in questione.
1) Crea_matriceT ---> questo programma ti consente di prendere i dati grezzi e trasformarli in dati utili per lavorare nel notebook di jupyter successivo 
2) n_components ---> prende il file .csv creato con il programma precedente e permette all'user di scegliere il numero di componenti (in questo caso il container di docker è stato necessariamente creato per 4 componenti)
3) programma-di-fit4 ---> questo programma, invece, è il core del lavoro in quanto fitta tutte le componenti ed estare i parametri termodinamici (tutto necessario per la ricostruzione)
4) Sperctral_recostruction4 ---> l'ultimo programma da runnare è proprio quello che ci ricostruisce gli spettri con 4 componenti, continene gli errori del modello.
