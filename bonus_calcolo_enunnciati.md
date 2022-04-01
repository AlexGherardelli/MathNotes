# Enunnciati (o proposizioni)

L'affermazione: *tutti i numeri naturali maggiori di due sono somme di due numeri primi" è un enunciato?
Sì, certo, è la **congettura di Goldbach**. Che nessuno ha mai dimostrato essere vera o falsa (anche se è verificata per numeri fino a $4*10^18), ma è sicuramente o vera o falsa.

Enunciati formati da una sola affermazione (e.g. "la neve è bianca") sono *enunciati atomici*, se prevedono connettivi logici (AND, OR, NOT), allora si dicono *enunciati composti*.

Tenendo conto che i connettivi logici sono, in fondo, operazioni sugli enunciati, i connettivi saranno definiti mediante le *tavole di verità*.

## Tavole di verità
| $P$    | $Q$    | $P \land Q$ | $P \lor Q$ | $\lnot P$ |
|--------|--------|-------------|------------|-----------|
| $\top$ | $\top$ | $\top$      | $\top$     | $\top$    |
| $\top$ | $\bot$  | $\bot$      | $\top$     | $\bot$    |
| $\bot$ | $\top$ | $\bot$      | $\top$     | $\top$    |
| $\bot$ | $\bot$ | $\bot$      | $\bot$     | $\top$    |