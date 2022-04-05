# Algebra e modelli
- [Algebra e modelli](#algebra-e-modelli)
  - [Connettivi logici](#connettivi-logici)
  - [Corrispondenze](#corrispondenze)
  - [Tavole di verità delle proposizioni](#tavole-di-verità-delle-proposizioni)
  - [Modelli](#modelli)
    - [Conseguenza semantica](#conseguenza-semantica)
- [Parte 2: l'implicazione](#parte-2-limplicazione)
  - [Tabelle di verità dell'implicazione](#tabelle-di-verità-dellimplicazione)
  - [Algebra di Heyting](#algebra-di-heyting)


La logica proposizionale è un sistema logico intimamente connesso con l'algebra d Boole. Molti concetti sintattici sono quasi gli stessi dell'algebra di Boole, con piccoli cambiamenti nella notazione e nella terminologia.

**Sintassi**: sistema di regole per la manipolazione dei termini
**Semantica**: l'interpretazione della sintassi.

Combinando le proposizioni ($P, Q$) con i connettivi logici $\land, \lor, \not, \implies$ otteniamo **la logica proposizionale** 

## Connettivi logici
Se - allora (struttura logica): se $P$, allora $Q$

Se $\lnot P$, allora $Q$ o $R$ -> $Q \lor R$ -> $Q \cup R$

Se $P$, allora $Q$ e $R$ -> $Q \land R$ -> $Q \cap R$ 

## Corrispondenze

| Logica             | Insiemi                  | Algebre di Boole       |
|--------------------|--------------------------|------------------------|
| Proposizioni       | Sottoinsiemi             | Elementi               |
| Modelli            | Elementi                 | Omomorfismi            |
| and $\land$        | intersezione $\cap$      | meet $\land$           |
| or $\lor$          | unione $\cup$            | join $\lor$            |
| not $\lnot$        | complemento  $\bar{ }$       | complemento $\bar{ }$     |
| modello $\models$ | sottoinsieme $\subseteq$ | minore o uguale $\leq$ |

- La logica non è altro che funzioni che mappano i predicati in top e bottom (connessione tra Logica e Algebre di Boole)
- Gli elementi di un insieme che corrispondon agli omomorfismo corrispondo anche a  delle funzionei che mappano i predicati logici in $\top$ e $\bot$.

## Tavole di verità delle proposizioni

| $P$    | $Q$    | $P \land Q$ | $P \lor Q$ | $\lnot P$ |
|--------|--------|-------------|------------|-----------|
| True | True | True     | True   | True    |
| True | False  |False      | True     | False    |
| False | True | False      | True    | True   |
| False| False | False     | False    | True    |

## Modelli
I modelli corrispondono agli elementi del mondo degli insiemi, e sono funzioni che assegnano un valore di verità a delle proposizioni.

> **DEFINIZIONE** modelli m:
> Funzioni che associano una preposizione a un'elemento dell'insieme $\{T, F\}$ (che corrispondono a $\top$ e $\bot$ dell'algebra di Boole)

$~~~~~~~~~~~$

**Esempio**:
- $P$ = essere un numero primo
- $Q$ = essere minore di 10

Nel mondo degli insiemi, si può vedere $P$ e $Q$ come due sottoinsiemi di $\mathbb{N}$, e i numeri primi minori di 10 come $P \cap Q$.

Se ne deduce che
$$
P \cap Q \subseteq P
$$
e che per ogni numero $n$, se $n \in P \cap Q$, allora $n \in P$.

In logica, possiamo scrivere una cosa completamente identica indicando che **per ogni modello m, se m soddisfa $P \land Q$, allora m soddisfa P:

$$
P \land Q \models P
$$

Il numero 9 è un numero inferiore a 10 ($9 \in Q$), ma non è un numero primo ($9 \notin P$).

Prendendolo come modello, si può dire che $m(Q) = T$ e $m(P) = F$, oppure $\models_{m}Q$, che si legge *m soddisfa Q*.

### Conseguenza semantica
Il modello ($\models$) viene chiamato anche **conseguenza semantica**, che è un'operazione che corrisponde al $\leq$ delle algebre di Boole (o al $\subseteq$ degli insiemi).

| Insiemi                                  | Algebra di Boole                    | Logica                                 |
|------------------------------------------|-------------------------------------|----------------------------------------|
| $\subseteq$                              | $\leq$                              | $\models$                              |
| $A_{1}, A_{2}, \dots, A_{n} \subseteq A$ | $A_{1}, A_{2}, \dots, A_{n} \leq A$ | $A_{1}, A_{2}, \dots, A_{n} \models A$ |

$~~~~~~~~~~~$

> La notazione può essere estesa da un esempio come $P \land Q \models P$, alla sua generalizzazione, usando $A_{1}, A_{2}, \dots, |A_{n}$ per indicare una serie di formule:
> 
> $$
>A_{1}, A_{2}, \dots, |A_{n} \models B
>$$
>
> Per ogni modello m, se m soddisfa $A_{1}, A_{2}, \dots, |A_{n}$, allora m soddisfa B
> 
> Oppure, B consegue semanticamente da $A_{1}, A_{2}, \dots, |A_{n}$

**Quando $n=0$, ciò significa che non c'è premessa, quindi per ogni modello m, m soddisfa $B$**
$$
\models B
$$

Quindi B è **valida** - B è una tautologia.

$~~~~~~~~~~~$

# Parte 2: l'implicazione

$A \implies B$ è la più debole (cioè l'insieme di modelli più grande) proposizione x tale che $x, A \models B$

- Implicazione come promessa 

> **NOTA BENE**
> 
> A implica B è semanticamente equivalmente a not A or B
> 
> $A \implies B = \lnot A \lor B$


## Tabelle di verità dell'implicazione
Nel mondo della logica la proposizione $A \implies B$ contienie il minimo d'informazione possibile ovvero che:
- se è vero che $A \implies B$, allora $A$ è vera

| $A$ 	| $B$ 	| $A \implies B$ 	|
|---	|---	|---	|
| True 	| True 	| True 	|
| True 	| False 	| False 	|
| False 	| True 	| True 	|
| False 	| False 	| True 	|


## Algebra di Heyting
L'algebra di Heyting è un reticolo distributivo dove per ogni copppia di $A$ e $B$ esiste lo pseudocomplemento di A rispetto a B: $A \implies B$, ovvero il più grande elemento x tale che $x \land A \leq B$
$$
\forall A, B \exists A \implies B
$$

Ogni algebra di Boole è anche un'algebra di Heyting, ma non è vero il contrario.
