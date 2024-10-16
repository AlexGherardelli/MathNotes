# Relazioni 

- [Relazioni](#relazioni)
  - [Relazione inversa $R^{-1}$](#relazione-inversa-r-1)
  - [Relazioni $A \times A$ (tra un insieme e se stesso)](#relazioni-a-times-a-tra-un-insieme-e-se-stesso)
    - [Proprietà riflessiva](#proprietà-riflessiva)
    - [Proprietà antiriflessiva](#proprietà-antiriflessiva)
    - [Proprietà simmetrica](#proprietà-simmetrica)
    - [Proprietà antisimmetrica](#proprietà-antisimmetrica)
    - [Proprietà transitiva](#proprietà-transitiva)
    - [Casi speciali](#casi-speciali)
  - [Proprietà vere per verità vacua](#proprietà-vere-per-verità-vacua)
      - [Relazione riflessiva e antiriflessiva](#relazione-riflessiva-e-antiriflessiva)
      - [Relazione simmetrica e antisimmetrica](#relazione-simmetrica-e-antisimmetrica)
    - [Relazione nè simmetrica nè antisimmetrica](#relazione-nè-simmetrica-nè-antisimmetrica)
      - [Relazione asimmetrica ma non transitiva](#relazione-asimmetrica-ma-non-transitiva)
      - [Relazione simmetrica ma non riflessiva](#relazione-simmetrica-ma-non-riflessiva)
  - [Relazione transitiva ma non simmetrica né riflessiva](#relazione-transitiva-ma-non-simmetrica-né-riflessiva)
    - [Numero di relazioni su un set](#numero-di-relazioni-su-un-set)
  - [Chiusure](#chiusure)
    - [Chiusura riflessiva ( $r(S)\  o \ R^{+}_{r}$ )](#chiusura-riflessiva--rs--o--r_r-)
    - [Chiusura simmetrica ( $s(S)\  o \ R^{+}_{s}$ )](#chiusura-simmetrica--ss--o--r_s-)
    - [Chiusura transitiva ( $t(S)\  o \ R^{+}_{t}$ )](#chiusura-transitiva--ts--o--r_t-)
- [Relazioni speciali](#relazioni-speciali)
  - [Relazione di equivalenza](#relazione-di-equivalenza)
    - [Classi di equivalenza](#classi-di-equivalenza)
  - [Relazione di ordine parziale ($\leq$)](#relazione-di-ordine-parziale-leq)
  - [Relazione di ordine stretto o totale ($<$)](#relazione-di-ordine-stretto-o-totale-)
    - [Relazione inversa $R^{-1}$](#relazione-inversa-r-1-1)
  - [Relazione di pre-ordine](#relazione-di-pre-ordine)
    - [Partizione](#partizione)


<br/>
<br/>
<br/>
<br/>

> **DEFINIZIONE**: **Relazione**
> Una relazione tra due insiemi $A$ e $B$ è un sottoinsieme del prodotto cartesiano $A \times B$.
>
> Data la coppia $(a, b)$ di un sottoinsieme $R$, $A$ è in relazione con $B$: $R \subseteq A \times B$.
> 
> La proposizione $(a, b) \in R$ viene spesso abbreviata con $xRy$

Esistono relazioni:
- binarie (tra due elementi)
- ternarie (tra tre elementi)
- n-arie (tra n elementi)

Esempi di relazioni già incontrate sono: 
- relazione di identità $U = \{(a, b) \in U \times U: a = b\}$
- relazione di apparteneza $\in_{u} = \{(a, A) \in A \times \wp(U): a \in A$
- relazione di sottoinsieme

## Relazione inversa $R^{-1}$
Dato $R \subseteq A \times B$, possiamo considerare come *nuova* relazione, indicata con $R^{-1}$ la relazione tra gli insiemi $B$ e $A$, cioè $R^{-1} \subseteq B \times A$, ottenuta invertendo l'ordine di tutte le coppie di R. 

Ciò è denominata una **relazione inversa**.

## Relazioni $A \times A$ (tra un insieme e se stesso)
Alcune relazioni godono di speciali proprietà 

### Proprietà riflessiva
*Essere in relazione con se stesso*

> **DEFINIZIONE** 
> Una relazione $R \subseteq A \times A$ è **riflessiva** se $\forall a \in A: (a, a) \in R$ 
> vale a dire
> 
>> $R \subseteq A \times A = \{ \forall a \in A : a \mathrel{R} a \}$

**Esempi**:
- Essere uguale a (uguaglianza)
- Essere sottoinsieme di  $\subseteq$
- Essere divisibile per (divisibilità)
- Essere maggiore o uguale a 
- Essere minore o uguale a

>> NOTA: Il numero di relazioi riflessive su un insieme di cardinalità $n$ è $2^{n^{2}-n}$


### Proprietà antiriflessiva
*Non essere in relazione con se stesso*

> **DEFINIZIONE**: 
> Una relazione $R \subseteq A \times A$  è **antiriflessiva** se $\forall x \in A: (a, a) \notin R$
> vale a dire
> $\forall a \in R: a \not \mathrel{R} a$

**Esempi**:
- Non essere uguale a 
- Essere sottoinsieme proprio di $\subset$
- Essere maggiore di 
- Essere minore di

### Proprietà simmetrica
> **DEFINIZIONE**
>  Una relazione $R \subseteq A \times A$ è **simmetrica**  se $(a, b) \in R, allora\ (b, a) \in R$
> vale a dire
> $R \subseteq A \times A = \{ \forall a, b \in A: a \mathrel{R} b \implies b \mathrel{R} a \}$

**Esempi**:
- Essere uguale a (uguaglianza)
- Essere entrambi dispari 
- Essere entrambi pari
- Essere sposati a
- Essere fratello/sorella di
- Essere omofono di 
- Essere collega di 


### Proprietà antisimmetrica
> **DEFINIZIONE** 
>  Una relazione $R \subseteq A \times A$ è **antisimmetrica** se $(a, b) \in R$ e $(b, a) \in R$, allora $a = b$
> vale a dire
>>  $R \subseteq A \times A = \{ \forall a, b \in A: (a \mathrel{R} b) \land  (b \mathrel{R} a)\implies a = b \}$

**Esempi**:
- essere maggiore o uguale a 
- essere sottoinsieme di $\subseteq$


>> **ATTENZIONE**: antisimmetrica $\not =$ asimmetrica: ($\forall a, b \in A: a \mathrel{R} b \implies \lnot (b \mathrel{R} a$)

Esempi di proprietà asimmetriche: 
- essere maggiore di
- essere minore di
- essere sottoinsieme proprio di
- essere il padre di



### Proprietà transitiva
> **DEFINIZIONE** 
>  Una relazione $R \subseteq A \times A$ è **transitiva** se $(a, b) \in R$ e $(b, c) \in R$, allora $(a, c) \in R$
> vale a dire
>> $R \subseteq A \times A = \{\forall a, b, c \in A: (a \mathrel{R} b) \land (b \mathrel{R} c) \implies a R c \}$

- essere maggiore di
- essere minore di
- essere parallelo a 

s a subset of" (set inclusion, a relation on sets)
"divides" (divisibility, a relation on natural numbers)
"implies" (implication, symbolized by "⇒", a relation on propositions)

> **NOTA**
> Una relazione transitiva è asimmetrica sse è anche antiriflessiva


### Casi speciali


## Proprietà vere per verità vacua

> **IMPORTANTE** Una proprietà per una relazione è vera a ? meno che non ci sia un controesempio che prova che tale proprietà non è soddisfatta. In altre parole, una proprietà non è soddisfatta **se e solo se** c'è un controesempio.

Dato il set $\{1,2,3,4\}$ la relazione $R=\{(1,2),(2,3),(3,4)\}$ dato che non c'è nessun $(a, b) \in R$ che anche $(b, a) \in R$, per cui è *verità vacua* che la relazione è antisimmetrica. (vedi [spiegazioni](https://math.stackexchange.com/questions/255683/antisymmetric-relations))


>>*A word of warning about antisymmetry: Students frequently find it difficult to understand this definition. Keep in mind that this term is defined through an “If...then...” statement. The question that you must ask is: Is it true that whenever there are elements and from where and , it follows that is not related to ? If so, then the relation is antisymmetric. Another way to determine whether a relation is antisymmetric is to examine (or imagine) its digraph. The relation is not antisymmetric if there exists a pair of vertices that are connected by edges in both directions.* [Applied Discrete Structures - Properties of Relations](https://discretemath.org/ads/s-properties-of-relations.html)


#### Relazione riflessiva e antiriflessiva
Ne esiste solo una, la relazione vuota.

$\varnothing \subseteq \varnothing \times \ \varnothing$: unico esempio di relazione contemporaneamente **riflessiva e antiriflessiva**. 

La relazione tra insiemi vuoti è anche **simmetrica**, **antisimmetrica** e **transitiva**, fondamentalmente perché non si può dimostrare il contrario :)


_The empty relation R (defined so that aRb is never true) on a set X is vacuously symmetric and transitive; however, it is not reflexive (unless X itself is empty)._

#### Relazione simmetrica e antisimmetrica
Ci sono fondamentalmente due casi in cui una relazione può essere simmetrica e anti-simmetrica

1. Relazione insieme vuoto
2. Relazione di uguaglianza, ovvero data la relazione $R$ sull'insieme $A$,   le uniche coppie ordinate in $R$ sono nella forma $(x, x)$, dove $x \in A$

Dunque in un insieme di cardinalità $n$, il numero di relazioni simmetriche e antisimmetriche corrisponde al numero delle parti dell'insieme $2^n$.

### Relazione nè simmetrica nè antisimmetrica
TODO

#### Relazione asimmetrica ma non transitiva
Successore, essere il triplo, etc.

Relazioni non transitive
    "is the successor of" (a relation on natural numbers)
    "is a member of the set" (symbolized as "∈")[2]
    "is perpendicular to" (a relation on lines in Euclidean geometry)

#### Relazione simmetrica ma non riflessiva
Essere perpendicolare a, essere parallelo a  

## Relazione transitiva ma non simmetrica né riflessiva


### Numero di relazioni su un set

- Totale: $2^{n^2}$
- Riflessive:  $2^{n^{2}-n}$
- Antiriflessive:  $2^{n^{2}-n}$
- Antisimmetriche: $2^{\frac{n^2+n}{2}}$
- Simmetriche e antisimmetriche: $2^n$
- Transitive: _nessuna formula conosciuta_

## Chiusure
Poniamo che R sia una relazione binaria sull'insieme A. LA relazione R può godere o non godere di certe proprietà, come quella riflessiva, simmetrica o transitiva.

Mettiamo, ad esempio, che R non sia riflessiva. In tal caso, possiamo aggiungere delle coppie ordinate alla relazione per *renderla* riflessiva. La più piccola relazione riflessiva $R^+$ che include R viene chiama chiusura riflessiva di R. 

Esiste solo una chiusura per ogni proprietà. 

[Per sapere di più](https://math24.net/closures-relations.html)

>**DEFINIZIONE**
>Un insieme B è detto chiusura di A rispetto a una proprietà P quando sono soddisfatte le seguenti prorpietà:
>1. B gode della proprietà P
> 2. B è un superinsieme di A
> 3. B è il più piccolo superinsieme di A che soddisfa la proprietà P
> <br>

[Esempi di chiusure](https://math24.net/closures-relations.html)

### Chiusura riflessiva ( $r(S)\  o \ R^{+}_{r}$ )
La chiusura riflessiva si ottiene aggiungendo elementi $(a, a$ alla relazione originale R, per ogni $a \in A$. Formalmente:
$$
r\left( R \right) = R \cup I
$$
dove $I$ è la relazione d'identità, data da 
$$
I = \left\{ {\left( {a,a} \right) \mid \forall a \in A} \right\}
$$

**Esempio**
Consideriamo la relazione $R = \{(1, 2), (2, 4), (3, 3), (4, 2) \}$  sul set $A = \left\{ {1,2,3,4} \right\}$.

Ciò che manca per renderla riflessiva sono le "diagonali"
$$
r\left( R \right) = R \cup I = \left\{ {\left( {1,2} \right),\left( {2,4} \right),{\left( {3,3} \right)},\left( {4,2} \right)} \right\} \cup \left\{ {{\left( \color{red}{1,1} \right)},{\left( \color{red}{2,2} \right)},{\left( \color{red}{3,3} \right)},{\left( \color{red}{4,4} \right)}} \right\} = \left\{ {{\left( \color{red}{1,1} \right)},\left( {1,2} \right),{\left( \color{red}{2,2} \right)},\left( {2,4} \right),{\left( {3,3} \right)},\left( {4,2} \right),{\left( \color{red}{4,4} \right)}} \right\}.
$$


### Chiusura simmetrica ( $s(S)\  o \ R^{+}_{s}$ )
La chiusura simmetrica di una relazione $R$ su $A$ si ottiene aggiungendo gli elementi $(b, a)$ alla relazione $R$ per ogni $(a, b) \in R$.


$$
s\left( R \right) = R \cup {R^{ - 1}}  =  R \cup {R^T} ,
$$

dove $R^{-1} = R^T$ denota l'inverso di $R$. 

**Esempio**
Sia $R = \{(1, 2), (1, 3), (2, 2), (2, 4), (4, 3)\}$ una relazione binaria sull'insieme $A = \{1, 2, 3, 4\}$. Possiamo creare una nuova relazione simmetrica aggiungendo le coppie mancanti: $(2, 1), (3, 1), (4, 2), (3, 4)$.

$$
s\left( R \right) = \left\{ {\left( {1,2} \right),\left( {1,3} \right),\left( {2,2} \right),\left( {2,4} \right),\left( {4,3} \right)} \right\} \cup \left\{ {\left( \color{red}{2,1} \right),\left( \color{red}{3,1} \right),\left( \color{red}{4,2} \right),\left( \color{red}{3,4} \right)} \right\} = \left\{ {\left( {1,2} \right),\left( {1,3} \right),\left( \color{red}{2,1} \right),\left( {2,2} \right),\left( {2,4} \right),\left( \color{red}{3,1} \right),\left( \color{red}{3,4} \right),\left( \color{red}{4,2} \right),\left( {4,3} \right)} \right\}
$$

### Chiusura transitiva ( $t(S)\  o \ R^{+}_{t}$ )
La chiusura transitiva è leggermente più complicata, ma può essere considerata come l'intersezione di tutte le relazioni transitive che contengono $R$.

**Esempi**
- Essere più basso di 
- "Essere antenato di" è la chiusura transitiva della relazione "essere genitore di"
- Esempio degli aereoporti e/o bus multipli per arrivare da punto  A a punto B. Roma e Nairobi non sono direttamente collegate, ma da Roma si può arrivare ad Addis Ababa e da Addis Ababa si arriva a Nairobi, dunque costituendo la chiusura transitiva di "essere collegati da un volo diretto".

La transitività è preservata nell'intersezione ma non nell'unione.



> **_NOTA_** **Chiusura e intersezione**
> Una confusione micidiale qui! O_O Pure nella nota esplicativa.

# Relazioni speciali

## Relazione di equivalenza

> **DEFINIZIONE: RST**
> Una relazione di equivalenza è una relazione $R$ sull'insieme $A$ che gode delle proprietà **riflessiva, simmetrica e transitiva**.

Due elementi $a$ e $b$ legati da una relazione di equivalenza sono chiamati elementi equivalenti e generalmente denotati come a ∼ b or a ≡ b.

**Esempi**:
- essere uguale a
- essere pari / essere dispari
- avere la stessa area di 
- essere simile a (proprietà dei triangoli)
- essere congruente a (proprietà dei triangoli)
  
*Esempi non matematici*:
- $a$ e $b$ vivono nella stessa città
- $a$ e $b$ hanno la stessa età
- $a$ e $b$ sono nati lo stesso giorno
- qualsiasi relazione che ha frase "hanno lo stesso/a"o "sono lo stesso/a"

*La relazione "essere maggiore o uguale a" invece non è una relazioen di equivalenza perché la relazione è riflessiva e transitiva, ma non è simmetria*.

### Classi di equivalenza
La classe di equivalenza di un elemento $[a]_{x}$ è il sottoinsieme formato da tutti gli elementi $x$ cn la stessa proprietà di $a$.

**Esempio**
Sull'insieme $A = \{ a, b, c\}$, la relazione $R = \{ (a, a), (b, b), (c, c), (b, c), (c, b)\}$ è una relazione di equivalenza. Le classi di equivalenza su questa relazione sono:
$$
[a] = \{a\}, \quad [b] = [c] = \{ b, c\}
$$

## Relazione di ordine parziale ($\leq$)

> **DEFINIZIONE: RAT**
> In una relazione $R \subseteq A \times A$, tale relazione è detta d'ordine parziale quando gode delle proprietà **riflessiva, antisimmetrica e transitiva** (RAT)

Un insieme parzialmente ordinato si chiama **poset** (partially ordered set).


## Relazione di ordine stretto o totale ($<$)
> **DEFINIZIONE**
> In una relazione $R \subseteq A \times A$, tale relazione è detta d'ordine stretto quando gode delle proprietà **antiriflessiva e transitiva** (aRT)

Una relazione di ordine stretto è un caso particolare di ordinamento parziale
$$
\forall (a, b) \in A: (a \mathrel{R} b) \lor (b \mathrel{R} a)
$$

### Relazione inversa $R^{-1}$
Nella relazione inversa, le proprietà si mantengono: la nuova relazione è sempre una relazione d'ordine, dunque con proprietà riflessiva, antisimmetrica e transitiva. 



## Relazione di pre-ordine
> **DEFINIZIONE**
> In una relazione $R \subseteq A \times A$, tale relazione è detta di pre-ordine quando gode delle proprietà **riflessiva e transitiva** (RT)

E' una definizione più "lassa" di quella di ordine o di equivalenza, fondamentalmente 

### Partizione
Si verifica quando, in un insieme, ogni elemento appartiene a un gruppo di sottoinsieme.

Dato un insieme A, una famiglia P di sottoinsiemi di A si chiama partizione di A se ogni $a \in A$ appartiene ad uno ed un solo insieme della famiglia P.
