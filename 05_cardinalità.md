# Cardinalità
- [Cardinalità](#cardinalità)
  - [Numeri transfiniti](#numeri-transfiniti)
    - [Esempio: Gli alberghi transfiniti](#esempio-gli-alberghi-transfiniti)
  - [Cardinalità](#cardinalità-1)
    - [Cantor-Schröder-Bernstein](#cantor-schröder-bernstein)
    - [Definizione infinito (Dodekin, 1888)](#definizione-infinito-dodekin-1888)
    - [Esempio: Polvere di Cantor](#esempio-polvere-di-cantor)
  - [Diagonale di Cantor](#diagonale-di-cantor)
    - [Teorema di Cantor](#teorema-di-cantor)
  - [Ipotesi del continuo](#ipotesi-del-continuo)
  - [Funzioni non calcolabili](#funzioni-non-calcolabili)

## Numeri transfiniti
I numeri transfiniti sono numeri "infiniti", nel senso che sono più grandi di qualsiasi numero finito, ma non necessariamente infiniti in manier assoluta.

Nei numeri transfiniti il concetto di numeri ordinali (uno, due, tre...) e cardinali (primo, secondo, terzo...) sono distinti e i numeri cardinali diventano strumento per descrivere la grandezza di un insieme infinitamente largo.

Il più piccolo numero ordinale transfinito è $\omega$, un insieme contenente tutti i numeri. Dato $\omega$ construiamo un nuovo insieme $\omega + 1$, che contiene, come $\omega$, più uno, dimostrando quindi che i numeri transfiniti sono, beh, infiniti. Con lo stesso principio possiamo continuare e avere $\omega + \omega, \omega + \omega + \omega, \dots$.

Il più piccolo numero cardinale transfinito è $\aleph_{0}$, che corrisponde alla potenza del numerabile (cardinalità di $\N$ o $\mathbb{Q}$). Il numero successivo è $2^{\aleph_{0}} = \aleph_{1}$, corrispondente alla potenza del continuo (cardinalità di $\R$ e $\wp(N)$).

### Esempio: Gli alberghi transfiniti
Esperimento mentale introdotto da David Hilbert in una lezione del 1924 e volto a dimostrare le proprietà controintuitive degli insiemi infiniti.

*Vedi video*: [The Infinite Hotel Parodox](https://www.youtube.com/watch?v=Uj3_KqkI9Zo)

## Cardinalità
Il discorso sulla cardinalità nasce dall'esigenza di dimostrare la grandezza dei numeri transfiniti.

> **DEFINIZIONE**
> La cardinalità di un insieme $A$, indicata come $|A|$, è la classe di equipotenza di $A$. 

1. L'equipotenza è una relazione di equivalenza (riflessiva, simmetrica, transitiva). 
2. Due insiemi si dicono equipotenti se esiste una funzione biiettiva $f: A \to B$ (quindi una **corrispondenza biunivoca**)


### Cantor-Schröder-Bernstein
Nella teoria degli insiemi, se $f: A \to B$  è iniettiva, allora $f: B \to A$ anche è iniettiva, allora $A \to B$ è biiettiva.

Ne consegue che:
1. se $|A| \leq |B|$ se e solo se esiste una funzione iniettiva $f: A \to B$
2. $|A| \leq |B|$ e $|B| \leq |A|$, allora $|A| = |B|$ : **se c'è una corrispondeza biunivoca tra le cardinalità di due insieme, essi sono equipotenti**.

Per questo principio si può dedurre anche che possiamo anche ricavare che $\omega$ è equipotente a $\omega + 1$

### Definizione infinito (Dodekin, 1888)
Un insieme si dice **infinto** se è equipotente ad una sua parte propria; in caso opposto si dice infinito.

### Esempio: Polvere di Cantor
L'insieme di Cantor è uno specifico sottoinsieme dei numeri reali nell'intervallo $[0, 1]$. Questo insieme è famoso per avere proprietà che sembrano quasi contradditorie o paradossali. 

> L'insieme di Cantor è un insieme continuo di dimensione zero. 
> Non ha cardinalità numerabile, poiché è equipotente a $\R$.

*La polvere di Cantor è una versione multidimensionale dell'insieme di Cantor, ottenuta costituendo il prodotto cartesiano dell'insieme di Cantor con se stesso*.

**Polvere di Cantor** 

L'insieme di Cantor è definibile in modo ricorsivo, partendo dall'intervallo $[0 , 1]$ ($C_{0}$) e rimuovendo ad ogni passo un segmento aperto centrale da ogni intervallo. 


Al primo passo $C_{1}$ rimuoviamo da $[0, 1]$ il sotto intervallo $(\frac{1}{3}, \frac{2}{3})$ e rimaniamo quindi con due intervalli $[0, \frac{1}{3}] \cup  [\frac{2}{3}, 1]$

Al secondo passo $C_{2}$ rimuoviamo un segmento aperto centrale in entrambi questi intervalli (avente lunghezza un terzo della lunghezza del segmento, come al primo passo), e otteniamo quattro intervalli ancora più piccoli. 

L'insieme di Cantor consiste di tutti i punti dell'intervallo di partenza $[0, 1]$ che non vengono mai rimossi da questo procedimento ricorsivo: in altre parole, l'insieme che rimane dopo aver iterato questo procedimento infinite volte. 

In maniera, formale:
($C$): $C_{0} \cup C_{1} \cup \dots \cup C_{\infty}$


![Insieme di Cantor](https://upload.wikimedia.org/wikipedia/commons/thumb/5/56/Cantor_set_in_seven_iterations.svg/729px-Cantor_set_in_seven_iterations.svg.png)



**Quali punti rimangono nell'insieme di Cantor**
Ad ogni passo viene rimosso un terzo dei punti inizialmente presenti nell'intervallo $[0, 1]$. Possiamo calcolare tramite la sottostante serie geometrica che l'insieme di Cantor ha misura nulla, poiché ciò "che rimane" ha misura 1 - 1 = 0. 

![Misura Cantor](https://wikimedia.org/api/rest_v1/media/math/render/svg/d980eaa5ded412346ed025bb8e24c00d5a1d3429)

Tuttavia, qualcosa rimane: sicuramente gli estremi, che non vengono mai rimossi sucessivamente.  Quindi 0 e 1, ma anche $\frac{1}{3}$ e $\frac{2}{3}$...

Rimangono anche "insoliti sospetti", come $\frac{1}{4}$. Perché? C'è un trucco, che è pensare ai numeri tra 0 e 1 usando la loro rappresentazione ternaria (quindi in base 3). Questo è perché, visto che rimuoviamo sempre il terzo centrale, è un modo molto utile di ragionare. Ad esempio, il primo segmento a sinistra che rimane in $C_{1}$ equivale all'intervallo $[0, \frac{1}{3}]$, che in base 3 è $[0, 0.02222...]$, mentre il segmento a destra, in base 3, corrisponde a $[22202001021022121212200112011, 1]$.


Alla fine, la polvere di Cantor è solo l'insieme dei numeri che hanno espansione in base 3 solo composta da 0 e 2, mentre vengono esclusi tutto i numeri che contengono, in base 3, degli uno.

*vedi: [Why is 1/4 in Cantor's set](https://www.quora.com/Why-is-the-fraction-1-4-in-the-Cantor-set)*

In generale, i numeri nell'insieme di Cantor possono essere espressi da: 
![cantor equation](https://wikimedia.org/api/rest_v1/media/math/render/svg/122050d8b533cd92e99ad1e651d3cffe1918a3b0)

Ovvero i punti nell'intervallo $[0, 1]$ che scritti in base ternaria hanno come cifre decimali solamente 0 o 2.


## Diagonale di Cantor
La cardinalità degli insiemi infiniti è sempre uguali? No, ovviamente.

**[Diagonale di Cantor](https://en.wikipedia.org/wiki/Cantor%27s_diagonal_argument)**

Ci sono infiniti "contabili" (potenza del numerabile): $\N, \mathbb{I}, \mathbb{Q}$, che sono al livello "inferiore" di infinità ($\aleph_{0}$); e infiniti "non contabili (potenza del continuo, $\aleph_{1}$.

### Teorema di Cantor
>**DEFINIZIONE**
> 
> Per ogni insieme $A$, il suo insieme potenza $\wp(A)$ ha strettamente cardinalità maggiore di $A$. 
> 
> $|A| < |\wp(A)$ 

Contando l'insieme infinto, un insieme con $n$ elementi ha $2^n$ sottoinsieme. Quindi il teorema rimane valido perché $\forall n: 2^{n} > n$

## Ipotesi del continuo
Il'ipotesi del continuo è un'ipotesi avanzata da Cantor riguardo alla possibile esistenza di numeri con una cardinalità intermedia tra $|\N|$ ($\aleph_{0}$)  e $|\R|$ $2^{\aleph_{0}}$.

**Conclusione**
- Insiemi infiniti non equipotenti a $\N$ o $\R$: sì, tramite i numeri transfiniti, iterando la costruzione dell'insieme delle parti": pertanto l'insieme dei numeri transfiniti è, a sua volta, transfinito. 
- Esistono numeri transfiniti tra $\aleph_{0}$ e $2^{\aleph_{0}}$ (ipotesi del continuo)? Questa è una domanda indecidibile, cioè nè la proposizione nè la sua negata sono deducibili nei classici sistemi assiomatici della teoria assiomatica (Zermelo-Frankael).

## Funzioni non calcolabili
Funzione calcolabile significa che se esiste un algoritmo che può svolgere il compito della funzione stessa, cioè se dato un input del dominio della funzione, questa è in grado di restituire il corrispondente output. Tutto ciò che è calcolabile, è Turing-calcolabile.

Se ci sono $\omega$ macchine $< 2^{\omega}$ funzioni. Dato che esitono più funzioni che macchine, ciò significa che esistono funzioni perfettamente definite ma non calcolabili!

**Esempi di funzioni non calcolabili**: 
- [Post Correspondence Problem](https://en.wikipedia.org/wiki/Post_correspondence_problem)
- [Halting problem](https://en.wikipedia.org/wiki/Halting_problem)

