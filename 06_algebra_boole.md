# Reticoli e algebre di Boole
- [Reticoli e algebre di Boole](#reticoli-e-algebre-di-boole)
  - [Reticoli](#reticoli)
  - [Algebra di Boole](#algebra-di-boole)
    - [Convulazione](#convulazione)
    - [Leggi di De Morgan](#leggi-di-de-morgan)

>**DEFINIZIONE*: Struttura algebrica
> Una struttura algebrica è un insieme dotato di operatori che soddisfano determinate proprieta o assiomi. Esempi di strutture algebriche sono i reticoli, i monoidi, i gruppi, gli anelli, e i campi.

Un **semireticolo** è un insieme parzialmente ordinato (POSET) che gode dell'operazione binaria di JOIN ($\lor$) per ogni insieme finito non-vuoto.

## Reticoli
Un **reticolo** è un insieme parzialmente ordinato (poset), dotato di due operatori binari, JOIN ($\lor$) e MEET ($\land$).

Con JOIN intendiamo "il superiore tra"
Con MEET intendiamo "l'inferiore tra"

Un **reticolo distributivo** è un reticolo dove ogni elemento è verificato dalla proprietà distributiva.

## Algebra di Boole
>**DEFINIZIONE**
> 
> Un'algebra di Boole è un reticolo distributivo dove ogni elemento ha un complemento.
> 
E' quindi una struttura costituita da una sestupla: un insieme $A$, dotato di operazioni due operazioni binarie $\land$ MEET e $\lor$ JOIN, un'operazione unaria complemento $\lnot$ e due elementi 0 e 1 in A, denominati $\top$ top e $\bot$ bottom, tale che $\forall a, b, c \in A$ , valgano i seguenti assiomi:

**Associatività**
$$
a \lor (b \lor c) = (a \lor b) \lor c
\\
a \land (b \land c) = (a \land b) \land c
$$

**Commutatività**
$$
a \lor b = b \lor a 
\\
a \land b = b \land a
$$

**Assorbimento**
$$
a \lor (b \land a) = a
\\
a \land (b \lor a) = a
$$

**Identità \ Idempotenza**
$$
a \lor \bot = a
\\
a \land \top = a
$$

**Distributività**
$$
a \lor (b \land c) = (a \land b) \lor (b \land c)
\\
a \land (b \lor c) = (a \lor b) \land (b \lor c)
$$

**Completento**
$$
a \lor \lnot a = \top
\\ 
a \land \lnot a = \bot
$$



Questa struttura algebrica ben rappresenta le proprietà essenziali sia della teoria degli insiemi che della logica - che è il motivo poi per cui è in questo corso. Si può considerare come una generalizzazione delle algebre dei sottoinsiemi potenza

### Convulazione

### Leggi di De Morgan