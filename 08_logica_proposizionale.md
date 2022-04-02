# Logica proposizionale
- [Logica proposizionale](#logica-proposizionale)
    - [Tavole di verità](#tavole-di-verità)
  - [Teorema di deduzione semantica](#teorema-di-deduzione-semantica)
  - [Equivalenza semantica](#equivalenza-semantica)
  - [Completezza funzionale](#completezza-funzionale)
  - [Formule valide e soddisfacibili](#formule-valide-e-soddisfacibili)
  - [Correttezza e completezza](#correttezza-e-completezza)
  - [Tableau proposizionali](#tableau-proposizionali)
    - [Foglie chiuse](#foglie-chiuse)
    - [Validità](#validità)
    - [Metodo dei Tableau](#metodo-dei-tableau)
<br>


L'affermazione: *tutti i numeri naturali maggiori di due sono somme di due numeri primi" è un enunciato?
Sì, certo, è la **congettura di Goldbach**. Che nessuno ha mai dimostrato essere vera o falsa (anche se è verificata per numeri fino a $4*10^18), ma è sicuramente o vera o falsa.

Enunciati formati da una sola affermazione (e.g. "la neve è bianca") sono *enunciati atomici*, se prevedono connettivi logici (AND, OR, NOT), allora si dicono *enunciati composti*.

**Proposizioni atomiche**: P, Q, R, falso 
**Proposizioni composte**: $P \land Q$, $P \lor Q$, $P \implies Q$, $\lnot P$

Tenendo conto che i connettivi logici sono, in fondo, operazioni sugli enunciati, i connettivi saranno definiti mediante le *tavole di verità*.

**Sintassi**
Insieme delle proposizioni, ovvero oggetti sintatici (indicati con a,b)trutturate in diversi modi possibili: $P, Q, False, A \lor B, A \land A, A \implies B, \lnot A$

Simboli proposizionali P, Q: minima descrizione possibile della proposizione

**Semantica** (significato delle espressioni)
Modelli m: associanno simboli proposizionali ai valori di True o False attraverso le tavole di verità.

### Tavole di verità

| $A$ 	| $B$ 	| $\lnot A$ 	| $A \land B$ 	| $A \lor B$ 	| $A \implies B$ 	|
|---	|---	|---	|---	|---	|---	|
| V 	| V 	| F 	| V 	| V 	| V 	|
| V 	| F 	| (F) 	| F 	| V 	| F 	|
| F 	| V 	|  V 	| F 	| V 	| V 	|
| F 	| F 	| (V) 	| F 	| F 	| V 	|


## Teorema di deduzione semantica
![Teorema Deduzione semantica](assets/teorema_deduzione_semantica.png)

Generalizzando:

$$
C_{1}, C_{2}, \dots, C_{n} \models A \implies B
$$

in cui $C_{1}, C_{2}, \dots, C_{n}$ sono **sequenti**, e se 
$$
n = 0 \quad \quad A \models B
$$


## Equivalenza semantica
> **DEFINIZIONE**
> Date due proposizioni A, B , esse sono semanticamnete equivalenti ($\equiv$) quando hanno gli stessi valori di verità per ogni interpretazione

**Esempi di equivalenze logiche**
$$
A \equiv \lnot \lnot A
\\
A \equiv A \land A
\\
A \equiv A \lor A
\\
A \implies B \equiv \lnot B \implies \lnot A
\\
A \implies B \equiv \lnot A \lor B
\\
A \land B \equiv \lnot (A \implies \lnot B)
\\
A \lor B \equiv \lnot (A \implies B)
\\
A \land B = \lnot (\lnot A \lor \lnot B) \ \text{legge di De Morgan}
\\
A \lor B = \lnot (\lnot A \land \lnot B) \ \text{legge di De Morgan}
$$

## Completezza funzionale
Per ottenere un operatore, è possibile utilizzarne altri due:
-  $\implies$ e $falso$
-  $\land$ e $\lnot$

Con queste due coppie di operatori possiamo ottenere tutti gli altri operatori e crearne di nuovi.

**Esempio**
XOR $\veebar$:

$$
A \veebar B \equiv (A \land \lnot B) \lor (B \land \lnot A)
$$

## Formule valide e soddisfacibili

## Correttezza e completezza

## Tableau proposizionali

### Foglie chiuse

### Validità 

### Metodo dei Tableau