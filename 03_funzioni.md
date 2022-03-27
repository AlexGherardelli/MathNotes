# Funzioni
Una funzione può essere vista come qualcosa che "invia" elementi da un set $A$ a un set $B$ - quindi può essere vista come una relazione speciale tra insiemi. s

> **DEFINIZIONE**: 
> Una funzione $f$ da un insieme $D$ (dominio) ad un insieme $C$ (codominio) ($f : D \to C$)
> è una relazione $R \subseteq D \times C$ tale che per ogni elemento $a \in D$, esiste uno e un solo $b \in D$ tale che $a \mathrel{R} C$
> quindi:
>>  1. ogni elemento di D ha un corrispondente in C
>> 2. nessun elemento di D ha più di un corrispondente in C 

Può succedere che più elementi del dominio siano associati allo stesso elemento del codominio (e.g. funzione costante) e si possono avere valori nel codomino a cui nessun elemento del dominio è associato (cioè, immagine e codominio possono o no coincidere).
Non ci possono essere però elementi del dominio associati a più elementi del codominio, o elementi del dominio che non sono associati a nessun elemento del codominio.

> **DEFINIZIONE**
> **Dominio**  $D$: tutti i possibili "valori di input" della funzione
**Codominio**  $C$: l'insieme in cui sono contenute le immagini della funzione (insieme di arrivo)
**Immagine** $Im$: l'insieme delle $b$ tali che $f(a) = b$ per qualche $a$, ovvero l'insieme dei valori assunti da una funzione sul proprio dominio. $Im \subseteq C$, cioè un sottoinsieme del codominio (con cui può coincidere). 
>> ovvero: se $X \subseteq B$, $f(X) = \{ x \in X: f(x) \in X\} \subseteq B$ 
>
> **Controimmagine**: è l'insieme di tutti gli elementi del dominio $D$; ogni elemento deve avere una relazione con il codomino $C$.
>> ovvero: se $Y \subseteq B$, $f^{-1}(Y) = \{ x \in A: f(x) \in Y\} \subseteq A$ 

# Proprietà delle funzioni
## Funzione inettiva
> **DEFINIZIONE**: 
> Una funzione si die ineittiva se per ogni coppia di elementi del dominio corrisponde una coppia di elmeenti del codominio
> ovvero data $f: A \to B$
>>  $\quad\forall a, a' \in A: ( f(a) = f(a') )\implies a = a'$

## Funzione suriettiva
> **DEFINIZIONE**: 
> Una funzione si dice suriettiva, se ogni elemento del codominio ha corrisposta almeno una controimmagine nel dominio
> ovvero data $f: A \to B,$
>>$\forall b \in B: \exist a \in A \implies f(a) = b$


## Funzione biiettiva (o biunivoca)
> **DEFINIZIONE**:
> Una funzione si dice biiettiva se è sia iniettiva che suriettiva 

Una funzione biiettiva si dice anche biuniovoca (one-to one): in una funzione biiettiva $f: A \to B$, A e B sono **equipotenti**, cioè tra i due insiemi vi è una **relazione di equivalenza**.

# Composizione e inversione delle funzioni

## Funzione composta

## Funzione parziale

## Funzione identità 

## Funzione inversa
Una funzione è invertibile se e solo se è biiettiva. Infatti, invertendo una funzione non-iniettiva o non-suriettiva si ottiene una relazione che non è una funzione. 

L'inversione di funzione si denota con $f^{-1}: f(a) = a$. 