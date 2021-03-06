# Numeri Naturali e Induzione
- [Numeri Naturali e Induzione](#numeri-naturali-e-induzione)
  - [Assiomi di Peano](#assiomi-di-peano)
- [Induzione](#induzione)
  - [Induzione non per $P(0)$](#induzione-non-per-p0)
  - [Induzione completa](#induzione-completa)

A differenza di quanto accaduto in geometria, i matematici antichi non si posero il problema di caratterizzare i numeri naturali. La prima caratterizzazione è di Campano da Novara nella seconda metà del XIII secolo. 

Il discorso viene ripreso nella fine del 1800, quando l'intero mondo matematico si sta dedicando a una formalizzazione rigorosa della disciplina. 

Gotlib Frege pubblica nel 1884 la sua opera magna, che contiene la sua rigorosa definizione dei numeri naturali, definiti ricorsivamente a partire dallo zero.

Giuseppe Peano nel 1891 propone una versione assiomatica basata su tre concetti primitivi: **lo zero, il numero e il successivo**.

## Assiomi di Peano
1. Lo zero è un numero ($0 \in \mathbb{N}$)
2. Esiste una funzione $S: \mathbb{N} \to \mathbb{N}$ chiamata *successore*
3. Se $a, b \in \mathbb{N}$ e $S(a) = S(b)$, allora $a = b$
4. Lo zero non è successore di nessuno: se $a \in \mathbb{N}$, allora $S(a) \not = 0$
5. Ogni sottoinsieme di numeri naturali che contenga lo zero e il successore di ogni proprio elemento coincide con l'intero insieme dei numeri naturali: se $A \subseteq \mathbb{N}$ è tale che $0 \in A$ e inoltre $n \in A \implies S(n) \in \mathbb{N}$, allora $A = \mathbb{N}$  (assioma dell'induzione)

# Induzione
Il principio di induzione è una tecnica di dimostrazione che consente di dimostrare la validità di una tesi dalla verifica di due condizioni: la validità del *passo zero* e la validità del *passo induttivo*. [Principio di Induzione - YouMath](https://www.youmath.it/lezioni/analisi-matematica/successioni/701-dimostrazioni-con-il-principio-di-induzione.html)

E' utilizzato per dimostrare che una proprietà $P$ vale per una serie infinita di numeri - per verificare ciò basta che sia vero per $n$ e per $n + 1$, e ne conseguirà che è valida per tutti i numeri. 

**Principio di induzione**: $P(n) da dimostrare sia vera per $\forall n \in \mathbb{N}$

1. **Caso base**: dimostrazione verità di $P(0), \ n \leq n_{0} \leq 0$
2. **Passo induttivo**: si ammette la verità di $P(n)$, si dimostra la verità di $P(n+1)$

>**DEFINIZIONE**
>Se $P$ è un predicato su $\mathbb{N}$ tale che vale $P(0)$, e inolte $P(n) \implies P(n + 1)$, allora $\forall n, P(n)$

$$
\frac{P(0) \quad \quad P(n) \implies P{n+1}}{\forall N, P(n)}
$$

## Induzione non per $P(0)$
Esistono alcuni casi che non possono essere risolti se nel caso base partiamo da $P(0)$ e.g. bisogna partire dai numeri $n > 2$. In questo caso il principio di induzione rimane valido, ma va applicato su una nuova proprietà $Q(n)$ ottenuta modificando $P(n)$, in modo tale che sia vera per la traccia del prolema da verificare 

<!-- ESEMPIO MANCANTE-->

## Induzione completa
In alcuni casi (come quello degli alberi binari) occorre utilizzare un diverso modo di applicazione del principio di induzione: 
1. Introduzione di una nuova proprietà $Q(n)$, ottenuta partendo dalla proprietà $P(n)$, applicata però a m, ovvero tutti i numeri più piccoli di $n$ ($m \leq n$)
2. Applicazione del caso base e del passo induttivo per $Q(n + 1)$
