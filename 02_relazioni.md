# Relazioni 

> **DEFINIZIONE**: **Relazione**
> Una relazione tra due insiemi $A$ e $B$ è un sottoinsieme del prodotto cartesiano $A \times B$.
>
> Data la coppia $(a, b)$ di un sottoinsieme $R$, $A$ è in relazione con $B$: $R \subseteq A \times B$.**
> 
> La proposizione $(a, b) \in R$ viene spesso abbreviata con $xRy$

Esistono relazioni:
- binarie (tra due elementi)
- ternarie (tra tre elementi)
- n-arie (tra n elementi)

Esempi di relazioni già incontrate sono: 
- relazione di identità $ U = \{(a, b) \in U \times U: a = b\}$
- relazione di apparteneza $\in_{u} = \{(a, A) \in A \times \wp(U): a \in A$
- relazione di sottoinsieme

### Relazione inversa $R^{-1}$
Dato $R \subseteq A \times B$, possiamo considerare come *nuova* relazione, indicata con $R^{-1}$ la relazione tra gli insiemi $B$ e $A$, cioè $R^{-1} \subseteq B \times A$, ottenuta invertendo l'ordine di tutte le coppie di R. 

Ciò è denominata una **relazione inversa**.

## Relazioni $A \times A$ (tra un insieme e se stesso)
Alcune relazioni godono di speciali proprietà 

### Proprietà riflessiva
> **DEFINIZIONE** 
> Una relazione $R \subseteq A \times A$ è **riflessiva** se $\forall(x, y) \in A: (x, y) \in R $ 
> vale a dire
> 
>> $ R \subseteq A \times A = \{ \forall a \in A : a \mathrel{R} a \}$
> 

### Proprietà antiriflessiva
> **DEFINIZIONE**: 
> Una relazione $R \subseteq A \times A$  è **antiriflessiva** se \forall(x, y) \in A: (x, y) \notin R 
> vale a dire
> 
>> $ R \subseteq A \times A = \{ \forall a \in A : a \not \mathrel{R} a \}$

### Proprietà simmetrica
> **DEFINIZIONE**
>  Una relazione $R \subseteq A \times A$ è **simmetrica**  se $(a, b) \in R, allora\ (b, a) \in R$
> vale a dire
>>  $R \subseteq A \times A = \{ \forall a, b \in A: a \mathrel{R} b \implies b \mathrel{R} a \}$

### Proprietà antisimmetrica
> **DEFINIZIONE** 
>  Una relazione $R \subseteq A \times A$ è **antisimmetrica** se $(a, b) \in R$ e $(b, a) \in R$, allora $a = b$
> vale a dire
>>  $R \subseteq A \times A = \{ \forall a, b \in A: (a \mathrel{R} b) \land  (b \mathrel{R} a)\implies a = b \}$

### Proprietà transitiva
> **DEFINIZIONE** 
>  Una relazione $R \subseteq A \times A$ è **transitiva** se $(a, b) \in R$ e $(b, c) \in R$, allora $(a, c) \in R$
> vale a dire
>> $R \subseteq A \times A = \{\forall a, b, c \in A: (a \mathrel{R} b) \land (b \mathrel{R} c) \implies a R c \}$

#### Esempi

**Insieme vuoto**
$\varnothing \subseteq \varnothing \times \ \varnothing$: unico esempio di relazione contemporaneamente **riflessiva e antiriflessiva**. La relazione tra insiemi vuoti è anche **simmetrica**, **antisimmetrica** e **transitiva**, fondamentalmente perché non si può dimostrare il contrario :)


**Relazione simmetrica e antisimmetrica**
- Relazione di uguaglianza
- Relazione insieme vuoto


## Chiusure

## Classi di equivalenza

# Relazioni speciali

## Relazione di equivalenza

## Relazione di ordine parziale

## Relazione di ordine stretto (totale)

## Relazione di pre-ordine

### Partizione