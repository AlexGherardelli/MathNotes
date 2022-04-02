# Algebra e modelli
- [Algebra e modelli](#algebra-e-modelli)
  - [Connettivi logici](#connettivi-logici)
  - [Corrispondenze](#corrispondenze)
  - [Tavole di verità delle proposizioni](#tavole-di-verità-delle-proposizioni)
  - [Conseguenza semantica](#conseguenza-semantica)
- [Implicazione **SONO QUI**](#implicazione-sono-qui)
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
| soddisfa $\models$ | sottoinsieme $\subseteq$ | minore o uguale $\leq$ |

- La logica non è altro che funzioni che mappano i predicati in top e bottom (connessione tra Logica e Algebre di Boole)
- Gli elementi di un insieme che corrispondon agli omomorfismo corrispondo anche a  delle funzionei che mappano i predicati logici in $\top$ e $\bot$.

## Tavole di verità delle proposizioni
| $P$    | $Q$    | $P \land Q$ | $P \lor Q$ | $\lnot P$ |
|--------|--------|-------------|------------|-----------|
| $\top$ | $\top$ | $\top$      | $\top$     | $\top$    |
| $\top$ | $\bot$  | $\bot$      | $\top$     | $\bot$    |
| $\bot$ | $\top$ | $\bot$      | $\top$     | $\top$    |
| $\bot$ | $\bot$ | $\bot$      | $\bot$     | $\top$    |

    RIVEDERE DEFINIZIONE

> **DEFINIZIONE** modelli m: 
> simboli proposizionali $\{T, F\}$
> Funzioni che associano preposizion a un'elemento ell'insieme $\{T, F\}$ (che corrispondono a $\top$ e $\bot$ dell'algebra di Boole)


m si estende alle proposizioni (interpretazioni come segue:
m(falso) = F
e per le proposizioni composete  comn le tavole di verità

Combinando le proposizioni con i connettivi logici otteniamo la *logica proposizionale*.

## Conseguenza semantica
La conseguenza semantica ($\models$) è un'operazione che corrisponde al $\leq$ delle algebre di Boole (o al $\subseteq$ degli insiemi).

$$
P \land Q \models P \quad \} \quad A_{1}, A_{2}, \dots, |A_{n} \models B
$$

| Insiemi                                  | Algebra di Boole                    | Logica                                 |
|------------------------------------------|-------------------------------------|----------------------------------------|
| $\subseteq$                              | $\leq$                              | $\models$                              |
| $A_{1}, A_{2}, \dots, A_{n} \subseteq A$ | $A_{1}, A_{2}, \dots, A_{n} \leq A$ | $A_{1}, A_{2}, \dots, A_{n} \models A$ |

# Implicazione **SONO QUI**
$A \implies B$ è la più debole (cioè l'insieme di modelli più grande) proposizione x tale che $x, A \models B$

- Implicazione come promessa 
- Implicazione come A not B qualcosa

## Tabelle di verità dell'implicazione
Nel mondo della logica la proposizione $A \implies B$ contienie il minimo d'informazione possibile ovvero che:
- se è vero che $A \implies B$, allora $A$ è vera



    RIVEDERE

## Algebra di Heyting
L'algebra di Heyting è un reticolo distributivo dove per ogni copppia di $A$ e $B$ esiste lo pseudocomplemento di A rispetto a B: $A \implies B$, ovvero il più grande elemento x tale che $x \land A \leq B$
$$
\forall A, B \exists A \implies B
$$

Ogni algebra di Boole è anche un'algebra di Heyting, ma non è vero il contrario.