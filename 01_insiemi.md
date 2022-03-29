
# Insiemi

## Assioma di estensione e specificazione
Insieme come collezione di oggetti, chiamati elementi, i quali sono associato ad esso tramite proprietà generali. Insiemi possono contenere qualunque cosa: si può parlare di insiemi di persone, di animali, di cose. Ovviamente, in matematica siamo interessati a insiemi di entità matematiche e delle loro proprietà. 

Un insieme si può definire "elencando" i suoi elementi, che possono appartenere ($\in$) o meno ($\notin$) all'insieme. Un insieme può avere un numero infinito di elementi. In questo caso si chiama insieme infinito, altrimenti è un insieme finito. Il numero di elementi di un insieme si dice **cardinalità**.
<br/>

> **DEFINIZIONE**: **Assioma di Estensione**
> 
> Due insiemi sono uguali se e solo se hanno gli stessi elementi. 

<br/>
Dall'assioma di estensione ne consegue che: 
- Non esiste una nozione di ordinamento all'interno di un insieme
- Le ripetizioni in un insieme non vengono contate
>> **_ESEMPIO 1_**:  $A = \{3, 4, 5\} \quad B = \{5, 5, 3, 4\}$ sono insiemi equivalenti


**Relazione di sottoinsieme**

Come conseguenza dell'assioma di estensione, si può definire la relazione di **essere sottoinsieme di**: 
<br/>

>**DEFINIZIONE: Sottoinsieme**
$B \subset A$ **se e solo se ogni elemento di B è elemento di A**

> **DEFINIIZIONE: Uguaglianza tra insiemi**
> Se $A \subset B$ e $B \subset A$, allora $A = B$

<br/>
Esiste anche un insieme "speciale" che non contiene alcun elemento, l'insieme vuoto $\varnothing = \{\}$. L'insieme vuoto è sottoinsieme di qualunque insieme.

> **DIMOSTRAZIONE** 
> 
> Qualunque elemento di un insieme vuoto è anche un elemento di A. Visto che in un insieme vuoto non ci sono elementi, allora $\varnothing \subset A$

Ne consegue anche che ogni insieme è sottoinsieme di se stesso $A \subseteq A$, dato che ogni elemento di A è elemento di A.
<br/>
>  **DEFINIZIONE**: **Assioma di specificazione**
> Ad ogni insieme $A$ e ad ogni proprietà $P(x)$ che predica sugli elementi $x$ di $A$, corrisponde un insieme $\{x  \in A: P(x)\}$ i cui elementi sono esattamente quelli di $A$ che soddisfano $P$

$$
A = \{x: P(x)\}
$$

Gli insiemi possono avere una **rappresentazione tabulare** (vedi esempio 1) o una **rappresentazione caratteristica**, in cui si evidenzia la condizione necessaria e sufficiente per l'appartenenza di un elemento all'insieme considerato. 


Una proprietà astratta riferita agli elementi di un insieme A in logica si chiama *predicato su A*. Se P è un predicato su A, indicando con x un generico elemento appartenente ad A, con P(x) indichiamo che *x gode della proprietà P*

## Operazioni su insiemi
Così come per i numeri possono essere combinati tra loro usando delle operazioni, così anche per gli insieme esistono una serie di operazioni che possono essere performate su di essi

### Intersezione
$$
A \cap B = \{x: x \in A \quad and \quad x \in B\}
$$

L'intersezione tra A e B contiene gli elementi contenuti in A **e** B: dunque ne risulta un set "più piccolo" di A e B (se A e B sono diversi).

### Unione 
 
$$
A \cup B = \{x: x \in A \quad or \quad x \in B \}
$$

L'unione tra A e B contiene gli elementi contenuti in A **o** B: dunque ne risulta un set "più grande" sia di A che di B (se A e B sono diversi).
<br/>
> **DEFINIZIONE**: **Assioma dell'unione**
> 
> Per ogni collezione $C$ di insiemi, esiste un insieme $U$ che contiene tutti gli elementi che appartengono almeno ad un insieme della collezione.

<br/>

### Differenza
$$
A - B = \{x : x \in A \quad and \quad x \notin B\}
$$

La differenza tra gli insiemi $A$ e $B$ è l'insieme delle cose che sono in A ma non sono in B: ne risulta un set "più piccolo" di A. 

> **_NOTA_**
> 
> Intersezione e differenza:
>
> $A \cap B = A - (A -B)$ 
> 
> Differenza e sottoinsiemi:
> $A \subset B$ sse $A - B = \varnothing$
> <br/>


### Complemento
Il complemento è un tipo particolare di differenza che si verifica quando $B \subset A$, $A - B$ si chiamna complemento di B rispetto ad A$

$$
\bar B = \{x \in A: x \notin B\}
$$

### Proprietà delle operazioni sugli insiemi
Sia per l'unione che per l'intersezione valgono le seguenti proprietà 

**Intersezione e unione con se stesso**
$$
A \cap A = A
\\
A \cup A = A
\\
A - A = \varnothing
$$

**Intersezione e unione con un insieme vuoto**
$$
A \cap \varnothing = A
\\
A \cup \varnothing = A
\\
A - \varnothing = A
\\ 
\varnothing - A = \varnothing
$$ 

**Proprietà commutativa**
$$
A \cap B = B \cap A
\\ 
A \cup B = B \cup A
$$ 

**Proprietà associativa**
$$
A \cap (B \cap C ) = (A \cap B) \cap C
\\
A \cup (B \cup C ) = (A \cup B) \cup C
$$ 

**Proprietà distributiva**

Dell'unione sull'intersezione e viceversa

$$ 
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
\\
A \cup (B \cap C) = (A \cup B) \cap (A \cup C)
$$ 

**Complemento: cambia relazione di unione con intersezione (e viceversa)**
$$
(A \cup B)' = \bar A \cap \bar B
\\ 
(A \cap B)' = \bar A \cup \bar B
$$

## Power Set (Insieme potenza)

> **Sottoinsiemi di A**
>
> Se un insieme finito a _n_ elementi, allora ha $2^n$ sottoinsiemi.


L'insieme potenza è l'nsieme di tutti i sottoinsiemi di $A$, indicato con	$\wp (A)$

$$ 
\wp (A) = \{X : X \subseteq A \} 
$$

>> **NOTA** 
>> 
>> $\wp (\mathbb{R}^2)$ dovrebbe sconquassare il cervello.
>>
>> $\mathbb{R}^2$ è l'insieme delle coordinate del piano Cartesiano. Un qualsiasi sottoinsieme di $\mathbb{R}^2$ (un elemento dunque $\wp (\mathbb{R}^2)$ ) dunque è un insieme di punti nel piano. 
>> 
>> Fondamentalmente, $\wp (\mathbb{R}^2)$ contiene qualsiasi funzione immaiginabile, qualsiasi "pagina" scritta o mai scritta (che in fondo sono sempre coordinate sul piano), una biografia non scritta della tua vita e così via.
>>  
>> Incredibile che cinque simboletti rappresentino una così grande vastità di cose. 

## Prodotto cartesiano

**Coppia ordinata**

Dati due insiemi $A$ e $B$, la coppia ordinata $(a, b)$ è un insieme cosituito dal primo elemento dell'insieme $A$ con il primo elemento dell'insieme $B$.  
La **coppia ordinata** può essere utilizzata in particolar eper indicare un particolare ordinamento all'interno di un insieme. 

**Prodotto Cartesiano**

Dati due insiemi A e B, il prodotto cartesiano $A \times B$ è **l'insieme** composto dalle coppie ordinate $(a, b)$, tali che $a \in A$ e $b \in B$

$$
A \times B = \{ (a, b) : a \in A, b \in B     \}
$$

> **ESEMPIO**
> 
> Se $A = \{ k, l, m\}$ e $B = \{ a, b, c \} $
> 
> allora il loro prodotto cartesiano è  
> 
> $ A \times B = \{ (k, a), (l, b), (m, c) \}$

Si possono ovviamente andare oltre la coppia ordinata e avere triple, quadruple, n-tuple ordinate. 

$$
 A_{1} \times A_{2} \times ... \times A_{n} = \{ (x_{1}, x_{2}, ..., x_{n}: x_{i} \in A_{i} \ 
\text{for each} \ i = 1, 2, ..., n \}
$$

**Proiezione**

Sia $S \subseteq A \times B$. Si dice proiezione $S$ su $A$ l'insieme $\{a : a \in A \ e \ (a, b), \text{per almeno un } b \in B $}

> **ESEMPIO**
> 
> Sia $S$ il sottoinsieme di $\mathbb{N} \times \mathbb{N}$ costituito dalle coppie $(n, m)$ tali che $n+m = 3$
> 
> $S = \{(0, 3), (1, 2), (2, 1), (3, 0)\}$
> La proiezione di $S$ su entrambe le sue componenti è $S = \{ 0, 1, 2, 3\}$


## Antinomie degli insiemi - Russel's Pararadox
AGGIUNGERE