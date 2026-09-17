\# Domande d'Esame - Parte 3: Machine Learning



\---



\## Domanda 1

Un amico vuol costruire un modello di ML per classificazione disponendo di 1000 dati etichettati. È incerto tra le seguenti opzioni su come dividere i dati per Training (TR), Validation (VL) e Test (TS) ai fini sia della model selection che della model assessment. Scegliete quelle che vanno escluse (perché non corrette) tra le seguenti.



\*\*Opzioni:\*\*

1\. 800 dati TR, 100 VL, 100 TS

2\. 5-fold CV su 600 dati ai fini della model selection, 400 TS

3\. 900 dati TR e VL (sugli stessi 900 dati) e 100 TS

4\. 900 TR, 100 VL, 100 TS riestratto con ricampionamento casuale dai 1000 dopo la model selection

5\. 10-fold CV su 700 dati ai fini della model selection, 300 TS

6\. 10-fold CV ai fini della model assessment con all'interno delle iterazioni 800 dati TR, 100 VL

7\. 900 dati TR, 100 VL e TS (sugli stessi 100 dati)

8\. 10-fold CV ai fini della model assessment con all'interno delle iterazioni 800 dati TR, 200 VL



\---



\## Domanda 2

Immaginiamo di regolare il lambda in ridge regression: cosa vi aspettate (non necessariamente ma con maggiore probabilità in base alla Statistical Learning Theory)?



\*\*Opzioni:\*\*

1\. L'errore in training aumenta al crescere di lambda

2\. L'errore sul validation set aumenta al crescere di lambda a parità di errore di training

3\. L'errore sul validation set non cambia

4\. L'errore sul validation set può aumentare o diminuire

5\. Se l'errore di training aumenta, aumenta anche in validation e test

6\. L'errore sul validation set può aumentare ma non quello in test



\---



\## Domanda 3

Nei DT, dopo lo splitting il DT classifica più casi come positivi.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 4

Un classificatore lineare con LBE può risolvere problemi non linearmente separabili.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 5

Candidate Elimination (CE). Consideriamo una variabile a valori 0 o 1 e H espresso con il linguaggio che abbiamo usato per CE, ossia {<0>, <1>, <∅>, <?>}. È fornito il seguente esempio di training: X1= <0, +>. Si chiede cosa restituirà CE dopo il training su questo esempio (S e G) e cosa si risponderà classificando sull'esempio di test X2=<1> con le ipotesi del Version Space creato.



\*\*Opzioni:\*\*

1\. S={<1>}, G={<?>}, VS risponde +

2\. S={}, VS risponde +

3\. S={<0>}, G={<0>}, VS risponde -

4\. S={<0>}, G={<?>}, VS risponde -

5\. S={<0>}, G={<1>}, VS risponde -

6\. S={<0>}, G={<?>}, VS risponde +

7\. S={<1>}, G={<0>}, VS risponde rejection

8\. S={<0>}, G={<1>}, VS risponde +

9\. S={<∅>}, G={<?>}, VS risponde rejection

10\. S={<0>}, G={<?>}, VS risponde rejection



\---



\## Domanda 6

Il K-nn migliora le prestazioni di accuratezza con più dati nel training set.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 7

Il vantaggio della SVM consiste nell'avere i Kernel che riducono la VC-dimension.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 8

La formulazione duale della SVM permette di non avere una dipendenza della soluzione dalla dimensione del feature space.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 9

Aumentando lambda per un modello di ridge regression quali tra le seguenti quantità aumentano nel VC-bound della SLT?



\*\*Opzioni:\*\*

1\. R\_emp

2\. Il delta δ

3\. La somma dei due termini del bound se era in overfitting

4\. La somma dei due termini del bound se era in underfitting

5\. VC-Confidence

6\. Uno solo dei due termini del bound in base al valore di delta

7\. VC-dim

8\. l (elle)



\---



\## Domanda 10

Se ci sono molti dati potrei avere meno necessità di un lambda alto in ridge regression per controllare il termine VC-confidence del VC-bound della SLT.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 11

Il bias induttivo è più forte per find-S che per CE.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 12

Il bias induttivo è una preferenza del sistema di learning che riguarda i vincoli sul modello oppure il modo di fare ricerca nello spazio delle ipotesi, ma non entrambe.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 13

Model Selection. Si consideri la seguente affermazione: “Valutare la media tra errore di training e di validation permette una selezione più accurata del miglior modello (model selection)”. Scegli tra le seguenti osservazioni relative all'affermazione quelle appropriate.



\*\*Opzioni:\*\*

\- a. È errata, l'errore di validazione non si considera quando si effettua la selezione del modello

\- b. È errata, stimare anche il fitting non è quanto richiesto e opportuno nella fase di model selection

\- c. È errata, serve un test set per fare questa selezione in modo rigoroso

\- d. È corretta, ci permette un buon compromesso tra underfitting e overfitting

\- e. È errata, si rischia di favorire un modello in overfitting

\- f. È errata, si rischia di favorire un modello in underfitting

\- g. È corretta, la scelta di un modello con un basso errore esterno al training combinata con un buon fitting è probabilmente quella vincente



\---



\## Domanda 14

Considerate il modello h(x) = 1 se $2x\_1 + 2x\_2 + 4x\_3 \\geq 0$; 0 (classe negativa) altrimenti. Vanno indicate tutte e sole le affermazioni appropriate.



\*\*Opzioni:\*\*

1\. È un modello per regressione

2\. È un modello a minimo margine

3\. Ha un bias (ossia threshold) nullo

4\. Realizza un AND

5\. Se regolarizzato si avrebbero più bassi i valori 2, 2 e 4 presenti nell'equazione

6\. Se in (1,1,1) il target è 1 il coefficiente di $x\_3$ va abbassato

7\. Il punto (0,-1,-1) verrebbe classificato 0 (o classe negativa)

8\. Tutti i punti sono classificati come negativi

9\. È un modello polinomiale

10\. Se in (1,1,1) il target è 0 il coefficiente di $x\_3$ va abbassato



\---



\## Domanda 15

Quali di queste quantità (iperparametri/parametri) aumentando di valore fanno potenzialmente alzare il VC-confidence term (e abbassare Remp) nel bound della SLT?



\*\*Opzioni:\*\*

1\. Il numero dei nodi di un DT

2\. Il numero di dati l (elle)

3\. I valori di input x nei modelli lineari

4\. La dimensione di input in un linear model

5\. Il grado del kernel polinomiale

6\. Il lambda in ridge regression

7\. Il sigma di SVM con RBF kernel

8\. Il grado M in una LBE polinomiale

9\. Il numero di parametri liberi in un modello lineare perché fa crescere il lambda di Tikhonov

10\. Il C di SVM



\---



\## Domanda 16

Per tutti i modelli supervised (visti nel corso) si può avere in principio underfitting o overfitting.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 17

Dato il modello h giudicate quali tra le seguenti affermazioni sono vere:

$h(x) = x\_1w\_1 + x\_2w\_2 + \\log(x\_1)w\_3 + w\_0$



\*\*Opzioni:\*\*

1\. Permette un'approssimazione di (alcuni tipi di) funzioni non lineari

2\. Può andare in overfitting

3\. Le x sono i parametri liberi del modello

4\. È un modello lineare nei parametri liberi

5\. È un modello polinomiale

6\. Non si può sottoporre a training con l'algoritmo a discesa di gradiente

7\. È una linear basis expansion

8\. È un modello lineare nelle variabili di ingresso



\---



\## Domanda 18

Un passo di Candidate Elimination: Indicare il risultante VS dopo aver visto l'esempio indicato in forma x, c(x), con valori binari per x e c(x) e H={x, not(x), 0, 1} (dove in CE <0> è per not(x), <1> è per x, <?> è per l'1; 0 restituisce sempre 0, 1 sempre 1). Esempio: 1, 1.



\*\*Opzioni:\*\*

1\. VS={x, 1}

2\. VS={not(x), 1}

3\. VS={x}

4\. VS={1}



\---



\## Domanda 19

Un passo di Candidate Elimination: Indicare il risultante VS dopo aver visto l'esempio indicato in forma x, c(x), con valori binari per x e c(x) e H={x, not(x), 0, 1} (dove in CE <0> è per not(x), <1> è per x, <?> è per l'1; 0 restituisce sempre 0, 1 sempre 1). Esempio: 0, 1.



\*\*Opzioni:\*\*

1\. VS={not(x)}

2\. VS={x, 1}

3\. VS={1}

4\. VS={not(x), 1}



\---



\## Domanda 20

Trovare tra i seguenti modelli lineari (specificati con i valori di $w\_1$ per $x\_1$, $w\_2$ per $x\_2$ e $w\_0$) quelli che classificano correttamente i punti del piano (-1,-1), (0,0), (1,1) come positivi e (0,-2), (1,-1) come negativi, specificando le opzioni corrette anche in base al possedere (o meno) per il modello la proprietà di separazione a massimo margine.



\*\*Opzioni:\*\*

1\. w1=-1, w2=1, w0=-1 (no max. margine)

2\. w1=-1, w2=1, w0=1 (no max. margine)

3\. w1=-1, w2=1, w0=0.5 (max. margine)

4\. Nessuno di questi (non sono due insiemi di punti linearmente separabili)

5\. w1=-1, w2=1, w0=1 (max. margine)

6\. w1=-1, w2=1, w0=0.5 (no max. margine)

7\. w1=-1, w2=1, w0=-1 (max. margine)



\---



\## Domanda 21

Trovare tra i seguenti modelli lineari (specificati con i valori di $w\_1$ per $x\_1$, $w\_2$ per $x\_2$ e $w\_0$) quelli che classificano correttamente i punti del piano (1,3), (-1,1) come positivi e (-1,-1), (1,1), (1,-1) come negativi, specificando le opzioni corrette anche in base al possedere (o meno) per il modello la proprietà di separazione a massimo margine.



\*\*Opzioni:\*\*

1\. w1=-1, w2=1, w0=-0.5 (max. margine)

2\. w1=-1, w2=1, w0=-0.5 (no max. margine)

3\. w1=-1, w2=1, w0=-1 (no max. margine)

4\. w1=-1, w2=1, w0=-1 (max. margine)

5\. w1=-1, w2=1, w0=+0.5 (max. margine)

6\. w1=-1, w2=1, w0=+0.5 (no max. margine)

7\. Nessuno di questi (non sono due insiemi di punti linearmente separabili)



\---



\## Domanda 22

Costruire un classificatore (+1/-1) da features a valori reali x ottenuto elaborando un segnale di Elettrocardiogramma. Scegliere tra i seguenti modelli quelli che potrebbero essere adeguati/corretti (indipendentemente dal valutare le loro capacità sul problema).



\*\*Opzioni:\*\*

1\. $h(x) = \\text{sign}(w^T \\log(x))$

2\. $h(x) = w^T x$

3\. $h(x) = w^T x + \\lambda ||w||^2$

4\. $h\_k(x) = \\frac{1}{k} \\sum\_{x\_i \\in N\_k(x)} y\_i$

5\. $h(x) = w^T \\log(x)$

6\. $h(x) = \\arg\\min\_i ||x - c\_i||^2$ con i $c\_i$ trovati con K-means

7\. $h(x)$ da DT

8\. $h(x) = \\text{sign}(w^T x)$



\---



\## Domanda 23

In un problema di regressione (con le usuali notazioni adottate nel corso) viene proposta la seguente ipotesi: $h\_w(x) = w\_1x\_1 + w\_2x\_2 + w\_3\\cos(x\_2) + w\_4(x\_2)^4 + w\_0$. Si vuol calcolare la regola di apprendimento di tipo "discesa di gradiente" per il parametro $w\_4$. Indicare tra le seguenti la o le formulazione/i corretta/e:



\*\*Opzioni:\*\*

1\. $w\_4^{(new)} = w\_4 + \\eta 2 \\sum\_{p=1}^l (y\_p - h\_w(x\_p)) \\cdot x\_{p,4}$

2\. $w\_4^{(new)} = w\_4 + \\eta 2 \\sum\_{p=1}^l (y\_p - h\_w(x\_p)) \\cdot (x\_{p,2})^4$

3\. $w\_4^{(new)} = w\_4 + \\eta 2 \\sum\_{p=1}^l (y\_p - h\_w(x\_p)) \\cdot 4(x\_{p,2})^3$

4\. $w\_4^{(new)} = w\_4 + \\eta 2 \\sum\_{p=1}^l (y\_p - h\_w(x\_p)) \\cdot x\_{p,2}$



\---



\## Domanda 24

Il bias induttivo è preferibile averlo in termini di restrizioni sul modello.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 25

Il bias induttivo nei modelli più flessibili si focalizza sulla strategia di ricerca nello spazio delle ipotesi.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 26

Il bias induttivo per il Find-S riguarda solo le assunzioni sul modello.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 27

L'algoritmo di apprendimento per il Decision Tree ha un bias di ricerca.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 28

Dati degli scatoloni contenenti M periferiche di computer etichettate con 0 (tastiera) od 1 (ogni altro oggetto), si vuol creare un classificatore che discrimina tra gli scatoloni senza tastiere (attribuiti alla classe negativa o zero) e gli scatoloni con almeno una tastiera (attribuiti alla classe positiva o 1). Quali tra i seguenti modelli possono risolvere il task perfettamente?



\*\*Opzioni:\*\*

1\. SVM ma solo se con Kernel RBF

2\. K-NN per opportuno valore di K

3\. Decision Tree

4\. SVM con kernel polinomiali

5\. SVM ma solo se in versione soft margin

6\. Find-S

7\. Linear model

8\. Linear model ma solo con LBE che estende la dimensione dell'input originale

9\. Candidate Elimination



\---



\## Domanda 29

Il bias induttivo è presente in un sistema di SVM.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 30

Il bias induttivo è necessario per avere un sistema capace di generalizzare.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 31

Ci sono modelli più flessibili ma proni all'overfitting.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 32

Solo i modelli lineari hanno una flessibilità limitata che permette di evitare l'overfitting.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 33

Dati dei pacchetti di figurine, contenenti L figurine etichettate con 0 (se rosse) od 1 (ogni altro colore), si vuol creare un classificatore che discrimina tra i pacchetti senza figurine rosse (attribuiti alla classe negativa o zero) e i pacchetti con almeno una figurina rossa (attribuiti alla classe positiva o 1). Quali tra i seguenti modelli possono risolvere il task perfettamente?



\*\*Opzioni:\*\*

1\. Candidate Elimination

2\. Decision Tree ma solo con pruning

3\. SVM ma solo se con Kernel RBF

4\. Linear model

5\. K-NN per opportuno valore di K

6\. Find-S

7\. SVM con kernel polinomiali

8\. Linear model ma solo con LBE che riduce la dimensione dell'input originale

9\. SVM hard margin



\---



\## Domanda 34

Per una hard margin SVM, si selezionino tutte le affermazioni appropriate in merito ai vettori di supporto:



\*\*Opzioni:\*\*

1\. I vettori di supporto sono i punti con classificazione incerta del modello

2\. Sono i punti più vicini al piano separatore

3\. I vettori di supporto sono i punti ove $w^T x > 1$

4\. Sono i punti più vicini al margine

5\. I vettori di supporto sono dati del training set

6\. I vettori di supporto stanno dentro il margine

7\. I vettori di supporto sono i punti ove $w^T x = 1$

8\. Sono i punti $x\_p$ tali che $|w^T x\_p + b| = 1$

9\. Sono i punti $x\_p$ tali che $|w^T x\_p + b| > 1$

10\. Sono i vettori $x\_p$ per cui $\\alpha\_p < 0$



\---



\## Domanda 35

Nella costruzione di un Decision Tree con un insieme di dati Z, quali di queste formulazioni permetterebbero di scegliere il miglior attributo A in accordo al massimo information gain?



\*\*Opzioni:\*\*

1\. $\\text{Gain}(Z, A) = \\text{Entropy}(Z) + \\sum\_{p \\in \\text{Values}(A)} \\frac{|Z\_p|}{|Z|} \\text{Entropy}(Z\_p)$

2\. $\\text{Gain}(Z, A) = - \\sum\_{p \\in \\text{Values}(A)} \\text{Entropy}(Z\_p) \\frac{|Z|}{|Z\_p|} + \\text{Entropy}(Z)$

3\. $\\text{Gain}(Z, A) = - \\sum\_{i=1}^c \\frac{|Z\_i|}{|Z|} \\log\_2 \\frac{|Z\_i|}{|Z|}$

4\. $\\text{Gain}(Z, A) = \\text{Entropy}(Z) + \\sum\_{p \\in \\text{Values}(A)} \\frac{|Z\_p|}{|Z|} \\text{Entropy}(Z)$

5\. $\\text{Gain}(Z, A) = \\text{Entropy}(Z) - \\sum\_{p \\in \\text{Values}(A)} \\frac{|Z\_p|}{|Z|} \\text{Entropy}(Z\_p)$

6\. $\\text{Gain}(Z, A) = - \\sum\_{p \\in \\text{Values}(A)} \\text{Entropy}(Z\_p) \\frac{|Z\_p|}{|Z|} + \\text{Entropy}(Z)$

7\. $\\text{Gain}(Z, A) = \\text{Entropy}(Z) - \\sum\_{p \\in \\text{Values}(A)} \\frac{|Z\_p|}{|Z|} \\text{Entropy}(Z)$

8\. $\\text{Gain}(Z, A) = - \\sum\_{p \\in \\text{Values}(A)} \\text{Entropy}(Z\_p)$

9\. $\\text{Gain}(Z, A) = \\text{Entropy}(Z) - \\sum\_{p \\in \\text{Values}(A)} \\frac{|Z|}{|Z\_p|} \\text{Entropy}(Z\_p)$



\---



\## Domanda 36

Il bias induttivo è una preferenza del sistema di learning che riguarda i vincoli sul modello ma non la strategia di ricerca nello spazio delle ipotesi.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 37

Il bias induttivo è di due tipi: uno chiamato language bias ed uno chiamato search bias.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 38

Terminare in anticipo la crescita di un DT permette un controllo dell'overfitting.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 39

I modelli lineari permettono di avere già un sistema che evita l'overfitting.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 40

Il training di un classificatore si può attuare con una tecnica di discesa di gradiente.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 41

Il general boundary, G, di un version space è l'insieme dei membri minimamente generali di H consistenti con l'insieme dei dati D.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 42

In H discreti per Concept Learning, la relazione di "more general than" permette un ordinamento assoluto tra le ipotesi.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 43

Relativamente al bound SLT quali delle seguenti affermazioni sono vere/corrette?



\*\*Opzioni:\*\*

1\. Non sempre l'aumento della VC-dim porta ad aumentare il VC-bound

2\. Un decrescente valore di lambda nella ridge regression tende ad aumentare il Remp

3\. Un decrescente valore di lambda nella ridge regression può aumentare il termine di VC-confidence

4\. Aumentare la VC-dim porta ad aumentare il Remp



\---



\## Domanda 44

Scegli tra le seguenti una o più formulazioni alternative di Loss che siano valide (utilizzabili) per il training (con discesa di gradiente) di un classificatore lineare, con l pattern input di dimensione n.



\*\*Opzioni:\*\*

1\. $\\text{Loss}(w) = 0.6 \\sum\_{j=1}^l (w^T x\_j - y\_j)^2$

2\. $\\text{Loss}(w) = \\sum\_{p=1}^l (y\_p - h\_w(x\_p))^2$

3\. $\\text{Loss}(w) = 1 + \\sum\_{p=1}^l (y\_p - x\_p^T w)^2$

4\. $\\text{Loss}(w) = \\sum\_{j=1}^l (-w^T x\_j + y\_j)^2$

5\. $\\text{Loss}(w) = \\sum\_{p=1}^n (y\_p - h\_w(x\_p))^2$

6\. $\\text{Loss}(w) = \\sum\_{j=1}^n (w\_j^T x\_j - y\_j)^2$

7\. $\\text{Loss}(w) = \\sum\_{p=1}^l (y\_p + x\_p^T w)^2$



\---



\## Domanda 45

Quali tra queste affermazioni sulla SVM hard-margin sono vere?



\*\*Opzioni:\*\*

1\. I vettori di supporto sono i punti ove $w^T x = 0$

2\. I vettori di supporto determinano il margine

3\. Il numero di vettori di supporto è una frazione del numero di dati di training

4\. I vettori di supporto sono i dati errati del training set

5\. I vettori di supporto determinano da soli l'iperpiano separatore

6\. Il numero di vettori di supporto è una frazione del numero di dati di test

7\. I vettori di supporto sono i punti con classificazione errata di un modello lineare

8\. I vettori di supporto sono sia tra i dati nella classe positiva che negativa



\---



\## Domanda 46

Le slack variable (ossia i loro valori) nella SVM soft margin sono indicate dall'utente.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 47

Il problema primale della SVM ha una funzione obiettivo per cercare il piano a minimo errore di classificazione in training.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 48

Una procedura per costruire un modello di ML. Per costruire un classificatore si hanno training, validation e test set (hold out). Si ottimizza l'accuracy in training, si valuta il miglior modello sul validation set e poi si controlla il risultato sul test set; se quest'ultimo non è soddisfacente si attua un nuovo e diverso ciclo di selezione di varianti del modello scegliendo il migliore sul validation set (rieseguendo ogni volta un training sul training set), alla fine si valuta sul test set. Scegli tra le seguenti osservazioni una o più alternative che sono corrette.



\*\*Opzioni:\*\*

1\. È una procedura corretta

2\. Va evitato il secondo ciclo se avevo già correttamente ottimizzato su training e validation set al primo ciclo

3\. È una procedura non ottimizzata, potrei direttamente fornire il risultato di model assessment con quanto ottenuto sul validation set del secondo ciclo senza riverificare sul test set

4\. È una procedura corretta solo se i 3 insiemi hanno intersezione nulla (nessun dato in comune)

5\. È una procedura parzialmente corretta, basterebbe non rieseguire ogni volta il training

6\. È una procedura errata, perché così facendo il risultato del test set non sarà una stima rigorosa della capacità di generalizzazione su dati nuovi

7\. È una procedura errata, perché così facendo il test set è utilizzato per fare scelte sul modello

8\. È bene aver fatto il secondo ciclo, ho raffinato il modello e potenzialmente incrementato i risultati complessivi

9\. È una procedura errata, perché così facendo si rischia l'overfitting giacché si prova più volte a ridurre l'errore di training senza tener conto della generalizzazione

10\. È una procedura errata, perché così facendo si rischia l'underfitting giacché si è data troppa rilevanza ai risultati di validation e test rispetto a quelli di training

11\. È una procedura parzialmente corretta, basterebbe scambiare il validation set con il test set alla seconda iterazione



\---



\## Domanda 49

Si vuol costruire un Decision Tree con l'algoritmo ID3 e l'uso di Gain(S,A) che realizzi la funzione booleana NOR per le variabili booleane x e y. Si indichino tra le seguenti le affermazioni corrette.



\*\*Opzioni:\*\*

1\. Il calcolo iniziale (per la radice) di Gain(S, x) = E(S) - 2/3

2\. Il calcolo iniziale (per la radice) di Gain(S, x) = E(S) - 1/4

3\. Si sceglie prima (alla radice) y per il gain più alto

4\. Si può scegliere indifferentemente prima x o y

5\. La soluzione è l'albero not(x) or not(y)

6\. La soluzione è l'albero not(x) and not(y)

7\. Si sceglie prima (alla radice) x per il gain più basso

8\. Il calcolo iniziale (per la radice) di Gain(S, x) = E(S) - 1/3

9\. Il calcolo iniziale (per la radice) di Gain(S, x) = E(S) - 1/2



\---



\## Domanda 50

Un cliente si rivolge a 5 aziende di IA (A1, A2, ..., A5) per creare modelli di ML fornendo dati di training, ma tenendo un blind set (non reso noto alle 5 aziende fornitrici). Avuti i 5 modelli (M1, M2, ..., M5, rispettivamente da A1, ..., A5) il cliente calcola l'errore sul blind set (E1, E2, ... E5, rispettivamente da M1, ..., M5) e sceglie il modello M2 che fornisce il miglior risultato (errore minimo). Scegliere tra le seguenti affermazioni quelle che sono possibili validi commenti alla procedura (più opzioni possono essere commenti validi).



\*\*Opzioni:\*\*

1\. Non è detto il miglior modello per scopi predittivi sia M2 poiché non conosciamo il tempo di training dei modelli

2\. Può scegliere M2 e quell'errore (E2) sarà la stima dell'errore del modello nel suo uso successivo

3\. Doveva farsi dare da A2 l'errore di training e verificare se fosse uguale ad E2 e solo in quel caso pagare A2

4\. Doveva farsi dare dalle aziende più informazioni, in particolare che errore di predizione stimavano ed usare quello per decidere l'azienda migliore da pagare

5\. Prima di scegliere in modo autonomo, poteva farsi dare da A2 più informazioni, in particolare che stima avevano di test e le modalità usate per ottenere la stima

6\. Doveva farsi dare dalle aziende più informazioni, in particolare che errore di training avevano e scegliere in base a quello il miglior modello e poi usare E2 come errore di test

7\. E2 è stato usato per model selection

8\. Doveva farsi dare dalle aziende più informazioni, in particolare che errore di training avevano e scegliere in base a quello il miglior modello

9\. Può scegliere M2 ma E2 non è una buona stima delle prestazioni di accuratezza nel suo uso successivo



\---



\## Domanda 51

In una LBE polinomiale di grado “g”, cosa vi aspettate con maggiore probabilità in base alla disequazione della Statistical Learning Theory?



\*\*Opzioni:\*\*

1\. La somma dei due termini Remp e VC-confidence diminuisce sempre con l'aumentare di g

2\. Si può generalizzare bene quando il valore di g permette un bilanciamento tra Remp e VC-confidence

3\. Aumentare g tende a ridurre il Remp

4\. L'aumento di g tende a ridurre la VC-dim

5\. La diminuzione di g fa diminuire il valore di δ (delta)

6\. La diminuzione di g tende a far diminuire la VC-confidence (a pari valore degli altri termini e valori presenti)



\---



\## Domanda 52

Dopo che è stata calcolata la soluzione (valori alfa) di una SVM soft-margin, viene aggiunto un punto nel training set. Valutare le seguenti affermazioni sulle possibili modifiche alle nuove soluzioni.



\*\*Opzioni:\*\*

1\. Se il punto sta dalla parte giusta dell'iperpiano separatore precedente e oltre il margine la soluzione non cambia

2\. Se il punto entra nell'area del margine precedente, la slack variable associata potrà assumere un valore non nullo per mantenere un margine più ampio

3\. Se il punto sta dalla parte giusta dell'iperpiano separatore precedente e oltre il margine la soluzione cambia dovendo scegliere nuovi vettori di supporto e un nuovo iperpiano separatore

4\. Se il punto sta dalla parte errata dell'iperpiano separatore precedente, nella zona dei pattern di classe opposta, non necessariamente si fallisce a trovare una soluzione

5\. Se il punto entra nell'area del margine precedente, la slack variable associata potrà assumere un valore non nullo per mantenere un margine meno ampio

6\. Se il task diventa non linearmente separabile (esempio un punto negativo tra i positivi), la SVM fallisce a trovare una soluzione che soddisfi i vincoli



\---



\## Domanda 53

Far crescere i nodi in un DT corrisponde ad avere Remp alto e VC-confidence basso.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 54

Nessun modello generalizza meglio di un unbiased learner.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 55

Un unbiased learner generalizza in modo migliore di un learner con bias induttivo di linguaggio.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 56

Un modello lineare con w tutti nulli è un modello look-up table.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 57

Per un modello lineare si può trovare un compromesso tra underfitting e overfitting regolando il valore dei w.



\*\*Opzioni:\*\*

\- Vero

\- Falso



\---



\## Domanda 58

Prese delle immagini con pixel 0 (spento)/1 (acceso), si vuol creare un classificatore che discrimina tra quelle nere (attribuite alla classe negativa o zero) e quelle con almeno un pixel acceso (attribuite alla classe positiva o 1). Quali tra i seguenti modelli possono risolvere il task perfettamente?



\*\*Opzioni:\*\*

1\. Candidate Elimination

2\. SVM ma solo se in versione soft margin

3\. SVM con kernel polinomiali

4\. Decision Tree

5\. Find-S

6\. Linear model ma solo con LBE che estende la dimensione dell'input originale

7\. K-NN per opportuno valore di K

8\. Linear model

9\. SVM ma solo se con Kernel RBF



\---



\## Domanda 59

Quali tra le seguenti affermazioni sulla regressione con LBE polinomiale sono corrette? Selezionare tutte e sole le opzioni corrette. Opzioni errate comportano un punteggio negativo.



\*\*Opzioni:\*\*

\- a. Un polinomio di grado più alto non garantisce migliore generalizzazione, perché può aumentare il rischio di overfitting.

\- b. Il test set può essere riutilizzato per model selection e poi per ottenere una stima finale non distorta dell'errore.

\- c. Il grado $M$ non è un iperparametro, perché non influenza il modello appreso.

\- d. La regressione polinomiale può essere ottenuta costruendo una rappresentazione espansa degli input.



\---



\## Domanda 60

Scegliere tutte le affermazioni corrette riguardo agli alberi di decisione e all'algoritmo ID3. Opzioni errate comportano un punteggio negativo.



\*\*Opzioni:\*\*

\- a. La scelta greedy di ID3 valuta gli split nel nodo corrente senza valutare l'effetto globale sull'intero albero finale.

\- b. Quando il sottoinsieme di esempi associato a un ramo è vuoto, ID3 assegna a quel ramo una foglia con la classe più frequente negli esempi del nodo padre.

\- c. Sebbene un attributo abbia information gain nullo nel nodo corrente, può esistere un albero che usa quell'attributo in nodi discendenti migliorando la classificazione degli esempi.

\- d. Un attributo con molti valori tende a essere penalizzato dall'information gain perché produce molti sottoinsiemi piccoli.

\- e. In un nodo con esempi di classi diverse, ID3 può comunque creare una foglia se non restano attributi disponibili.

\- f. L'information gain è indipendente dalla distribuzione delle classi nei sottoinsiemi generati dallo split.

\- g. Se uno split riduce l'entropia media pesata dei figli rispetto al nodo padre, allora ciascun figlio ha necessariamente entropia minore del nodo padre.

