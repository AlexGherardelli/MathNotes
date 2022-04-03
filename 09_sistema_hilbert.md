# Il sistema di Hilbert
- [Il sistema di Hilbert](#il-sistema-di-hilbert)
  - [Definizione di sistema logico - assiomatico](#definizione-di-sistema-logico---assiomatico)
  - [Il sistema deduttivo di Hilbert](#il-sistema-deduttivo-di-hilbert)
    - [Assiomi](#assiomi)
    - [Regola di inferenza (*Modus Ponens*)](#regola-di-inferenza-modus-ponens)
  - [Dimostrazione nel sistema di Hilbert](#dimostrazione-nel-sistema-di-hilbert)
    - [Dimostrazione di $A \implies A$](#dimostrazione-di-a-implies-a)
    - [Teorema di deduzione](#teorema-di-deduzione)

## Definizione di sistema logico - assiomatico
>**DEFINIZIONE**:
> 
> Un **sistema logico-assiomatico** è un sistema dove vengono definite:
> - una serie di assiomi, ovvero proposizioni fondanti per la teoria, assunte senza dimostrazione, 
> - delle regole di inferenza che ci permettano di dedurre altre proposizioni

## Il sistema deduttivo di Hilbert

### Assiomi
0. $A \implies A$ (*identità*)
1. $B \implies (A \implies B)$
2. $(A \implies (B \implies C)) \implies (A \implies B) \implies (A \implies C)$ (*transitività*)
3. $\lnot A \implies \lnot B) \implies (B \implies A)$

E poi l'assioma zero è in realtà un teorema, perché derivabile in realtà dagli altri.

In realtà sono **schemi di assiomi**, perché in realtà questi quattro assiomi sono applicabili a qualsiasi proposizione abbia tale struttura, sostituendo ogni lettera si può sostituire altre poposizioni.

**Esempi**
$(P \implies Q) \implies (P \implies Q)$ è uno schema di $A \implies A$ (*assioma zero*)

$(P \land Q) \implies ((Q \implies R) \implies (P \land Q)$ (*primo assioma*)

### Regola di inferenza (*Modus Ponens*)

$$
\frac{\vdash A \quad \vdash A \implies B}{B}
$$

Se ho dimostrato la validità della formula $A$ e della formula $A \implies B$, allora la formula $B$ può essere correttamente dedotta da $A$ e $A \implies B$

>> **NOTA** il *modus ponens* è praticamente identico all'induzione in cui
$$
\frac{P(0) \quad P(n+1)}{\forall n, P(n)}
$$ 

## Dimostrazione nel sistema di Hilbert
> **DEFINIZIONE**: senza premesse
>  Una dimostrazione di una proposizione $A$ è una sequenza di proposizioni, di cui $A$ è l’ultima, ciascuna delle quali è una istanza di assioma o è ottenuta per *modus ponens* da due proposizioni che la precedono.

> **DEFNIZIONE**: con premesse
> Una dimostrazione di una proposizione $A$ da un insieme di premesse $\Gamma = {B_{1}, B_{1}, \dots, B_{n}}$ è una sequenza di proposizioni, di cui A è l’ultima, ciascuna delle quali è un’istanza di assioma, o una proposizione in $\Gamma$, o è ottenuta per modus ponens da due proposizioni che la precedono
> ovvero
  > $$
  B_{1}, B_{2}, \dots, B_{n} \vdash A
  > $$
>> A è dimostrabile - A è un teorema.

$~~~~~~~~~~~~~~~$

### Dimostrazione di $A \implies A$
1. Prendiamo il secondo assioma e istanziamolo con $A = A, B = A \implies A, C = A)$ :  

$$
A \implies ((A \implies A) \implies A) \implies (A \implies (A \implies A)) \implies (A \implies A)
 $$ 
2. Prendiamo il primo assioma e lo istanziamo con $A \implies (A \implies A)$
3. Quindi per modus ponens, poniamo (1) e (2) come premesse, e la seconda parte di (2) la possiamo derivare per modus ponens
$$
\frac{A \implies (A \implies A) \quad \quad \quad A \implies ((A \implies A) \implies A) \implies (A \implies (A \implies A)) \implies (A \implies A)}{(A \implies (A \implies A)) \implies (A \implies A)}
$$
4. Usando di nuovo in modus ponens, poniamo come premesse il risultato del primo passaggio di MP e il primo assioma, instanziato come $A \implies (A \implies A)$
$$
  \frac{A \implies (A \implies A) \quad \quad (A \implies (A \implies A)) \implies (A \implies A) }{A \implies A}
$$


E voilà, abbiamo appena dimostrato che $A \implies A$

In sintesi:
```
1. (A→((A→A)→A))→((A→(A→A))→(A→A)) (Assioma 2)
2. A→((A→A)→A) (Assioma 1)
3. (A→(A→A))→(A→A) (MP 1, 2)
4. A→(A→A) (Assioma 1)
5. A→A (MP 3, 4)
```

### Teorema di deduzione
In maniera totalmente simile al **teorema di deduzione semantica**,

$$
C_{1}, C_{2}, \dots, C_{n}, A \models B \iff C_{1}, C_{2}, \dots, C_{n} \models A \implies B
$$

nel **teorema di deduzione**
$$
C_{1}, C_{2}, \dots, C_{n}, A \vdash B \iff C_{1}, C_{2}, \dots, C_{n} \vdash A \implies B
$$

Che significa: 
- avendo dimostrato $A \implies B$, posso dimostrare $B$ includendo $A$ nelle premesse
- se riesco a dimostrare $B$ a partire dalle sue premesse, incluso $A$, allora posso dedurre che $A \implies B$ senza usare $A$ tra le sue premesse

Questo in realtà semplifica *enormemente* la dimostrazione $A \implies A$, perché genera una conclusione a partire da un sequente ovvio, cioè che data $A$ come premessa ne consegue $A$.
$$
\frac{A \vdash A}{\vdash A \implies A}
$$

**Esempio**
$$
(A \implies B) \implies ((B \implies C) \implies (A \implies C))
$$
