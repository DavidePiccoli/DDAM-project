# DDAM-project

link:
https://www.kaggle.com/datasets/patrickhallila1994/nba-data-from-basketball-reference

Alla fine abbiamo preso i dati solo da Boxscore. Salary non è stato utilizzato e games viene usato solo per season start year e gameid


- Prendiamo dati maggiori anno 2000 e minori 2010 causa lockout nel 2011 (quindi il concetto è prende il periodo in cui i punti segnati sono costanti)
- pulire colonna MP in Boxscore
- eliminare notes startET, datetime, isregular, attendance in games.

- Abbiamo visto che tutti i valori nel dataset unito (dopo il join) sono stringhe (tralasciando game_id, Is_starter, seasonstartyear, is_regular). Abbiamo quindi convertito i valori convertibili in int, tranne il tempo in float. Ci siamo resi conto che i minuti < 10 sono preceduti da uno spazio. Si è optato per convertire tutto in secondi. 

ESKETIT

- Data exploration
- Creazione features (specialmente in base al tempo) per giocatore

- Clustering sulle performance e confronto con ruoli e salari (k-means)
- Classificazione in base al ruolo (RF)



- OPTIONAL
- Creare delle profilazioni (in base al cluster) dei giocaTori ed eseguire la classificazione. 
- Capire se un giocatore è IsStarter in base alle statistiche di ogni giocatore (togliendo minuti giocati).
