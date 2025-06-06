---
title: Algebra
draft: false
tags:
  - matematica
  - triennale
---
# Teoria degli Insiemi

In questa sezione vediamo richiami sulla teoria degli insiemi, con un focus su insiemi, corrispondenze, relazioni, relazioni di equivalenza e applicazioni con esempi ed esercizi.

## Definizione di Insieme

Un "insieme" è una nozione _primitiva_, che possiamo descrivere come una _collezione di elementi_. Sono insiemi $\{ 0,1 \}$, $\{ \text{rosso, nero} \}$, $\{ 0,1,2,3,\dots \} = \mathbb{N}$. L'insieme vuoto $\emptyset$ è l'unico insieme privo di elementi.

Abbiamo due modi di descrivere un insieme I:

1. Caratterizzazione dei suoi elementi:
   $$
     \begin{align*}
       & \\
	   & I = \{ 0,1 \} \\
	   & \mathbb{N} = \{ 1,2,3,\dots \} \\
	   & \\
     \end{align*}
	$$

2. Caratterizzazione come sottoinsieme di un **Insieme Universo** $U$ attraverso una o più proprietà: 
   $$
     \begin{align*}
       & \\
       & U = \mathbb{N} \\
       & I = \{ x \in U : x \text{ è pari} \} \\
     \end{align*}
   $$


Possiamo quindi dare una semplice definizione di insieme:

> [!INFO] Definizione di Insieme
> Un insieme è una collezione di oggetti, detti _elementi_. Un insieme può essere definito in modo esplicito elencando i suoi elementi, oppure tramite una o più proprietà che caratterizzi gli elementi dell'insieme universo. Si indica l'appartenenza di un elemento $x$ ad un insieme $A$ scrivendo $x \in A$.

## Comparabilità

Gli insiemi possono essere comparati tra loro. Ad esempio, possiamo indicare se un insieme è "incluso" in un altro: dati due insiemi $X$ e $Y$, con $X \subset Y$ stiamo indicando che $\forall x \in X \text{ allora } x \in Y$. Al contrario, con $X \not \subset Y$ stiamo indicando che $\exists x \in X : X \not \in Y$.

> [!INFO] Definizione di un sottoinsieme
> Un insieme $X$ è detto **sottoinsieme** di un insieme $Y$ quando tutti gli elementi di $X$ sono contenuti in $Y$.
> 
> $$
> \begin{align*}
>   & X \subset Y \implies \forall x \in X \text{ allora } x \in Y \\
>   & X \not \subset Y \implies \exists x \in X : x \not \in Y \\
> \end{align*}
> $$
> 
> Quando due insiemi sono sottoinsiemi l'uno dell'altro, allora gli insiemi sono uguali
> 
> $$
> X = Y \iff X \subset Y \lor Y \subset X
> $$
> 
> Due insiemi si dicono **comparabili** quando $X \subset Y \land Y \subset X$ (ossia $X \cap Y \not= \emptyset$)
> 
> > [!warning]- Osservazione:
> > 
> > Non è vero che presi qualunque due sottoinsiemi dell'insieme universo $U$ essi siano comparabili. 
> > 
> > Ad esempio, preso l'insieme universo $U = \{ 1,2,3 \} \in \mathbb{N}$, gli insiemi $X = \{ 1 \}$ e $Y = \{ 2,3 \}$ non sono comparabili, poiché $X \cap Y = \emptyset$. Questi due insiemi di dicono _disgiunti_, poiché la loro intersezione è l'insieme vuoto.
> > 
> > È possibile anche avere due insiemi non disgiunti, come $X = \{ 1,2 \}$ e $Y=\{ 1,3 \}$ che non sono comparabili tra loro.
## Insiemi Fondamentali

Esistono degli insiemi standard di particolare importanza:

| **Insieme** | **Descrizione** | Esempi                                                      |
| ----------- | --------------- | ----------------------------------------------------------- |
| ℕ           | Naturali        | $0,1,2,3,4,\dots$                                           |
| ℤ           | Relativi        | $-2,-1,0,1,2,\dots$                                         |
| ℚ           | Razionali       | $-\frac{1}{2},\frac{1}{2},\frac{2}{3},\frac{12}{322},\dots$ |
| ℝ           | Reali           | $\sqrt{ 2 }, -\sqrt{ 5 }, \dots$                            |
| ℂ           | Complessi       | $i, \sqrt{ -1 }, \dots$                                     |
Leggendo dalla prima all'ultima riga, ogni insieme si costruisce dal precedente attraverso una procedura specifica. Non sempre questo è facile, come ad esempio per costruire $\mathbb{R}$ a partire da $\mathbb{Q}$.

### Operazioni sugli insiemi

Nelle seguenti definizioni, tutti gli insiemi che vengono citati sono da considerarsi come sottoinsiemi del medesimo insieme universo.

> [!INFO] Definizione: Intersezione
> Si dice **intersezione** di due insiemi $X$ e $Y$ l'insieme formato da tutti quegli elementi che appartengono sia ad $X$ che ad $Y$:
> 
> $$ X \cap Y = \{ x \in U : x \in X \land x \in Y\} $$

> [!INFO] Definizione: Unione
> Si dice **unione** di due insiemi $X$ e $Y$ l'insieme formato da tutti quegli elementi che appartengono ad $X$ o ad $Y$:
> 
> $$ X \cup Y = \{ x \in U : x \in X \lor x \in Y \} $$

> [!INFO] Definizione: Complementare
> 
> Si dice **complementare** di un insieme $X$ l'insieme formato da tutti quegli elementi che appartengono all'insieme universo $U$ che non sono in $X$:
> 
> $$ \complement X =  \{x \in U : x \not\in X\} $$

> [!INFO] Definizione: Differenza
> 
> Si dice **differenza** di due insiemi $X$ e $Y$ l'insieme formato da tutti quegli elementi che appartengono ad $X$ e non appartengono ad $Y$:
> 
> $$ X \setminus Y = \{ x \in X : x \not \in Y \} $$

## Diagrammi di Venn
Questa sezione è omessa in quanto di facile intuizione e precedentemente trattata in modo esaustivo in altri corsi.

## Prodotto Cartesiano

> [!INFO] Definizione: Prodotto Cartesiano
> 
> Siano $X$ e $Y$ due insiemi non vuoti. Si definisce il **prodotto cartesiano** $X \times Y$ l'insieme
> 
> $$
> X \times Y = \{ (x,y) : x \in X \land y \in Y \}
> $$
> 
> ovvero l'insieme di tutte le coppie ordinate in cui il primo elemento appartiene ad $X$ ed il secondo elemento ad $Y$
> 
> > [!warning]- Osservazione:
> > 
> > Da non confondere nella notazione l'utilizzo delle parentesi graffe e delle parentesi tonde, in quanto le prime non tengono conto dell'ordine mentre le seconde sì

### Definizione rigorosa delle coppie ordinate (Kuratowski)

Nella teoria degli insiemi possiamo fornire una definizione rigorosa delle coppie ordinate e delle triple ordinate, questo al fine di distinguere chiaramente la differenza tra $(x,y)$ e $(y,x)$ ad esempio. Per una coppia ordinata $(x,y)$, essa è definita come:

$$
(x,y) = \{ \{ x \}, \{ x,y \} \}
$$
Questa definizione garantisce che le coppie ordinate siano distinguibili dalle singole componenti. Analogamente, per una tripla ordinata $(x,y,z)$, possiamo estendere la definizione nel seguente modo:
$$
  \begin{align*}
    & \text{1. }(x,y,z) \\
    & \text{2. }(x,(y,z)) \\
    & \text{3. }\{ x, \{ x, (y,z) \} \} \text{ e sappiamo che } (y,z) = \{ y, \{ y, z \} \} \\
    & \text{4. } \{ \{ x \}, \{ x, \{\{ y \}, \{ y,z \} \}\} \}
  \end{align*}
$$
Questa rappresentazione rigorosa si generalizza a tuple di ordine superiore.

## Corrispondenze

> [!info] Definizione: Corrispondenze
> 
> Siano $X$ e $Y$ due insiemi non vuoti. Una **corrispondenza** tra $X$ e $Y$ è una terna $(X,Y,\Gamma)$ dove:
> $$
> \Gamma \subset X \times Y
> $$
> è un sottoinsieme non vuoto del prodotto cartesiano $X \times Y$, chiamato _grafo_ della corrispondenza, $X$ è detto _dominio_ e $Y$ è detto _codominio_

## Relazioni

Una **relazione** è una corrispondenza $(X,Y,\Gamma)$ in cui il dominio e il codominio coincidono, ovvero $X=Y$. In tal caso, la relazione si rappresenta semplicemente come $(X, \Gamma)$ dove $\Gamma \subset X \times X$ è il grafo della relazione.

> [!info] Definizione: Relazione
> 
> Data una relazione $\mathrel{\mathcal{R}} = (X, \Gamma)$ per $x,y$ si dice che $x$ e $y$ sono in **relazione** $\mathrel{\mathcal{R}}$ se e solo se la coppia $(x,y)$ appartiene al grafo $\Gamma$, cioè:
> $$
> x \mathrel{\mathcal{R}} y \iff (x,y) \in \Gamma
> $$

### Proprietà delle relazioni

Quattro proprietà fondamentali delle relazioni sono:

> [!info] Definizione: Proprietà riflessiva
> 
> Una relazione $\mathrel{\mathcal{R}}$ su X si dice **riflessiva** se $\forall x \in X, x \mathrel{\mathcal{R}} x$, ovvero:
> $$
> \forall x \in X, (x,x) \in \Gamma
> $$

> [!info] Definizione: Proprietà simmetrica
> 
> Una relazione $\mathrel{\mathcal{R}}$ su $X$ è detta **simmetrica** se $\forall x,y \in X, x \mathrel{\mathcal{R}} y \implies y \mathrel{\mathcal{R}} x$, ovvero:
> $$
> (x,y) \in \Gamma \implies (y,x) \in \Gamma
> $$

> [!info] Definizione: Proprietà transitiva
> 
> Una relazione $\mathrel{\mathcal{R}}$ su $X$ è detta **transitiva** se $\forall x,y,z \in X$ se $x \mathrel{\mathcal{R}} y$ e $y \mathrel{\mathcal{R}} z$, allora $x \mathrel{\mathcal{R}} z$, ovvero:
> $$
> (x,y) \in \Gamma \land (y,z) \in \Gamma \implies (x,z) \in \Gamma
> $$

> [!info] Definizione: Proprietà antisimmetrica
> 
> Una relazione $\mathrel{\mathcal{R}}$ su $X$ è detta **antisimmetrica** se $\forall x,y \in X$ se $x \mathrel{\mathcal{R}} y$ e $y \mathrel{\mathcal{R}} x$ allora $x=y$, ovvero:
> $$
> (x,y) \in \Gamma \land (y,x) \in \Gamma \implies x = y
> $$

### Relazioni d'equivalenza

Una relazione che soddisfa le proprietà di riflessività, simmetria e transitività è chiamata **relazione d'equivalenza**.

> [!info] Defininzione: Relazione d'equivalenza
> 
> Una relazione $\mathrel{\mathcal{R}} = (X,\Gamma)$ si dice **relazione d'equivalenza** se soddisfa le proprietà di riflessività, simmetria e transitività.
> 

### Classi d'equivalenza

Sia $\mathrel{\mathcal{R}} = (X, \Gamma)$ una relazione di equivalenza. Con $x \in X$ poniamo $\mathrm{Cl}(x) = \{ y \in X : x \mathrel{\mathcal{R}} y \} \subset X$. Notiamo che $\mathrm{Cl}(x) \not = \emptyset$, in quanto essendo $\mathrel{\mathcal{R}}$ una relazione d'equivalenza vale la proprietà riflessiva, ossia $x \mathrel{\mathcal{R}} x$.

> [!INFO] Classi di equivalenza
> 
> Data una relazione di equivalenza $\mathcal{R}$ su un insieme $X$, la **classe di equivalenza** di un elemento $x \in X$ è l'insieme di tutti gli elementi di $X$ che sono in relazione con $x$ secondo $\mathcal{R}$. Si denota con $[x]$ e si definisce come:
> 
> $$
>   [x] = \{ y \in X \mid x \mathrel{\mathcal{R}} y \}
> $$
> 
> 
> > [!tip]- Spiegazione
> > 
> > In altre parole, la classe di equivalenza $[x]$ è l'insieme di tutti gli elementi che sono **equivalenti** a $x$ rispetto alla relazione $\mathcal{R}$. Ogni classe di equivalenza contiene elementi che, secondo $\mathcal{R}$, sono indistinguibili o condividono una certa proprietà comune definita dalla relazione.
> > 
> > **Esempio**:
> > 
> > Se consideriamo l'insieme dei numeri interi $\mathbb{Z}$ e la relazione di equivalenza "congruo modulo $n$", allora la classe di equivalenza di un intero $a$ è:
> > 
> >  $$
> >   [a] = \{ b \in \mathbb{Z} \mid b \equiv a \ (\mathrm{mod}\ n) \}
> > $$
> > 
> > Questa classe contiene tutti i numeri interi che hanno lo stesso resto di $a$ quando divisi per $n$.

Possiamo indicare le classi di equivalenza con diverse notazioni:

$$
\bar{x},\, \bar{x}_{\mathrel{\mathcal{R}}},\, [x],\, [x]_{\mathrel{\mathcal{R}}}, \,\mathrm{Cl}_{\mathrel{\mathcal{R}}}(x),\, \dots
$$

e notiamo che c'è sempre dipendenza da un _rappresentante_ $x$ della classe.

> [!abstract] Proposizione 1
> 
> Data $\mathrel{\mathcal{R}} = (X, \Gamma)$ relazione d'equivalenza abbiamo che:
> $$
>     \begin{align*}
>          & \text{1. Dati } x,y \in X, \text{ allora } \mathrm{Cl}(x) = \mathrm{Cl}(y) \iff x \mathrel{\mathcal{R}} y \\
>         & \\
>         & \text{2. } \forall x,y \in X \text{ allora } \begin{cases}
>         \text{o } \mathrm{Cl}(x) = \mathrm{Cl}(y) \\
>         \text{oppure } \mathrm{Cl}(x) \cap \mathrm{Cl}(y) = \emptyset
>         \end{cases} \\
>     \end{align*}
> $$
>
> In particolare, data una classe d'equivalenza $\mathrm{C}$, allora $\forall x \in \mathrm{C}$, $\mathrm{C} = \mathrm{Cl}(x)$; ogni elemento è rappresentante della classe cui appartiene. Inoltre, le classi di equivalenza sono **disgiunte**, ossia ogni elemento di $X$ appartiene a una sola classe.
> 
> > [!warning]+ Osservazione
> > In sintesi, possiamo considerare le classi di equivalenza come gli insiemi di elementi che la relazione non è in grado di distinguere tra loro.

> [!tip]- Dimostrazione del punto 1
> 
> **Enunciato:** Per ogni $x,y \in X$, si ha $\mathrm{Cl}(x) = \mathrm{Cl}(y) \iff x \mathrel{\mathcal{R}} y$.
> 
> **Dimostrazione:**
> 
> ($\Rightarrow$) Supponiamo che $\mathrm{Cl}(x) = \mathrm{Cl}(y)$.
> - **Obiettivo:** Dimostrare che $x \mathrel{\mathcal{R}} y$.
> - Poiché la relazione $\mathrel{\mathcal{R}}$ è riflessiva, abbiamo $y \mathrel{\mathcal{R}} y$, quindi $y \in \mathrm{Cl}(y)$.
> - Dato che $\mathrm{Cl}(x) = \mathrm{Cl}(y)$, segue che $y \in \mathrm{Cl}(x)$.
> - Per definizione di classe di equivalenza:
>   
>  $$
>    y \in \mathrm{Cl} (x) \implies x \mathrel{\mathcal{R}} y
> $$
> - **Conclusione:** $x \mathrel{\mathcal{R}} y$
>
>---
>
> ($\Leftarrow$) Supponiamo che $x \mathrel{\mathcal{R}} y$.
> - **Obiettivo:** Dimostrare che $\mathrm{Cl}(x) = \mathrm{Cl}(y)$.
> - Dimostriamo l'uguaglianza mostrando che ogni elemento di $\mathrm{Cl}(x)$ appartiene a $\mathrm{Cl}(y)$ e viceversa.
>   
> **Passo 1: Dimostriamo che** $\mathrm{Cl}(x) \subseteq \mathrm{Cl}(y)$.
> - Sia $z \in \mathrm{Cl}(x)$. Per definizione, $x \mathrel{\mathcal{R}} z$.
> - Sappiamo che $x \mathrel{\mathcal{R}} y$ (ipotesi) e $x \mathrel{\mathcal{R}} z$.
> - Poiché $\mathrel{\mathcal{R}}$ è simmetrica, da $x \mathrel{\mathcal{R}} z$ segue $z \mathrel{\mathcal{R}} x$.
> - Poiché $\mathrel{\mathcal{R}}$ è transitiva, da $y \mathrel{\mathcal{R}} x$ e $x \mathrel{\mathcal{R}} z$, segue $y \mathrel{\mathcal{R}} z$.
> - Quindi, $z \in \mathrm{Cl}(y)$.
> - **Conclusione:** $\mathrm{Cl}(x) \subseteq \mathrm{Cl}(y)$
> 
> **Passo 2: Dimostriamo che** $\mathrm{Cl}(y) \subseteq \mathrm{Cl}(x)$.
> - Sia $w \in \mathrm{Cl}(y)$. Per definizione, $y \mathrel{\mathcal{R}} w$.
> - Sappiamo che $x \mathrel{\mathcal{R}} y$ e $y \mathrel{\mathcal{R}} w$.
> - Poiché $\mathrel{\mathcal{R}}$ è transitiva, da $x \mathrel{\mathcal{R}} y$ e $y \mathrel{\mathcal{R}} w$ segue $x \mathrel{\mathcal{R}} w$.
> - Quindi $w \in \mathrm{Cl}(x)$.
> - **Conclusione:** $\mathrm{Cl}(y) \subseteq \mathrm{Cl}(x)$.
>   
> **Conclusione finale:**
> - Dalle inclusioni reciproche, abbiamo $\mathrm{Cl}(x) = \mathrm{Cl}(y)$.

> [!tip]- Dimostrazione del punto 2
> 
> **Enunciato:** Per ogni $x,y \in X$ si ha che:
> - o $\mathrm{Cl}(x) = \mathrm{Cl}(y)$
> - oppure $\mathrm{Cl}(x) \cap \mathrm{CL}(y) = \emptyset$
>   
> **Dimostrazione**
> - Sia $x,y \in X$.
> - **Caso 1:** Se $\mathrm{Cl}(x) \subseteq \mathrm{Cl}(y) = \emptyset$ non c'è nulla da dimostrare.
> - **Caso 2:** Supponiamo che $\mathrm{Cl}(x) \cap \mathrm{Cl}(y) \not = \emptyset$.
> 	- Allora esiste almeno un elemento $z \in X : z \in \mathrm{CL}(x) \land z \in \mathrm{Cl}(y)$.
> 	- Per definizione di classe di equivalenza:
> 		- $z \in \mathrm{Cl}(x) \implies x \mathrel{\mathcal{R}} z$.
> 		- $z \in \mathrm{Cl}(y) \implies y \mathrel{\mathcal{R}} z$.
> 	- Poiché $\mathrel{\mathcal{R}}$ è simmetrica, da $y \mathrel{\mathcal{R}} z$ segue $z \mathrel{\mathcal{R}} y$.
> 	- Poiché $\mathrel{\mathcal{R}}$ è transitiva, da $x \mathrel{\mathcal{R}} z$ e $z \mathrel{\mathcal{R}} y$, segue $x \mathrel{\mathcal{R}} y$.
> 	- **Dal punto 1**, sappiamo che se $x \mathrel{\mathcal{R}} y$, allora $\mathrm{Cl}(x) = \mathrm{Cl}(y)$.
> - **Conclusione:** Se $\mathrm{Cl}(x) \cap \mathrm{Cl}(y) \not = \emptyset$, allora $\mathrm{Cl}(x) = \mathrm{Cl}(y)$.

## Insieme delle parti (Power Set)

> [!info] Definizione di Insieme delle parti
> 
> Dato un insieme $X \not = \emptyset$, si definisce l'**insieme delle parti** di $X$, denotato con $\mathcal{P}(X)$, l'insieme di tutti i sottoinsiemi di $X$. Formalmente:
> 
> $$
>  \mathcal{P}(X) = \{ P : P \subseteq X \}
> $$
> 
> **N.B.** l'insieme delle parti contiene anche l'insieme vuoto, ovvero $\emptyset \in \mathcal{P}$
## Partizioni di un Insieme

> [!info] Definizione di partizione
> 
> Sia $\mathcal{P}$ un insieme di sottoinsiemi **non vuoti** (quindi $\emptyset \not\in \mathcal{P}$) di $X$, cioè $\mathcal{P} \subseteq \mathcal{P}(X) \text{ e } \mathcal{P} \not = \emptyset$.
> 
> Si dice che $\mathcal{P}$ è una **partizione** di $X$ se soddisfa le seguenti condizioni:
> 
> 1. **Non vacuità dei blocchi:**
>     $$
>         \forall P \in \mathcal{P},\, P \not = \emptyset
>     $$
>     Ogni insieme della partizione non è vuoto.
> ---
> 2. **Disgiunzione dei blocchi:**
>     $$
>         \forall P,Q \in \mathcal{P},\, P \not = Q \implies P \cap Q = \emptyset
>     $$
>     Due insiemi distinti della partizione sono disgiunti.
> ---
> 3. **Copertura dell'insieme originale:**
>     $$
>         \bigcup_{P \in \mathcal{P}}P = X
>     $$
>     L'unione di tutti gli insiemi della partizione è l'insieme X. In altre parole:
>     $$
>         \forall x \in X,\, \exists! P \in \mathcal{P} : x \in P
>     $$

In sintesi, una partizione di $X$ è un insieme di sottoinsiemi non vuoti, a due a due disgiunti, la cui unione è l'intero insieme $X$ (_de facto la partizione rappresenta un "modo" di suddividere tutto l'insieme $X$_).

> [!abstract] Proposizione 2
> 
> **Enunciato:**
> 
> Sia $\mathrel{\mathcal{R}} = (X, \Gamma)$ una relazione d'equivalenza su un insieme $X$. Allora l'insieme delle classi di equivalenza di $\mathrel{\mathcal{R}}$:
> 
> $$
>    \mathcal{P} = \{ \mathrm{Cl}(x) : x \in X \} 
> $$
> 
> è una **partizione** di $X$.

> [!tip]- Dimostrazione
> 
> Vogliamo dimostrare che l'insieme delle classi di equivalenza $\mathcal{P} = \{  \mathrm{Cl}(x) : x \in X \}$ forma una partizione di $X$ soddisfacendo le tre condizioni sopra elencate.
> 
> 1. **Ogni classe di equivalenza è non vuota**:
>    - Per ogni $x \in X$
>      - La classe di equivalenza di $x$ è definita come:
>       $$
>         \mathrm{Cl}(x) = \{  y \in X : x \mathrel{\mathcal{R}} y \}
>      $$
>      - Poiché $\mathrel{\mathcal{R}}$ è riflessiva, abbiamo che $x \mathrel{\mathcal{R}} x$
> 	 - Quindi, $x \in \mathrm{Cl}(x)$
> 	 - **Conclusione:** $\mathrm{Cl}(x) \not = \emptyset$
> 2. **Le classi di equivalenza distinte sono disgiunte**
>    - Supponiamo che esistano $x,y \in X : \mathrm{Cl}(x) \not = \mathrm{Cl}(y)$
>    - Supponiamo per assurdo che $\mathrm{Cl}(x) \cap \mathrm{Cl}(y) \not = \emptyset$
>      - Allora esiste un elemento $z \in X : z \in \mathrm{Cl}(x)\text{ e }z \in \mathrm{Cl}(y)$.
>      - Ciò implica:
>        - $x \mathrel{\mathcal{R}} z$ (perché $z \in \mathrm{Cl}(x)$)
>        - $y \mathrel{\mathcal{R}} z$ (perché $z \in \mathrm{Cl}(y)$)
> 	 - Poiché $\mathrel{\mathcal{R}}$ è simmetrica:
> 	   - Da $y \mathrel{\mathcal{R}} z$, otteniamo $z \mathrel{\mathcal{R}} y$
> 	 - Poiché $\mathrel{\mathcal{R}}$ è transitiva:
> 	   - Da $x \mathrel{\mathcal{R}} z\text{ e }z \mathrel{\mathcal{R}} y$, otteniamo $x \mathrel{\mathcal{R}} y$.
> 	 - Secondo la Proposizione 1, se $x \mathrel{\mathcal{R}} y$, allora $\mathrm{Cl}(x) = \mathrm{Cl}(y)$.
> 	 - **Contraddizione!** Avevamo supposto che $\mathrm{Cl}(x) \not = \mathrm{Cl}(y)$
>    - **Conclusione:** Le classi di equivalenza distinte sono disgiunte, cioè:
>     $$
>     \mathrm{Cl}(x) \cap \mathrm{Cl}(y) = \emptyset \text{ se } \mathrm{Cl}(x) \not = \mathrm{Cl}(y)
>     $$
> 3. **L'unione di tutte le classi di equivalenza è $X$**:
>    - Per ogni $x \in X$:
>      - Abbiamo già stabilito che $x \in \mathrm{Cl}(x)$
>    - Quindi:
>      - Ogni elemento di £X£ appartiene ad almeno una classe di equivalenza in $\mathcal{P}$
>    - **Conclusione:**
>       $$
>         X = \bigcup_{x \in X} \mathrm{Cl}(x) = \bigcup_{P\in \mathcal{P}}P
>      $$
>      
> **Conclusione della dimostrazione:**
> 
> Poiché l'insieme $\mathcal{P}$ delle classi di equivalenza soddisfa le tre condizioni:
> 1. Ogni $\mathrm{Cl}(x)$ è non vuoto;
> 2. Le classi distinte sono disgiunte;
> 3. L'unione delle classi copre tutto $X$;
>    
> Possiamo concludere che $\mathcal{P}$ è una **partizione** di $X$
## Insieme quoziente

> [!info] Definizione di insieme quoziente
> 
> Dato un insieme $X$ e una relazione di equivalenza $\mathcal{R}$ su $X$, si definisce l'**insieme quoziente** di $X$ rispetto ad $\mathcal{R}$ come l'insieme delle classi di equivalenza di $X$ indotte da $\mathcal{R}$.
> 
> L'insieme quoziente è denotato con:
> 
> $$
>     X \big/ \mathcal{R} \text{ oppure } \frac{X}{\mathcal{R}}
> $$
> 
> e si definisce come:
> 
> $$
>     X \big/ \mathcal{R} = \{ \mathrm{Cl}(x) : x \in X \}
> $$
> 
> dove $\mathrm{Cl}(x)$ è la classe di equivalenza di $x$ rispetto ad $\mathcal{R}$.

## Sistema Completo di Rappresentanti

> [!info] Definizione di SCR
> 
> Dato un insieme $X$ e una relazione di equivalenza $\mathcal{R}$ su $X$, un **Sistema Completo di Rappresentanti** (SCR) per $\mathcal{R}$ è un sottoinsieme $X' \subseteq X$ tale che:
> 
> 1. **Rappresentanza Unica delle Classi:**
>    - Ogni classe di equivalenza contiene esattamente un elemento di $X'$;
>    - Formalmente:
>      
>       $$
>         \forall x \in X,\, \exists! x'\in X' : x \in \mathrm{Cl}(x')
>      $$
>      
>      Dove $\mathrm{Cl}(x')$ è la classe di equivalenza di $x'$.
>      
> 2. **Classi di Equivalenza Distinte**:
>    - Gli elementi di $X'$ non appartengono a classi di equivalenza distinte.
>    - Cioè, per ogni $x_{1}', x_{2}' \in X' \text{ con } x_{1}' \not = x_{2}'$, le loro classi di equivalenza non si sovrappongono:
>       $$
>         x_{1}' \not = x_{2}' \implies \mathrm{Cl}(x_{1}') \cap \mathrm{Cl(x_{2}')} = \emptyset
>      $$
>  In altre parole, $X'$ contiene esattamente un elemento per ogni classe di equivalenza di $\mathcal{R}$.

> [!example]- Esempio di SCR
> 
> $X = \{ \text{r retta di } \mathbb{R}^2 \}$
> $\mathcal{R} = ||$ _(parallelismo, è una relazione di equivalenza)_
> 
> Allora possiamo dire $X' = \{ \text{rette per l'origine} \}$ è un sistema completo di rappresenti su $\mathcal{R} = ||$.
> 
> La prima condizione è verificata, in quanto due rette per l'origine distinte non sono parallele; per la seconda invece, abbiamo che $\forall r \in X,\,\exists! r' \in X' : r\, ||\, r'$

> [!warning]- Osservazioni:
> 
> - **Non Unicità del Sistema Completo di Rappresentanti:**
>   In generale, non esiste unicità per un **Sistema Completo di Rappresentanti** (SCR). Questo significa che, data una relazione di equivalenza su un insieme $X$, è possibile costruire diversi SCR, ciascuno dei quali soddisfa le condizioni per essere un sistema completo, ma che differiscono tra loro per la scelta dei rappresentanti delle classi di equivalenza.
> - **Esempio: Fascio di Rette Passanti per un Punto $P$ nel Piano**
>   Ad esempio, consideriamo il piano cartesiano $\mathbb{R}^2$ e fissiamo un punto $P \in \mathbb{R}^2$. Il **fascio di rette passanti per** $P$, denotato con $\mathscr{X}_{P}$​, può essere considerato un sistema completo di rappresentanti rispetto alla relazione di equivalenza che associa tra loro tutte le rette parallele.
> - **Assenza di Canonicità nella Scelta del Sistema Completo di Rappresentanti**
>   Non esiste, in generale, una scelta "canonica" o naturale per il sistema completo di rappresentanti. Questo significa che non c'è un modo univoco e preferibile di scegliere i rappresentanti delle classi di equivalenza; la scelta dipende spesso dal contesto o dall'applicazione specifica.

# Applicazioni (Funzioni)

> [!info] Definizione di Applicazione
> 
> Un'applicazione (o funzione) è una corrispondenza $f = (X,Y,\Gamma)$, dove ad ogni elemento $a \in X$ corrisponde esattamente uno e un solo elemento $b \in Y$, cioè:
>   
>   $$
>    \forall a \in X,\, \exists! b \in Y : (a,b) \in \Gamma
>  $$
>  
>  Qui, $X$ è detto **dominio**, $Y$ è detto **codominio** (o insieme immagine), e $\Gamma$ è il **grafo** dell'applicazione.
>  L'elemento $b$ si indica come **immagine** di $a$ attraverso $f$, e si scrive:
>  
>  $$
>   b = f(a) \,\,\, \text{(si legge "f di a")}
> $$
> 
> Un'applicazione si rappresenta spesso come $X \xrightarrow{f} Y$

**Esempio:**

Dominio: $X = \{1,2,3\}$
Codominio: $Y=\{x,y\}$
Grafo: $\Gamma = \{(1,x),(2,y),(3,y)\}$

Utilizzando i Diagrammi di Venn:

![[img1.png]]

**N.B: La corrispondenza non è sempre una funzione!**
## Funzioni inverse

> [!info] Definizione di Funzione Inversa
> 
> Sia $f : X \rightarrow Y$ un'applicazione. L'**immagine inversa** di un sottoinsieme $Y' \subset Y$ tramite $f$, indicata con $f^{-1}(Y')$, è definita come:
> 
> $$
>   f^{-1}(Y') = \{ x \in X :  f(x) \in Y' \}
> $$
> 
> > [!warning]- Osservazioni
> > 1. $f^{-1}(Y')$ è un **sottoinsieme** di $X$.
> > 2. Se $y \in Y$, $f^{-1}(\{ y \})$ rappresenta l'insieme degli **antecedenti di** $y$ (tutti gli $x \in X$ tali che $f(x) = y$)
> 
> > [!tip]- AI-splaining
> > Cerchiamo di capire a fondo la definizione di Funzione Inversa, o meglio, l'immagine inversa di un sottoinsieme. La definizione che hai fornito riguarda un concetto fondamentale quando si lavora con le funzioni e le loro proprietà.
> >
> > Iniziamo col dire che la definizione parla di un'applicazione $f : X \rightarrow Y$. Questo significa che $f$ è una funzione che prende elementi da un insieme $X$ (il dominio) e li associa a elementi di un insieme $Y$ (il codominio).  È importante tenere a mente questa distinzione tra dominio e codominio, perché l'immagine inversa è definita in relazione a questi insiemi.
> >
> > L'immagine inversa, indicata con $f^{-1}(Y')$, è un'operazione che prende un sottoinsieme $Y' \subset Y$ (cioè un insieme contenuto in $Y$) e lo "riporta indietro" al dominio $X$.  Non si tratta della funzione inversa nel senso stretto del termine (che esiste solo se $f$ è biunivoca), ma di un insieme di elementi di $X$ che soddisfano una certa condizione.
> >
> > La formula $$f^{-1}(Y') = \{ x \in X :  f(x) \in Y' \}$$ è la chiave per capire cosa significa.  Leggiamola attentamente: "L'immagine inversa di $Y'$ tramite $f$ è l'insieme di tutti gli elementi $x$ che appartengono a $X$ tali che $f(x)$ appartiene a $Y'$".
> >
> > In altre parole, prendiamo tutti gli elementi $x$ del dominio $X$.  Per ogni $x$, applichiamo la funzione $f$.  Se il risultato di $f(x)$ è un elemento che appartiene al sottoinsieme $Y'$, allora $x$ fa parte dell'immagine inversa $f^{-1}(Y')$.  Se $f(x)$ non appartiene a $Y'$, allora $x$ non fa parte di $f^{-1}(Y')$.
> >
> > L'osservazione numero 1 sottolinea che $f^{-1}(Y')$ è sempre un **sottoinsieme** di $X$. Questo è logico, perché stiamo prendendo elementi dal dominio $X$ e costruendo un nuovo insieme a partire da essi.  Non possiamo avere elementi in $f^{-1}(Y')$ che non appartengono a $X$.
> >
> > L'osservazione numero 2 è particolarmente utile.  Se consideriamo un singolo elemento $y$ nel codominio $Y$, allora $f^{-1}(\{ y \})$ rappresenta l'insieme di tutti gli **antecedenti di** $y$.  Cosa significa? Significa che stiamo cercando tutti gli elementi $x$ nel dominio $X$ tali che $f(x) = y$.  In altre parole, stiamo trovando tutti gli input $x$ che, quando vengono applicati alla funzione $f$, producono l'output $y$.  Questo insieme può essere vuoto (se non esiste alcun $x$ tale che $f(x) = y$), può contenere un solo elemento (se $f$ è iniettiva in quel punto), o può contenere più elementi (se $f$ non è iniettiva).
> >
> > Per riassumere, l'immagine inversa è un'operazione che prende un sottoinsieme del codominio e lo "riporta indietro" al dominio, trovando tutti gli elementi del dominio che vengono mappati in quel sottoinsieme.  È un concetto fondamentale per capire le proprietà delle funzioni e le loro relazioni con i loro insiemi di input e output.  Non confondere l'immagine inversa con la funzione inversa, che è un concetto diverso e richiede che la funzione sia biunivoca.

## Particolari tipi di applicazione

> [!info] Definizione di funzione iniettiva
> 
> Una funzione $X \xrightarrow{f} Y$ è detta **iniettiva** (o **iniettiva uno ad uno**) se: 
> 
> $$
>   x,x' \in X,\,f(x) = f(x'), \implies x = x'
> $$
> 
> In altre parole, due elementi distinti del dominio $X$ non possono avere la stessa immagine in $Y$.
> 
> **Caratterizzazione alternativa:**
> 
> Per ogni elemento $y \in Y$, l'immagine inversa di $y$ è:
> 
> $$
> f^{-1}(\{y\}) =
> \begin{cases}
> \emptyset, & \text{se } y \notin \text{Im}(f), \\
> \{x\}, & \text{se } y \in \text{Im}(f).
> \end{cases}
> $$
> 
> Ciò significa che ogni elemento del codominio $Y$ è immagine di **al massimo un elemento** del dominio $X$.
> > [!tip]- AI-splaining
> > Cominciamo con la definizione fondamentale: una funzione $f$ che mappa un insieme $X$ in un insieme $Y$ (scritto come $X \xrightarrow{f} Y$) è detta **iniettiva** (o **uno ad uno**) se soddisfa una specifica condizione. Questa condizione riguarda il comportamento della funzione quando applicata a elementi distinti del dominio $X$.
> > 
> > La condizione di iniettività è espressa matematicamente come:  $x,x' \in X,\,f(x) = f(x'), \implies x = x'$.  Cerchiamo di scomporla.  Significa che *se* prendiamo due elementi qualsiasi, chiamati $x$ e $x'$, appartenenti all'insieme di partenza $X$, e *se* il valore della funzione applicata a $x$ è uguale al valore della funzione applicata a $x'$ (cioè $f(x) = f(x')$), *allora* possiamo concludere che $x$ e $x'$ devono essere uguali ($x = x'$).
> > 
> > In parole più semplici, l'iniettività garantisce che elementi diversi nel dominio $X$ vengano sempre mappati in elementi diversi nel codominio $Y$.  Se due elementi distinti del dominio producono la stessa immagine, la funzione non è iniettiva.  È cruciale capire che l'iniettività non dice nulla su cosa succede agli elementi *uguali* nel dominio; semplicemente afferma che elementi *distinti* devono avere immagini distinte.
> > 
> > Ora passiamo alla **caratterizzazione alternativa** dell'iniettività. Questa caratterizzazione ci fornisce un modo diverso per verificare se una funzione è iniettiva, basato sull'immagine inversa. L'immagine inversa di un elemento $y$ appartenente al codominio $Y$, denotata come $f^{-1}(\{y\})$, è l'insieme di tutti gli elementi $x$ nel dominio $X$ tali che $f(x) = y$.
> > 
> > La caratterizzazione alternativa afferma che per ogni elemento $y$ in $Y$, l'immagine inversa di $y$ può avere solo due possibili valori: o è l'insieme vuoto ($\emptyset$), oppure è un insieme contenente un singolo elemento ($\{x\}$).  Se $y$ non appartiene all'immagine della funzione ($y \notin \text{Im}(f)$), allora non esiste alcun elemento $x$ nel dominio tale che $f(x) = y$, e quindi l'immagine inversa di $y$ è l'insieme vuoto.
> > 
> > Se invece $y$ appartiene all'immagine della funzione ($y \in \text{Im}(f)$), allora esiste almeno un elemento $x$ nel dominio tale che $f(x) = y$.  La caratterizzazione alternativa ci dice che, in questo caso, esiste *solo un* elemento $x$ tale che $f(x) = y$.  In altre parole, ogni elemento del codominio $Y$ è immagine di **al massimo un elemento** del dominio $X$.  Questo è un modo equivalente di esprimere l'iniettività. Se un elemento del codominio avesse più di un'immagine inversa, la funzione non sarebbe iniettiva.

> [!info] Definizione di funzione suriettiva
> 
> Una funzione $f: X \rightarrow Y$ è detta **suriettiva** (o sopraiettiva) se ogni elemento del codominio $Y$ è immagine di almeno un elemento del dominio $X$. Formalmente:
> 
> $$
>   f(X) = Y
> $$
> 
> ovvero:
> 
> $$
>   \forall y \in Y, \exists x \in X : f(x) = y
> $$
> 
> **Caratterizzazione alternativa:**
> Utilizzando l'immagine inversa, la funzione $f$ è suriettiva se:
> 
> $$
>   \forall y \in Y, f^{-1}(\{  y \}) \not = \emptyset
> $$
> 
> Questo significa che per ogni elemento del codominio $Y$, esiste almeno un elemento $x \in X$ tale che $f(x) = y$.
>
> > [!tip]- AI-splaining
> > Una funzione suriettiva, detta anche sopraiettiva, è un concetto fondamentale nella teoria degli insiemi e delle funzioni. Per comprenderla appieno, è necessario analizzare attentamente la sua definizione e le sue implicazioni. In sostanza, una funzione suriettiva "copre" completamente il suo codominio.
> >
> > La definizione formale di una funzione suriettiva $f: X \rightarrow Y$ afferma che $f(X) = Y$. Questo significa che l'insieme immagine di $X$ tramite la funzione $f$ (ovvero l'insieme di tutti i valori che $f$ assume quando applicata a tutti gli elementi di $X$) è uguale all'intero codominio $Y$. In altre parole, non ci sono elementi in $Y$ che non siano "raggiunti" dalla funzione $f$.
> >
> > Per chiarire ulteriormente, consideriamo un esempio. Supponiamo di avere una funzione $f$ che associa ogni studente di una classe (dominio $X$) al suo voto all'esame (codominio $Y$). Se la funzione è suriettiva, significa che ogni voto possibile (ad esempio, da 0 a 10) è effettivamente ottenuto da almeno uno studente della classe. Se, ad esempio, nessuno studente prendesse 10, la funzione non sarebbe suriettiva.
> >
> > La seconda parte della definizione formale, $\forall y \in Y, \exists x \in X : f(x) = y$, esprime la stessa idea in termini più precisi. Per ogni elemento $y$ nel codominio $Y$, deve esistere almeno un elemento $x$ nel dominio $X$ tale che $f(x) = y$. Questo garantisce che ogni elemento di $Y$ sia "colpito" dalla funzione $f$.
> >
> > La caratterizzazione alternativa utilizzando l'immagine inversa fornisce un modo diverso, ma equivalente, per verificare se una funzione è suriettiva. L'immagine inversa di un elemento $y \in Y$, denotata con $f^{-1}(\{y\})$, è l'insieme di tutti gli elementi $x \in X$ tali che $f(x) = y$. Se $f$ è suriettiva, allora $f^{-1}(\{y\}) \not = \emptyset$ per ogni $y \in Y$. Questo significa che per ogni elemento $y$ nel codominio, esiste almeno un elemento $x$ nel dominio che viene mappato su $y$.
> >
> > In sostanza, la condizione $f^{-1}(\{y\}) \not = \emptyset$ afferma che l'insieme delle soluzioni dell'equazione $f(x) = y$ non è vuoto per ogni $y \in Y$. Questo è equivalente a dire che ogni elemento di $Y$ è immagine di almeno un elemento di $X$.
> >
> > È importante notare che una funzione può essere iniettiva (ogni elemento del codominio è immagine di al più un elemento del dominio), suriettiva, entrambe le cose (biettiva) o nessuna delle due. La suriettività riguarda solo la copertura del codominio, mentre l'iniettività riguarda la distinzione degli elementi del dominio.

> [!info] Definizione di funzione biiettiva
> 
> Una funzione $f: X \rightarrow Y$ è detta **biiettiva** (o una biezione) se soddisfa contemporaneamente le seguenti due proprietà:
> 
> - $f$ è iniettiva $\iff \forall y \in Y, f^{-1}(\{  y \}) = \emptyset \text{ oppure singleton}$
> - $f$ è suriettiva $\iff \forall y \in Y, f^{-1}(\{ y \}) \not = \emptyset$
> 
> **Caratterizzazione unificata:**  
> Una funzione $f$ è biiettiva se:
> 
> $$
>   \forall y \in Y, f^{-1}(\{ y \}) \text{ è un singleton}
> $$
> 
> In altre parole, ogni elemento del codominio ha **esattamente un antecedente** nel dominio.
> 
> > [!tip]- AI-splaining
> > Una funzione biiettiva è un concetto fondamentale in matematica, in particolare nella teoria degli insiemi e nelle sue applicazioni. Per comprenderla appieno, è cruciale analizzare le due proprietà che la definiscono: iniettività e suriettività. Una funzione è biiettiva se e solo se è sia iniettiva che suriettiva. Cercheremo di sviscerare ogni aspetto, partendo dalle definizioni e arrivando alla caratterizzazione unificata.
> >
> > Innanzitutto, è importante ricordare cosa sia una funzione in generale. Una funzione $f: X \rightarrow Y$ è una relazione che associa ad ogni elemento $x$ dell'insieme $X$ (dominio) un **unico** elemento $y$ dell'insieme $Y$ (codominio).  Il simbolo $f(x)$ rappresenta l'immagine di $x$ tramite la funzione $f$.
> >
> > **Iniettività:** Una funzione $f$ è detta iniettiva (o uno-a-uno) se elementi distinti del dominio vengono mappati in elementi distinti del codominio. Formalmente, questo significa che se $x_1 \neq x_2$, allora $f(x_1) \neq f(x_2)$.  La definizione fornita,  $f$ è iniettiva $\iff \forall y \in Y, f^{-1}(\{  y \}) = \emptyset \text{ oppure singleton}$, è un modo equivalente per esprimere l'iniettività.  Cerchiamo di capire cosa significa.  $f^{-1}(\{ y \})$ rappresenta l'insieme di tutti gli elementi $x$ nel dominio $X$ tali che $f(x) = y$.  Se questo insieme è vuoto, significa che nessun elemento del dominio viene mappato in $y$. Se questo insieme contiene un solo elemento, significa che esiste un unico elemento nel dominio che viene mappato in $y$.  Quindi, se per ogni elemento $y$ nel codominio, l'insieme degli antecedenti di $y$ è vuoto o contiene un solo elemento, la funzione è iniettiva.
> >
> > **Suriettività:** Una funzione $f$ è detta suriettiva (o onto) se ogni elemento del codominio è immagine di almeno un elemento del dominio. In altre parole, per ogni $y \in Y$, esiste almeno un $x \in X$ tale che $f(x) = y$. La definizione fornita, $f$ è suriettiva $\iff \forall y \in Y, f^{-1}(\{ y \}) \not = \emptyset$, esprime proprio questo concetto.  $f^{-1}(\{ y \})$ rappresenta, come prima, l'insieme degli antecedenti di $y$. Se questo insieme è non vuoto, significa che esiste almeno un elemento nel dominio che viene mappato in $y$. Quindi, se per ogni elemento $y$ nel codominio, l'insieme degli antecedenti di $y$ è non vuoto, la funzione è suriettiva.
> >
> > **Caratterizzazione unificata:** La caratterizzazione unificata,  $\forall y \in Y, f^{-1}(\{ y \}) \text{ è un singleton}$,  combina le due proprietà di iniettività e suriettività in un'unica affermazione.  Essa afferma che per ogni elemento $y$ nel codominio, l'insieme degli antecedenti di $y$ deve contenere esattamente un elemento.  Questo significa che ogni elemento del codominio ha un unico antecedente nel dominio.  Se l'insieme degli antecedenti è vuoto, la funzione non è suriettiva. Se l'insieme degli antecedenti contiene più di un elemento, la funzione non è iniettiva.  Solo quando l'insieme degli antecedenti è un singleton, la funzione è sia iniettiva che suriettiva, e quindi biiettiva.
> >
> > **In sintesi:** Una funzione biiettiva stabilisce una corrispondenza perfetta tra il dominio e il codominio. Ogni elemento del dominio è associato a un unico elemento del codominio, e ogni elemento del codominio è associato a un unico elemento del dominio.  Questo concetto è cruciale per definire funzioni inverse, che esistono solo per le funzioni biiettive.  La funzione inversa "inverte" la corrispondenza stabilita dalla funzione originale, mappando ogni elemento del codominio nel suo unico antecedente nel dominio.

## Diagrammi

> [!info] Definizione di Diagramma
> 
> Un diagramma è una rappresentazione strutturata costituita da:
> - Una **collezione di insiemi non vuoti**, detti **nodi** del diagramma;
> - Un insieme di **applicazioni** (o funzioni) che collegano tali insiemi, rappresentate graficamente da **frecce** tra i nodi.
>   
> Formalmente, un diagramma è un grafo diretto in cui i nodi sono insiemi e le frecce rappresentano applicazioni tra questi insiemi.
> 
> > [!tip]- Spiegazione e notazione
> > Un diagramma può essere rappresentato come:
> > 
> > ```tikz
> >      \usepackage{tikz-cd}
> >     \begin{document}
> >    \begin{tikzcd}
> >    & X \arrow[dr, "f"] & \\
> >    Z \arrow[ur, "h"] & & Y \arrow[ll, "g"]
> >    \end{tikzcd}
> >    \end{document}
> > ```
> > dove:
> > - $X, Y, Z$ sono insiemi (i nodi del diagramma)
> > - $f: X \rightarrow Y$,  $g: Y \rightarrow Z$ e $h: Z \rightarrow X$ sono applicazioni che collegano gli insiemi.

## Operazioni sulle funzioni

> [!info] Definizione di composizione
> 
> Data una funzione $f: X \rightarrow Y$ e una funzione $g: Y \rightarrow Z$, la **composizione** di $f$ e $g$ è una nuova funzione:
> 
> $$
>   X \xrightarrow{f} Y \xrightarrow{g} Z
> $$
> 
> definita come:
> 
> $$
>   X \xrightarrow{g \,\circ\, f} Z
> $$
> 
> dove:
> 
> $$
>   (g \circ f)(x) = g(f(x)) \,\,\, \forall x \in X
> $$

> [!abstract] Proposizione: Biiettività e Funzione Inversa
> 
> Data una funzione $f: X \rightarrow Y$, $f$ è biiettiva se e solo se esiste una funzione $g: Y \rightarrow X$ tale che:
> 
> 1. $g \circ f = id_{X}$ (la composizione $g$ seguita da $f$ è l'identità su $X$)
> 2. $f \circ g = id_{Y}$ (la composizione $f$ seguita da $g$ è l'identità su $Y$)
> 
> In tal caso, $g$ è chiamata la **funzione inversa** di $f$. Se esiste, la funzione inversa è **unica**

> [!abstract]- Dimostrazione
> 
> **Direzione 1: $f$ biettiva implica l'esistenza di $g$**
> 
> Se $f$ è biiettiva, allora:
> 
> $$
>   \forall y \in Y, \exists!x \in X \text{ t.c. } f(x) = y
> $$
> 
> Poniamo $g(y) = x$, dove $x$ è l'unico element in $X$ tale che $f(x) = y$. Quindi $g: Y \rightarrow X$ è ben definita.
> 
> **Verifica:**
> 
> 1. $g \circ f = id_{X}$
> 	1. Per ogni $x \in X$, poniamo $y = f(x)$
> 	2. Allora, $g(f(x)) = g(y) = x$ (per definizione di $g$)
> 	3. Quindi: 
> 	   $$
> 	    g \circ f = id_{X}
>       $$
> 2. $f \circ g = id_{Y}$ **(omessa)**
> 	1. La verifica che $f(g(y)) = y$ per ogni $y \in Y$ segue in modo analogo.
> 
> ---
> 
> **Direzione 2: Esistenza di $g$ implica $f$ biiettiva**
> 
> Supponiamo che esista una funzione $g: Y \rightarrow X$ tale che:
> $$
>   f \circ g = id_{Y} \text{ e } g \circ f = id_{X}
> $$
> 
> **Verifica che $f$ è suriettiva:**
> 
> 1. Sia $y \in Y$.
> 2. Poiché $f \circ g = id_{Y}$, abbiamo:
>     $$
>       f(g(y)) = y
>     $$
>
> Questo implica che $y$ è immagine di $g(y) \in X$, quindi $f$ è **suriettiva**
> 
> **Verifica che $f$ è iniettiva:**
> 
> 1. Siano $x, x' \in X \text{ tali che } f(x) = f(x')$
> 2. Applichiamo $g$ a sinistra:
>     $$
>       g(f(x)) = g(f(x'))
>     $$
> 3. Poiché $g \circ f = id_{X}$, otteniamo:
>     $$
>       x = g(f(x)) = g(f(x')) = x'
>     $$
> Quindi $f$ è iniettiva.
> 
> Analogamente, si verifica che $g$ è sia iniettiva che ruriettiva, e quindi è biiettiva.
> 
> > [!warning]- GPT Says
> > ### **Enunciato**
> > 
> > La proposizione afferma che una funzione f:X→Yf: X \to Y è biiettiva **se e solo se** esiste una funzione g:Y→Xg: Y \to X tale che:
> > 
> > 1. f∘g=idYf \circ g = \mathrm{id}_Y (la composizione ff dopo gg è l'identità su YY),
> > 2. g∘f=idXg \circ f = \mathrm{id}_X (la composizione gg dopo ff è l'identità su XX).
> > 
> > Inoltre, questa gg è chiamata la **funzione inversa** di ff, e se esiste, è unica.
> >
> >---
> >
> > ### **Prima direzione: ff biiettiva implica l'esistenza di gg**
> > 
> > #### Cosa significa che ff è biiettiva?
> > 
> > - **Iniettività:** Se due elementi del dominio XX hanno la stessa immagine in YY (cioè f(x)=f(x′)f(x) = f(x')), allora x=x′x = x'. Questo garantisce che ff "non confonde" elementi distinti di XX.
> > - **Suriettività:** Ogni elemento del codominio YY è immagine di almeno un elemento del dominio XX. Questo significa che ff "copre" tutto YY.
> > 
> > #### Come definiamo gg?
> > 
> > Se ff è biiettiva:
> > 
> > - Per ogni y∈Yy \in Y, esiste un **unico** x∈Xx \in X tale che f(x)=yf(x) = y (per suriettività).
> > - Definiamo g:Y→Xg: Y \to X assegnando a ogni y∈Yy \in Y il corrispondente x∈Xx \in X tale che f(x)=yf(x) = y. In simboli: g(y)=x,dove f(x)=y.g(y) = x, \quad \text{dove } f(x) = y.
> > 
> > Questa definizione è valida perché, essendo ff biiettiva, xx è unico (grazie all'iniettività).
> > 
> > #### Verifica delle proprietà di gg:
> > 
> > 1. **g∘f=idXg \circ f = \mathrm{id}_X:**
> >     - Prendiamo un qualsiasi x∈Xx \in X.
> >     - Consideriamo y=f(x)y = f(x) (l'immagine di xx tramite ff).
> >     - Per costruzione di gg, abbiamo g(f(x))=g(y)=xg(f(x)) = g(y) = x.
> >     - Questo dimostra che: (g∘f)(x)=x∀x∈X.(g \circ f)(x) = x \quad \forall x \in X.
> > 2. **f∘g=idYf \circ g = \mathrm{id}_Y (omessa):**
> >     - La verifica che f(g(y))=yf(g(y)) = y per ogni y∈Yy \in Y segue in modo analogo.
> > 
> > Quindi, gg è la funzione inversa di ff.
> >
> >---
> >
> > ### **Seconda direzione: Esistenza di gg implica che ff è biiettiva**
> > 
> > #### Supponiamo che esista g:Y→Xg: Y \to X tale che:
> > 
> > 1. f∘g=idYf \circ g = \mathrm{id}_Y,
> > 2. g∘f=idXg \circ f = \mathrm{id}_X.
> > 
> > Dobbiamo dimostrare che ff è:
> > 
> > - **Suriettiva**, e
> > - **Iniettiva**.
> > 
> > ---
> > 
> > #### **1. ff è suriettiva**
> > 
> > - Per suriettività, dobbiamo mostrare che: ∀y∈Y, ∃x∈X tale che f(x)=y.\forall y \in Y, \, \exists x \in X \text{ tale che } f(x) = y.
> > - Sia y∈Yy \in Y.
> >     - Applicando gg, otteniamo g(y)∈Xg(y) \in X.
> >     - Applichiamo ff a g(y)g(y): per ipotesi, f(g(y))=yf(g(y)) = y (questa è l'identità su YY).
> >     - Quindi yy è effettivamente immagine di g(y)g(y), che appartiene a XX.
> > - Concludiamo che ogni y∈Yy \in Y ha un preimmagine in XX, quindi ff è suriettiva.
> > 
> > ---
> > 
> > #### **2. ff è iniettiva**
> > 
> > - Per iniettività, dobbiamo mostrare che: ∀x,x′∈X, f(x)=f(x′)  ⟹  x=x′.\forall x, x' \in X, \, f(x) = f(x') \implies x = x'.
> > - Siano x,x′∈Xx, x' \in X tali che f(x)=f(x′)f(x) = f(x').
> >     - Applicando gg a entrambi i lati, otteniamo: g(f(x))=g(f(x′)).g(f(x)) = g(f(x')).
> >     - Per ipotesi, g∘f=idXg \circ f = \mathrm{id}_X, quindi g(f(x))=xg(f(x)) = x e g(f(x′))=x′g(f(x')) = x'.
> >     - Quindi x=x′x = x'.
> > - Concludiamo che ff è iniettiva.
> > 
> > ---
> > 
> > #### Conclusione
> > 
> > Poiché ff è sia suriettiva che iniettiva, ff è biiettiva.
> >
> >---
> >
> > ### **Osservazioni finali**
> > 
> > 1. **Unicità di gg:** La funzione inversa gg è unica, perché per ogni y∈Yy \in Y c'è un unico x∈Xx \in X tale che f(x)=yf(x) = y.
> > 2. **Significato intuitivo:** Una funzione biiettiva stabilisce una corrispondenza "uno a uno" tra gli elementi di XX e YY, e l'inversa gg semplicemente "inverte" questa corrispondenza.
> >
> >---
> >
> > ### Diagramma per aiutare lo studio:
> > 
> > $$X \overset{f}{\underset{g}{\rightleftharpoons}} Y$$
> > 
> > - $f:X→Yf: X \to Y$,
> > - $g:Y→Xg: Y \to X$,
> > - $f∘g=idYf \circ g = \mathrm{id}_Y$,
> > - $g∘f=idXg \circ f = \mathrm{id}_X$.

## Teorema di struttura per le applicazioni

Chiamato anche "teorema di fattorizzazione canonica", afferma che ogni applicazione (o funzione) $f: X \rightarrow Y$ può essere "scomposta" in modo canonico attraverso 3 applicazioni più semplici:

1. Una proiezione canonica ($\pi$) che è suriettiva;
2. Un'applicazione biiettiva ($\phi$);
3. Un'inclusione canonica ($i$) che è iniettiva.

La scomposizione è quindi $f = i \circ\phi\circ\pi$.

### Passo 1: Definiamo una relazione d'equivalenza su X

Data un'applicazione $f: X \rightarrow Y$ si definisce una relazione $\sim$ sull'insieme di partenza $X$ nel seguente modo:
$$
\forall x,x' \in X, x \sim x' \iff f(x) = f(x')
$$
Cioè, due elementi di X sono in relazione se hanno la stessa immagine tramite $f$.

$\sim$ è una relazione di equivalenza:

1. $x \sim x \implies f(x) = f(x)$ che è ovvio. Pertanto è riflessiva.
2. $x \sim x' \implies f(x) = f(x') \implies f(x') = f(x) \implies x' \sim x$ . Pertanto è simmetrica.
3. $x \sim x' \text{ e } x' \sim x''$ implicano rispettivamente $f(x) = f(x') \text{ e } f(x') = f(x'')$, implicando a loro volta che $f(x) = f(x'') \implies x \sim x''$. Pertanto è transitiva.

Essendo riflessiva, simmetrica e transitiva possiamo concludere che è una relazione di equivalenza.

### Passo 2: Consideriamo l'insieme quoziente $X/\sim$

Essendo $\sim$ una relazione d'equivalenza, possiamo considerare l'insieme $X/\sim$, ossia l'insieme di tutte le classi di equivalenza $[x]$ di $X$.

Ogni classe di equivalenza $[x]$ è formata da tutti gli elementi tali che $x' \in X \text{ t.c. f(x') = f(x)}$.
Geometricamente, possiamo notare che ogni classe di equivalenza $X' \in X/\sim$ corrisponde all'insieme $f^{-1}(\{y\})$ per un certo $y$ che appartiene all'immagine (codominio) di $f$.

### Passo 3: Le tre applicazioni canoniche

1. La proiezione canonica $\pi$ (pi greco):
	1. $\pi: X \rightarrow X/\sim$
	2. Definita da $\pi(x) = [x]$ (associa ogni elemento alla sua classe di equivalenza)
	3. Questa applicazione è **suriettiva** per definizione stessa dell'insieme quoziente (ogni classe di equivalenza ha almeno un rappresentante in $X$).
2. L'applicazione $\phi$ (phi):
	1. $\phi: X/\sim \rightarrow f(X)$ (dove $f(X)$ è l'immagine di $f$, cioè $f(X) = \{ y \in Y \text{ t.c. } \exists x \in X, f(x) = y \}$)
	2. Definita da $\phi(x) = f(x)$
	3. È **biiettiva**
3. L'inclusione canonica $i$:
	1. $i: f(x) \rightarrow Y$
	2. Definita da $i(y) = y \text{,  } \forall y \in f(X)$
	3. Questa applicazione è semplicemente l'inclusione dell'immagine $f(X)$ nel codominio $Y$.
	4. È sempre **iniettiva**

A cosa ci serve questo teorema? Per ora non ho la più pallida idea. In teoria lo capiamo più avanti. I'm tired boss.

# Anelli

Prima di iniziare questo nuovo argomento, definiamo per comodità un insieme $Z$ "munito di operazione _opposto_":
$$
\begin{align}
& \mathbb{Z} \xrightarrow{-(.)} \mathbb{Z} \\
& a \mapsto -a
\end{align}
$$
e di due __operazioni binarie__:

1. **Somma**:
$$
\begin{align}
& \mathbb{Z} \times \mathbb{Z} \xrightarrow{+} \mathbb{Z} \\
& (a, b) \mapsto a+b
\end{align}
$$
2. Prodotto:
$$
\begin{align}
& \mathbb{Z} \times \mathbb{Z} \xrightarrow{*} \mathbb{Z} \\ \\

(a,b) \mapsto a*b = &\begin{cases}
\text{se } b = 0 \rightarrow 0 \\
\text{se } b > 0 \rightarrow a+a+\dots+a \text{ (per b volte)} \\
\text{se } b < 0 \rightarrow (-(a*(-b)))
\end{cases} \\
\end{align}
$$

L'operazione di "opposto" associa ad ogni $a \in \mathbb{Z}$ l'unico elemento $-a \text{ t.c. } a+(-a) = 0$

> [!info] Definizione di Anello
> 
> Un anello (commutativo unitario) è il dato di una sestupla $(A, +, -, *, 0_{A}, 1_{A})$ dove:
> 
> - A $\longrightarrow$ insieme non vuoto ($A \not= \emptyset$)
> - $+,* \rightarrow A \times A \longrightarrow A$ (sono operazioni binarie)
> - $- \rightarrow A \longrightarrow A$ (operazione di opposto)
> - $0_{A} \rightarrow 0_{A} \in A$ (elemento neutro dell'addizione)
> - $1_{A} \rightarrow 1_{A} \in A$ (elemento neutro della moltiplicazione)

Questi dati devono soddisfare 8 proprietà, di cui 4 sull'addizione e 4 sul prodotto:

> [!info] Proprietà sull'addizione
> 
> 1) **Commutatività della Somma**: $\forall a,b \in A \text{ vale che } a+b = b+a$ 
> 2) **Associatività della Somma**: $\forall a,b,c \in A \text{ vale che } (a+b)+c = a+(b+c)$
> 3) **Elemento Neutro della Somma**: $\forall a \in A \text{ vale che } a + 0_{A} = 0_{A} + a = a$
> 4) **Opposto**: $\forall a \in A \text{ vale che } a+(-a) = 0_{A}$
>    
> > [!note] Gruppo Abeliano
> > Queste quattro proprietà indicano che $(A,+,-,0_{A})$ è un **Gruppo Abeliano** in notazione additiva _(vedi gruppi)_

> [!info] Proprietà sul prodotto
> 
> 5) **Associatività del Prodotto**: $\forall a,b,c \in A \text{ vale che } a(b*c) = (a*b)c = abc$
> 6) **Distributività**: $\forall a,b,c \in A \text{ vale che } \begin{cases} (b+c) = ab+ac \\ (a+b)c = ac+bc \end{cases}$
> 7) **Elemento Neutro del Prodotto**: $\forall a \in A \text{ vale che } a*1_{A} = 1_{A} * a = a$
> 8) **Commutatività del Prodotto**: $\forall a,b \in A \text{ vale che } ab=ba$
> 
> > [!warning] Osservazioni
> > Notiamo che la proprietà 7 (elemento neutro del prodotto) rende l'anello **unitario**, mentre la proprietà 8 (communitatività del prodotto) rende l'anello **commutativo**

Ad esempio, l'insieme $\mathbb{Z}$ dei numeri relativi è un anello commutativo unitario, mentre l'insieme $\mathbb{N}$ dei numeri naturali non è un anello commutativo unitario poiché non definisce un'operazione di "opposto".

Vediamo alcune proprietà degli Anelli:

1. $\forall a \in A \text{ vale che } a*0_{A} = 0_{A}$
2. Se $0_{A} = 1_{A}$, allora $\forall a \in A$ si ha $a=0_{A}$, ovvero $A = \{ 0_{A} \}$

## Elementi Invertibili

> [!info] Definizione di Elemento Invertibile
> 
> Sia $A$ anello commutativo unitario con $1_{A} \not= 0_{A}$.
> Un elemento $a \in A$ è detto **invertibile** (o **unità**) se esiste un elemento $b \in A$ tale che:
> $$
> a*b = b*a = 1_{A}
> $$
> L'elemento $b$ è detto **inverso di $a$** e viene solitamente denotato con $a^{-1}$

> [!note]- Qualche esempio concreto
> 
> 1. Anello degli Interi ($\mathbb{Z}$)
> 	- $a = 1 \implies a^{-1} = 1$ ($1*1=1=1_{A}$)
> 	- $a = -1 \implies a^{-1} = -1$ ($-1 * -1 = 1 = 1_{A}$)
> 	- NOTA: Gli altri interi non hanno inversi in $\mathbb{Z}$
> 2. Anello dei Numeri Razionali ($\mathbb{Q}$)
> 	- $a = \frac{3}{2} \implies a^{-1} = \frac{2}{3}$ ($\frac{3}{2} * \frac{2}{3} = 1 = 1_{A}$) 
> 	- $a = -5 \implies a^{-1} = -\frac{1}{5}$ ($-5 * -\frac{1}{5} = 1 = 1_{A}$)
> 	- GENERICO: Qualsiasi numero razionale diverso da zero $\frac{a}{b}$ ha un inverso $\frac{b}{a}$
> 
> Sono solo alcuni esempi ma rendono l'idea.

## Proprietà dell'anello $\mathbb{Z}$

L'anello $\mathbb{Z}$ ha alcune proprietà particolari.

Esiste il sottoinsieme $\mathbb{N^*} = \mathbb{N}/\{ 0 \} \subset \mathbb{Z}$ che permette di definire una relazione di ordinamento su $\mathbb{Z}$ che si scrive come $a < b \iff a-b \in \mathbb{N^*}$

> [!info] Proprietà di Tricotomia
>$$
>\forall a \in \mathbb{Z} \text{ si ha: } \begin{cases}
>a \in \mathbb{N^*} \implies \text{è positivo} \\
>a = 0 \implies \text{è nullo} \\
>-a \in \mathbb{N^*} \implies \text{è negativo}
>\end{cases}
>$$

> [!info] Principio di Buon Ordinamento
> 
> Questo principio ci garantisce che ogni sottoinsieme $E \subset \mathbb{N^*}$ non vuoto possiede un più piccolo elemento, ossia:
> 
> $$
> \exists c \in E \text{ t.c. } \forall e \in E/\{ c \} \text{ si ha } e>c
> $$

> [!info] legge di cancellazione in $\mathbb{Z}$
> Se $ab=ac$ con $a\not=0$, allora $b=c$

## Relazione di Divisibilità

Introduciamo la relazione di divisibilità, espressa come:
$$
a,b \in A: a\mid b  \iff \exists c \in A \text{ t.c. } b = a*c
$$
> [!warning] Attenzione
> La relazione $a \mid b$ si legge come "a divide b", oppure "a è divisore di b" oppure "b è divisibile per a". Quindi $2 \mid 4$  significa che "2 divide 4", mentre $2 \nmid 7$ sarebbe "2 non divide 7"

Questa relazione è:
- **Riflessiva**: $\forall a \in A \text{ vale che } a = a*1_{A}$
- **Transitiva**: 
$$
\begin{align}
& \text{Dati } a,b,c \in A \\ &\\& \begin{cases}
a\mid b \iff b = a*a' (\exists a' \in A) \\
b\mid c \iff c = b*b' (\exists b' \in A) \\
\end{cases} \\
&  \\
& \text{quindi } c = a*a'*b' = a*(a'*b') = a*a'' \implies c = a*a'' \iff a\mid c
\end{align}
$$
Non è invece __simmetrica__ (es. $2\mid4$ mentre $4\nmid3$) né **antisimmetrica** (quest'ultimo lo è solo su $\mathbb{N^*}$)

La divisibilità è anche compatibile con la somma (e con il prodotto):
$$
a|b, a|c \implies \begin{cases}
a \mid b+c \\
a \mid b*c
\end{cases}
$$
Più generalmente, se $\alpha, \beta \in A$, $a \mid b$ e $a \mid c \implies a \mid \alpha*b+\beta*c$

## Elementi Irriducibili e Primi

> [!info] Definizione di Elemento Irriducibile
> 
> Un elemento $a \in A/A^{x}$ è detto __irriducibile__ se:
> $$
> \forall b,c \in A \text{ vale che } a=bc \implies b \in A^x \lor c \in A^x
> $$
> 
> > [!warning] Attenzione!
> > L'or nella definizione è __esclusivo__, poiché se sia $b$ che $c$ fossero invertibili, allora lo sarebbe anche $a$ e verrebbe meno la premessa per cui $a$ non lo è.
> 
> > [!tip]- Spiegazione intuitiva
> > In termini più semplici, un elemento irriducibile è un elemento che non può essere "fattorizzato" ulteriormente in elementi più piccoli (prodotto di due elemento non invertibili) all'interno dell'anello in cui stiamo lavorando. È come un "mattone" fondamentale dell'anello.
> > 
> > Qualche esempio su $\mathbb{Z}$:
> > - $2,3,5,7,11,\dots$ sono irriducibili perché possono essere divisi solo per $1$ e per se stessi;
> > - $-2,-3,-5,\dots$ sono anche irriducibili, poiché $-2 = (-1)*2$, ma $-1$ è invertibile;
> > - $1,-1$ non sono irriducibili;
> > - $4$ non è irriducibile perché $4 = 2*2$
> > - $6$ non è irriducibile perché $6=2*3$

> [!info] Definizione di Numero Primo
> 
> Un elemento $a \in A/A^{x}$ è detto __primo__ se:
> $$
> \forall b,c \in A \text{ vale che } a \mid bc \implies a \mid b \lor a \mid c
> $$

> [!info] Lemma
> 
> $$
> p \in \mathbb{Z} \text{ primo} \iff \text{irriducibile}
> $$
> 
> > [!tip] Spiegazione
> > In poche parole, questo lemma ci dice che i numeri primi ed i numeri riducibili coincidono in $\mathbb{Z}$, ossia i numeri irriducibili in questo anello sono i numeri primi ed il loro opposto.

## Valore Assoluto

> [!info] Definizione di Valore Assoluto
> 
> $$
> \mathbb{Z} \xrightarrow{|·|} \mathbb{N}
> $$
> 
> $$ \text{Dato } a \in \mathbb{Z} \begin{cases}
> a = 0 \implies |a| = 0 \\
> a \not= 0 \implies |a| = \{ a, -a \} \cap \mathbb{N}
> \end{cases}$$

## Divisione Euclidea

> [!info] Definizione di Divisione Euclidea
> 
> Dati $a,n \in \mathbb{Z}$, allora esistono unicamente determinati:
> $$
> q \in \mathbb{Z}, r \in \{ 0,\dots,|n|-1 \} \text{ t.c. } a = nq+r
> $$
> 
> > [!warning] Attenzione
> > - Importante notare che $0 \leq r < |n|$
> > - n è il divisore, q il quoziente, r il resto.

## Congruenza

> [!info] Definizione di Congruenza
> 
> $$
> a \equiv b \text{ (mod. n) }\begin{cases}
> \iff n \mid a-b \text{ (quindi b è il resto di } \frac{a}{b} \text{)} \\
> \iff \exists q \in \mathbb{Z} \text{ t.c. } a-b = qn
\end{cases} 
> $$

La congruenza modulo n è una __relazione d'equivalenza__:
1. __riflessiva__: $a \equiv_{n} a$, $n \mid a-a$ è vero poiché $\forall x \in \mathbb{Z}/\{ 0 \} \text{ vale che } x \mid 0$
2. **simmetrica**: $a \equiv_{n} b \implies b \equiv_{n} a$, ovvero $n \mid a-b \implies n \mid b-a$
3. **transitiva**: $a \equiv_{n}b \text{ e } b \equiv_{n} c \iff n \mid b-a \text{ e } n \mid c-b \implies n \mid c-b+c-a \implies n \mid c-a \iff c \equiv_{n} a \iff a \equiv_{n} c$
Facciamo alcuni esempi:

Congruenza modulo 2:
$$
\underbrace{2\mathbb{Z}}_{[0] \text{(numeri pari)}} \sqcup \underbrace{2\mathbb{Z} + 1}_{[1] \text{(numeri dispari)}}
$$
$$
\mathbb{Z}\text{ }/\equiv_{2} \text{ }= \{ 2\mathbb{Z}, 2\mathbb{Z}+1 \}
$$
```tikz
\usepackage{tikz}

\begin{document}
\begin{tikzpicture}
  \foreach \n in {-3,-2,-1,0,1,2,3} {
    \node (\n) at (\n,0) [font=\Large] {\n};
    \ifodd\n
      \fill[blue] (\n, -0.5) circle (0.10cm);
    \else
      \fill[red] (\n, -0.5) circle (0.10cm);
    \fi
  }
\end{tikzpicture}
\end{document}
```

Congruenza modulo 3:
$$
\underbrace{3\mathbb{Z}}_{[0]} \sqcup \underbrace{3\mathbb{Z}+1}_{[1]} \sqcup \underbrace{3\mathbb{Z}}_{[2]}
$$
$$
\mathbb{Z}\text{ }/\equiv_{3} \text{ } = \{ 3\mathbb{Z}, 3\mathbb{Z}+1, 3\mathbb{Z}+2 \}
$$
```tikz
\usepackage{tikz}

\begin{document}
\begin{tikzpicture}
  \foreach \n in {-3,-2,-1,0,1,2,3} {
    \node (\n) at (\n,0) [font=\Large] {\n};
    \pgfmathparse{abs(\n)}
    \let\absn\pgfmathresult
    \pgfmathtruncatemacro{\resto}{mod(\absn,3)}
    \ifnum\resto=0
      \def\col{red}
    \else\ifnum\resto=1
      \def\col{blue}
    \else
      \def\col{green}
    \fi\fi
    \fill[\col] (\n, -0.5) circle (0.10cm);
  }
\end{tikzpicture}
\end{document}
```

Ora concentriamoci sull'anello $\mathbb{Z}/n\mathbb{Z}$.

$\mathbb{Z}/n\mathbb{Z} = \mathbb{Z}/\equiv_{n}$ con $n > 0$ ed è l'insieme quoziente di $\mathbb{Z}$ sulla congruenza modulo n.

$[a] \in \mathbb{Z}/n\mathbb{Z} = \{ x: x\equiv a \text{ mod. }n \} = a +n\mathbb{Z}$ ovvero tutti gli elemento che danno resto $a$ quando dividi per $n$. Gli elementi di $\mathbb{Z}/n\mathbb{Z}$ sono le classi di equivalenza mod. $n$.

Le operazioni $+,*,-$ sono compatibili con $\equiv_{n}$

1. Compatibilità con opposto: $\forall a, a' \in \mathbb{Z} \text{ vale che } a \equiv_{n} a' \iff -a \equiv_{n} -a'$
2. Compatibilità con somma: $\forall a,a',b,b' \in \mathbb{Z} \text{ vale che } a \equiv_{n} a',b \equiv_{n}b' \implies a+b\equiv_{n}a'+b'$
3. Compatibilità con prodotto: $\forall a,a',b,b' \in \mathbb{Z} \text{ vale che } a \equiv_{n} a',b \equiv_{n}b' \implies ab \equiv_{n} a'b'$

Operatori:
- Opposto: $-[a] := [-a]$
- Somma: $[a]+[b] = [a+b]$
- Prodotto: $[a]*[b] = [a*b]$

Quindi $(\mathbb{Z}/n\mathbb{Z}, +, - *, [0], [1])$ è un **anello commutativo unitario**.

# Massimo Comun Divisore

> [!info] Definizione di Massimo Comun Divisore
> $$
> \text{Data } (a,b) \in \mathbb{Z}\times \mathbb{Z} \text{ con } (a,b) \not = (0,0)
> $$
> $d \in \mathbb{N}$ è $MCD$ di $a$ e $b$ se:
> 1. $d \mid a$ e $d \mid b$
> 2. se $\exists d' \in \mathbb{N} \text{ t.c. } d' \mid a \text{ e } d' \mid b, \text{ allora } d' \mid d$ ossia ogni dividore di $a$ e $b$ divide anche $d$
> 
> Se $d$ soddisfa 1. e 2. allora è **unico**

> [!info] Definizione di Coprimi (o primi tra loro)
> Se $MCD(a,b) = 1$, si dice che $a$ e $b$ sono **coprimi** o primi tra loro.

> [!info] Lemma
> Dato $\delta =MDC(a,b) \text{ vale che } a\mathbb{Z}+b\mathbb{Z}=\delta \mathbb{Z} \text{ con } \delta >0, (a,b)\not = (0,0)$

### Minimo Comune Multiplo

> [!info] Definizione di Minimo Comune Multiplo (mcm)
> 
> Dati $m_{1},\dots m_{k} \in \mathbb{Z}/\{ 0 \}$, il **minimo comune multiplo** (mcm) di $m_{1},\dots,m_{k}$ è l'unico intero $m$ t.c.
> 1. $m_{1},\dots,m_{k} \mid m$
> 2. se $\exists m' \text{ t.c. } m_{1},\dots,m_{k} \mid m', \text{ allora } m\mid m'$

Notiamo inoltre che l'insieme $m\mathbb{Z}$ (insieme dei multipli interi di $m$) è dato dall'intersezione degli insiemi dei multipli interi degli $m_{1},\dots,m_{k}$:
$$
m\mathbb{Z} = \{ m_{1}\mathbb{Z} \cap m_{2}\mathbb{Z} \cap \dots \cap m_{k}\mathbb{Z} \}
$$
Inoltre, notiamo che $mcm(a,b) = \frac{ab}{MCD(a,b)}$

## Algoritmo di Euclide x MCD

Dati $a,b > 0$, mi permette di trovare $\delta = MCD(a,b)$. Comincio con la divisione euclidea $a$ diviso $b$ _(funziona sia con $a/b$ che con $b/a$, ma conviene fare $a/b$ con $a>b$)_

```tikz
\usepackage{amsmath}
\usepackage{tikz}
\begin{document}
\begin{tikzpicture}
  \node (n0) at (0,0) [font=\Large] {$a = q_0 b + r_0$};
  \node (n1) at (4.5,0) [font=\Large] {( $0 \le r_0 < b$)};
  \node (n2) at (0,-1.5) [font=\Large] {$b = q_1 r_0 + r_1$};
  \node (n3) at (4.5,-1.5) [font=\Large] {( $0 \le r_1 < r_0$)};
  \node (n4) at (0,-3) [font=\Large] {$r_0 = q_2 r_1 + r_2$};
  \node (n5) at (4.5,-3) [font=\Large] {( $0 \le r_2 < r_1$)};
  \node (n6) at (0,-4.5) [font=\Large] {$\vdots$};
  \node (n7) at (0,-6) [font=\Large] {$r_{n-2} = q_n r_{n-1} + r_n$};
  \node (n8) at (4.5,-6) [font=\Large] {( $0 \le r_n < r_{n-1}$)};
  \node (n9) at (0,-7.5) [font=\Large] {$r_{n-1} = q_{n+1} r_n + 0$};

  \draw[->] (n0) -- (n2);
  \draw[->] (n2) -- (n4);
  \draw[->] (n4) -- (n6);
  \draw[->] (n6) -- (n7);
  \draw[->] (n7) -- (n9);
\end{tikzpicture}
\end{document}
```
Qui l'ultimo resto diverso da $0$, ossia $r_n$ è il nostro $MCD$.

Facciamo un piccolo esempio:
$$
\begin{align}
& \text{Dati } a = 3522, b = 321 \\ & \\
& 3522 = 10*321 + 312 \\
& 321 = 1*312 + 9 \\
& 312 = 34*9 + 6 \\
& 9 = 1*6 + 3 \\
& 6 = 2*3 + 0 \\ & \\
& MCD(3522,321) = 3
\end{align}
$$
## Identità di Bézout

> [!info] Lemma
>Dati $a,b \in \mathbb{Z}$ con $(a,b) \not = (0,0)$ e con $\delta = MCD(a,b)$ allora esistono due interi $u,v \text{ t.c. } au+bv = \delta$
>> [!warning] Nota Bene
>> $u,v$ non sono unicamente determinati.

Come possiamo calcolare $u$ e $v$? Prendiamo come esempio l'algoritmo precedente e vediamo due metodi.

### Metodo bottom-up (Pellarin)

Scriviamo l'ultimo passo dell'algoritmo (quello che contiene il $MCD$ come resto) in funzione del resto, e sostituiamo i resti "risalendo":

$$
\begin{align}
& 3 = 9-1*6 \\
& 3 = 9-1*(312-34*9) \implies 3 = -312+35*9 \\
& 3 = -312+35*(321-312) \implies 3 = 35*321 - 36*312 \\
& 3 = 35*321 - 36*(3522- 321*10) \implies 3 = 395*321 - 36*3522 \\ & \\
& \text{ Abbiamo trovato } u = 395, v=-36
\end{align}
$$
### Metodo top-down (tutor)

Partendo dal primo passo dell'algoritmo, li riscrivo tutti in funzione del resto sostituendo dove possibile; in più, per evitare confusione, scrivo $a$ e $b$ al posto dei due numeri iniziali:

$$
\begin{align}
& a = 3522, b = 321 \\
& 312 = a - 10b \\
& 9 = 321 - 1*312 \implies 9 = 11b - a \\
& 6 = 312 - 34*9 \implies 6 = a-10b -34*(11b-a) \implies 6 = 35a -384b \\
& 3 = 9 - 6 \implies 3 = 11b-a +384b - 35a \implies 3 = 395b - 36a \\ & \\
& \text{Abbiamo trovato } u = 395, v = -36
\end{align}
$$

## Lemma di Gauss

> [!info] Lemma di Gauss
> 
> Se $a,b \in \mathbb{Z}^*$ e $c \in \mathbb{Z}$, e se $MCD(a,b) = 1$, allora $a \mid bc \implies a \mid c$

> [!info] Lemma
> Dato $p \in \mathbb{Z}$ con $p \not\in \{ 0,-1,1 \}$ vale
> $$
> p \text{ irriducibile } \implies p \text{ primo}
> $$

## Elementi invertibili di $\mathbb{Z}/n\mathbb{Z}$

Definiamo $(\mathbb{Z}/n\mathbb{Z})^x = \{ [a]: \exists[b] \text{ con } [a]*[b] = [1] \}$

Abbiamo precedentemente visto che $[a]*[b] = [ab]$, quindi:
$(mod. n) [ab] = 1 \iff n \mid ab-1 \iff \exists k \in \mathbb{Z} \text{ t.c. } ab-1=kn \iff ab-kn = 1$ e quest'ultima è un'identità di Bézout, quindi $MCD(a,b) = 1$.
Quindi $(\mathbb{Z}/n\mathbb{Z})^x = \{ [a]: a \in \mathbb{Z}, MCD(a,n) = 1 \}$, ovvero che gli invertibili in questo insieme sono le classi dei coprimi a $n$.

Esiste quindi un'applicazione biiettiva che porta $r \rightarrow [r]$:
$$
\{ r \in \{ 0,\dots,n-1 \} \text{ t.c. } MCD(r,n) = 1 \} \longrightarrow (\mathbb{Z}/n\mathbb{Z})^x
$$
Esempio:
$$
\begin{align}
& \mathbb{Z}/_{12}\mathbb{Z} = \{ [0],[1],[2],[3],[4],[5],[6],[7],[8],[9],[10],[11] \} \\
& (\mathbb{Z}/_{12}\mathbb{Z})^x = \{ [1],[5],[7],[11] \}
\end{align}
$$
Se invece $n = p \text{ primo}$, allora osserviamo che:
$$
(\mathbb{Z}/_{p}\mathbb{Z})^x = \{ [r]: 1 \leq r \leq p-1 \}
$$
ovvero che $\forall [r] \in (\mathbb{Z}/_{p}\mathbb{Z})/\{ 0 \}, [r] \text{ è invertibile}$.

# Campi

> [!info] Definizione di Campo
> 
> Sia $A$ un anello commutativo unitario. Se per ogni $a \in A \setminus \{0\}$ vale che $a \in A^\times$, allora $A$ è un campo.

# Piccolo Teorema di Fermat

> [!info] Teorema di Fermat
> 
> Sia $p$ un numero primo e $n$ un intero. Allora, $n^p \equiv n \pmod{p}$.
Inoltre:
> - Se $[n] \neq [0]$ (ovvero se $[n] \in \mathbb{F}_{p}$), allora $[n]$ è invertibile e possiede inverso $[x]$.
> - Si ha $[n] = [n]^p$, e quindi $[x][n]^p = 1$.

# Fibonacci

> [!info] Definizione di successione di Fibonacci
> 
> La successione di Fibonacci, denotata con $(F_n)$ per $n \geq 0$, è definita ricorsivamente come segue:
>$$F_0 = 0, \quad F_1 = 1, \quad F_n = F_{n-1} + F_{n-2} \text{ per } n \geq 2.$$
>
> > [!warning] Alcune proprietà
> > Si osservi che $MCD(F_m, F_n) = F_{MCD(m,n)}$, e in particolare $MCD(F_m, F_{m+1}) = F_1 = 1$.
>
> > [!tip]- AI-splaining
> > La successione di Fibonacci è una sequenza di numeri interi in cui ogni numero è la somma dei due numeri precedenti. La definizione formale che ti è stata fornita descrive questo comportamento in modo preciso e ricorsivo. Analizziamo ogni componente di questa definizione.
> >
> > La notazione $(F_n)$ indica che stiamo considerando una sequenza di numeri, dove $F_n$ rappresenta l'n-esimo termine della sequenza. L'indice $n$ è un numero intero maggiore o uguale a 0, il che significa che la sequenza inizia con $n=0$ e continua all'infinito.
> >
> > La definizione ricorsiva è composta da tre parti: i casi base e la relazione di ricorrenza. I casi base sono $F_0 = 0$ e $F_1 = 1$. Questi sono i primi due termini della sequenza e sono definiti direttamente, senza fare riferimento ad altri termini. Sono fondamentali perché forniscono il punto di partenza per calcolare tutti gli altri termini.
> >
> > La relazione di ricorrenza è $F_n = F_{n-1} + F_{n-2}$ per $n \geq 2$. Questa equazione afferma che l'n-esimo termine della sequenza è uguale alla somma dell'(n-1)-esimo termine e dell'(n-2)-esimo termine. In altre parole, per calcolare un termine della sequenza (a partire dal terzo), è necessario sommare i due termini precedenti. Ad esempio, $F_2 = F_1 + F_0 = 1 + 0 = 1$, $F_3 = F_2 + F_1 = 1 + 1 = 2$, $F_4 = F_3 + F_2 = 2 + 1 = 3$, e così via.
> >
> > La seconda parte della definizione che ti è stata fornita, $MCD(F_m, F_n) = F_{MCD(m,n)}$, è un risultato importante che lega la successione di Fibonacci alla teoria dei numeri, in particolare al massimo comun divisore (MCD).  Il MCD di due numeri interi è il più grande numero intero che divide entrambi i numeri senza lasciare resto. Questa proprietà afferma che il massimo comun divisore di due termini qualsiasi della successione di Fibonacci ($F_m$ e $F_n$) è uguale al termine della successione di Fibonacci il cui indice è uguale al massimo comun divisore degli indici dei due termini originali ($m$ e $n$).
> >
> > Ad esempio, consideriamo $m=4$ e $n=6$. Abbiamo $F_4 = 3$ e $F_6 = 8$. Il MCD di 3 e 8 è 1.  Ora calcoliamo $MCD(4,6) = 2$.  Infatti, $F_2 = 1$, che conferma la proprietà.
> >
> > Il caso particolare $MCD(F_m, F_{m+1}) = F_1 = 1$ è una conseguenza diretta della proprietà precedente.  Infatti, se consideriamo $n = m+1$, allora $MCD(m, m+1) = 1$ per qualsiasi intero $m$. Questo perché due numeri consecutivi sono sempre coprimi (cioè, non hanno fattori comuni diversi da 1). Di conseguenza, $MCD(F_m, F_{m+1}) = F_{MCD(m, m+1)} = F_1 = 1$. Questo significa che qualsiasi coppia di termini consecutivi nella successione di Fibonacci è sempre coprima.

# Teorema Fondamentale dell'Aritmetica

> [!info] Definizione:
> $\forall a \in \mathbb{Z}^*$:
> 1. L'insieme $\mathcal{I} = \{ p \text{ primo }: p \mid a \}$ è finito.
> 2. $a = (\pm 1) \prod_{p \text{ primo }} p^{V_{p}(a)}$, dove $V_{p}(a) \in \mathbb{N}$ sono univocamente determinati.
>
> > [!warning] Osservazione:
> > Si sa che $\mathbb{P} = \{ p \in \mathbb{N}: p \text{ primo} \}$ è infinito.
> > Siccome $\forall a \in \mathbb{Z}, \mathcal{I}_{a}$ è finito, $\prod_{p} p^{V_{p}(a)} = \prod_{p \in \mathcal{I}} p^{V_{p}(a)} \cdot \prod_{p\not \in \mathcal{I}} p^{V_{p}(a)}$ ed in quest'ultimo $V_{p}(a)$ sarà $0$ per $p\not \in \mathcal{I}$.
> > Quindi è possibile dividere i numeri primi in divisori di $a$ e non-divisori di $a$ e splittare la produttoria.

Altra osservazione:

Dati $a \prod_{p} p^{V_{p}(a)}$ e $b \prod_{p} p^{V_{p}(b)}$:
- $a*b = \prod_{p} p^{V_{p}(a)} * \prod_{p} p^{V_{p}(b)} =\prod_{p} p^{V_{p}(a) + V_{p}(b)}$
- $p^{V_{p}(a)} * p^{V_{p}(a)} = p^{V_{p}(a) + V_{p}(b)}$
- $V_{p}(ab) = V_{p}(a) + V_{p}(b)$

> [!info] Enunciato
> 
> $\forall a > 0, \exists$ un numero finito di primi distinti $p_{1},\dots,p_{r} \text{ t.c. } a= p_{1}^\alpha * \dots * p_{r}^{\alpha r}$ e questa fattorizzazione è unicamente determianta.

# Divisori di Zero

> [!info] Definizione Di Divisore di Zero
> 
> Dato $A$ anello,l $a \in A$ si dice __divisore__ di zero se $$\exists b \in A\setminus{\{ 0 \}} \text{ t.c. } ab = 0_{A}$$

In $A$ qualsiasi (tranne se $1_{A} = 0_{A}, A= \{ 0 \}$) $0_{A}$ è divisore di $0$.

Nei _campi_ invece (es. $A = \mathbb{Q}, \mathbb{R}, \mathbb{C}, \mathbb{F}_{p}$), ossia quando $\forall a \in K \setminus{\{ 0 \}}, a \text{ è invertibile}$, ovvero $K^x = K \setminus{\{ 0 \}}$, l'unico divisore di zero in $K$ è $0_{K}$.

In $\mathbb{Z}$ se $a$ è divisore di $0$, allora $a=0$ (anche se $\mathbb{Z}$ non è un campo.)

# Dominio

> [!info] Definizione di Dominio
> 
> Dato $A$ anello, $A \not = \{  0 \}$, si dice che $A$ è un **dominio** se l'unico divisore di zero in $A$ è $0_{A}$.

Ogni campo è un dominio, ed anche $Z$ lo è.

# Legge di cancellazione

> [!info] Lemma legge di cancellazione
> 
> Sia $a \in A$ un elemento non divisore di zero. Allora, per ogni $b, c \in A$, se $ab = ac$, si ha $b = c$.
> 
> > [!warning] Osservazione
> > Questo implica la legge di cancellazione in $\mathbb{Z}$ (dominio), quando $a\not = 0$, poiché $0$ è l'unico divisore di zero in $\mathbb{Z}$

# Equazioni in $A$

Ora vediamo come risolvere le equazioni in un anello $A$, ed in particolare $A=\mathbb{Z}, A=\mathbb{Z}/n\mathbb{Z}$.
$$aX=b, a,b \in A$$
dove $X$ è _indeterminata_, ossia può essere sia un valore che un insieme. Quando invece è scritta in minuscolo ($x$) allora si tratta certamente di un valore.

- in $A=\mathbb{Z}$ una soluzione di $aX=b \text{ esiste } \iff a \mid b$ 
	- Infatti se l'insieme delle soluzioni $\not=\emptyset$  e se $x$ è la soluzione, si ha $ax=b \iff a\mid b$
	- Se invece $a \mid b \implies \exists k \in \mathbb{Z} \text{ t.c. } b = ak$ e prendo $k=x$
- In $A=\mathbb{Z}/n\mathbb{Z}, n \in \mathbb{N}$
	- Nel caso in cui $A$ è un anello qualsiasi e $a \in A^x$ di inverso $a^{-1}$, posso moltiplicare termine a termine per $a^{-1}$ $$a^{-1}*aX = a^{-1}*b$$ e quindi l'equazione ha l'unica soluzione $x = a^{-1}b$
	- Se per esempio $A=K$ campo $$aX=b \text{ con } a \not = 0 \text{ ammette sempre l'unica soluzione } x = a^{-1}b$$

> [!info] Proposizione
> 
> L'equazione $aX = b$ con $a, b \in \mathbb{Z}/n\mathbb{Z}$ ammette soluzioni se e solo se $\text{MCD}(\alpha, n) \mid \beta$, dove $a = [\alpha]$, $b = [\beta]$ e $\alpha, \beta \in \mathbb{Z}$.
> > [!tip]- AI-splaining
> > L'equazione $aX = b$ con $a, b \in \mathbb{Z}/n\mathbb{Z}$ ammette soluzioni se e solo se $\text{MCD}(\alpha, n) \mid \beta$, dove $a = [\alpha]$, $b = [\beta]$ e $\alpha, \beta \in \mathbb{Z}$. Questa affermazione riguarda la risolubilità di equazioni lineari in un anello quoziente, nello specifico $\mathbb{Z}/n\mathbb{Z}$, l'anello degli interi modulo *n*.  Cerchiamo di scomporre l'affermazione in modo da comprenderla appieno. Innanzitutto, cosa significa che $a, b \in \mathbb{Z}/n\mathbb{Z}$? Significa che *a* e *b* sono classi di equivalenza modulo *n*.  Ricorda che $\mathbb{Z}/n\mathbb{Z}$ è l'insieme dei resti della divisione per *n*.
> >
> >
> > L'equazione $aX = b$ in $\mathbb{Z}/n\mathbb{Z}$ non è la stessa cosa di un'equazione in $\mathbb{Z}$.  Qui, *X* rappresenta una classe di equivalenza, e l'operazione di moltiplicazione è la moltiplicazione modulo *n*.  Quindi, l'equazione significa che esiste una classe di equivalenza *X* tale che il prodotto di *a* e *X* (modulo *n*) sia uguale alla classe di equivalenza *b* (modulo *n*).  Per rendere più concreto, se $a = [2]$ in $\mathbb{Z}/5\mathbb{Z}$ e $b = [3]$ in $\mathbb{Z}/5\mathbb{Z}$, l'equazione $aX = b$ diventa $[2]X = [3]$.  Questo significa che esiste una classe di equivalenza *X* tale che $2X \equiv 3 \pmod{5}$.
> >
> >
> > Ora, vediamo cosa significa $a = [\alpha]$ e $b = [\beta]$ con $\alpha, \beta \in \mathbb{Z}$.  Questo ci dice che *a* e *b* sono rappresentanti delle rispettive classi di equivalenza.  In altre parole, $\alpha$ e $\beta$ sono interi che appartengono alla classe di equivalenza rappresentata da *a* e *b* rispettivamente.  Ad esempio, se $a = [2]$ in $\mathbb{Z}/5\mathbb{Z}$, allora $\alpha$ potrebbe essere 2, 7, -3, o qualsiasi altro intero congruo a 2 modulo 5.  La scelta di $\alpha$ e $\beta$ non è unica, ma è importante capire che rappresentano la stessa classe di equivalenza.
> >
> >
> > Il cuore dell'affermazione è la condizione $\text{MCD}(\alpha, n) \mid \beta$.  $\text{MCD}(\alpha, n)$ rappresenta il Massimo Comune Divisore di $\alpha$ e *n*.  Il simbolo $\mid$ indica la divisibilità.  Quindi, $\text{MCD}(\alpha, n) \mid \beta$ significa che $\beta$ è divisibile per il Massimo Comune Divisore di $\alpha$ e *n*.  Ad esempio, se $\alpha = 6$ e $n = 8$, allora $\text{MCD}(6, 8) = 2$.  La condizione $2 \mid \beta$ significa che $\beta$ deve essere un numero pari.
> >
> >
> > Perché questa condizione è necessaria e sufficiente per la risolubilità dell'equazione?  Consideriamo l'equazione $aX = b$ in $\mathbb{Z}/n\mathbb{Z}$.  Questa equazione è equivalente a trovare un intero *x* tale che $ax \equiv b \pmod{n}$.  Questo significa che esiste un intero *k* tale che $ax - b = nk$.  Riscrivendo l'equazione, otteniamo $ax - nk = b$.  Possiamo riscrivere questa equazione come $aX = b$ dove $X = x$ e $n$ è un intero.
> >
> >
> > Ora, consideriamo il $\text{MCD}(\alpha, n) = d$.  Questo significa che $d$ divide sia $\alpha$ che *n*.  Quindi, possiamo scrivere $\alpha = d\alpha'$ e $n = d\beta'$ per alcuni interi $\alpha'$ e $\beta'$.  Sostituendo questi valori nell'equazione $ax - nk = b$, otteniamo $d\alpha'x - d\beta'k = b$.  Dividendo entrambi i lati per *d*, otteniamo $\alpha'x - \beta'k = \frac{b}{d}$.  Se $\frac{b}{d}$ non è un intero, allora non esiste una soluzione per *x* e *k*, e quindi l'equazione $ax \equiv b \pmod{n}$ non ha soluzioni.  Questo significa che $d$ deve dividere *b*, ovvero $\text{MCD}(\alpha, n) \mid \beta$.
> >
> >
> > Se $\text{MCD}(\alpha, n) \mid \beta$, allora possiamo trovare un intero *x* tale che $ax \equiv b \pmod{n}$.  Infatti, possiamo scrivere $b = \text{MCD}(\alpha, n) \cdot c$ per qualche intero *c*.  Quindi, l'equazione diventa $ax \equiv \text{MCD}(\alpha, n) \cdot c \pmod{n}$.  Poiché $\text{MCD}(\alpha, n)$ divide sia $\alpha$ che *n*, possiamo dividere entrambi i lati per $\text{MCD}(\alpha, n)$ (modulo *n*) e ottenere una soluzione per *x*.  In conclusione, l'equazione $aX = b$ in $\mathbb{Z}/n\mathbb{Z}$ ammette soluzioni se e solo se $\text{MCD}(\alpha, n) \mid \beta$.

> [!info] Lemma
> 
> Siano $a, b, c \in \mathbb{Z}$. Se $a \mid c$ e $b \mid c$ e $\text{MCD}(a, b) = 1$, allora $ab \mid c$.

# Teorema Cinese dei Resti

Poniamo $r_{1},\dots,r_{s} \in \mathbb{N}$ e supponiamo $MCD(r_{i}, r_{j})=1\, \forall r_{i} \not = r_{j}$ (ossia sono a due a due coprimi).

Consideriamo inoltre $c_{1},\dots,c_{s} \in \mathbb{Z}$

Allora il sistema
$$
(*)
\begin{cases}
x \equiv c_{1} \text{ mod }r_{1} \\
x \equiv c_{2} \text{ mod }r_{2} \\
\text{ }\vdots \\
x \equiv c_{S} \text{ mod }r_{s}
\end{cases}
$$
ha un'unica soluzione modulo $R := r_{1}*r_{2}*\dots*r_{s}$ ovvero l'insieme $\varepsilon_{*} = \{ x \text{ soluzione in } \mathbb{Z} \text{ di } (*) \}$ è $x_0 + R\mathbb{Z}$

## Esempi

Per risolvere questo sistema abbiamo bisogno anzitutto di verificare la validità delle singole equazioni, assicurandoci che ognuna ammetta soluzione, ovvero che:
$$
\begin{align}
& a,b \in \mathbb{Z}, r \in \mathbb{N} \\
& ax \equiv b \text{ (mod } r \text{) ammette soluzione se} \\
& MCD(a,r) | b
\end{align}
$$
Verificata questa condizione, andiamo a ridurre il nostro sistema affinché $a = 1$, come vedremo nell'esempio.

Infine, per calcolare le soluzioni "principali" del nostro sistema, andiamo a calcolare $mcm(r_{1},\dots,r_{n})$, che sarà il "limite" a cui dovremmo stare nella ricerca della soluzione comune. Essendo i moduli coprimi tra loro, possiamo semplicemente considerare il prodotto $r_{1}*\dots*r_{n}$ come limite essendo questo il loro $mcm$.

> [!warning] Attenzione
> Questo esempio suppone che $MCD(r_{i},r_{j})=1 \text{ con } r_{i}\not=r_{j}$, ovvero che $r_{i},r_{j}$ siano coprimi tra loro. Nel caso non lo siano, è essenziale calcolare correttamente il $mcm$, che non sarà la semplice produttoria cui sopra.

Vediamo un esempio:

$$
\begin{align}
& \begin{cases}
2x \equiv 7 \text{ (mod }5 \text{)} \\
3x \equiv 8 \text{ (mod }4\text{)}
\end{cases} \\
&  \\
& MCD(2,5) = 1,\, 1 \mid 7 \implies \text{ammette soluzione} \\
& MCD (3,4) = 1,\, 1 \mid 8 \implies \text{ammette soluzione} \\
&  \\
& -------------------- \\
& \\
& x = \frac{5k + 7}{2} \implies \begin{cases}
k=0 \implies x=\frac{7}{2} \not \in \mathbb{N} \\
k=1 \implies x = \frac{12}{2} = 6 \in \mathbb{N}
\end{cases} \\
& x = \frac{4k+8}{3} \implies \begin{cases}
k=0 \implies x = \frac{8}{3} \not \in \mathbb{N} \\
k=1 \implies x = \frac{12}{3} = 4 \in \mathbb{N}
\end{cases} \\ \\
& \begin{cases}
x \equiv 6 \text{ (mod }5 \text{)} \\
x \equiv 4 \text{ (mod }4 \text{)}
\end{cases} \\ \\
& -------------------- \\ \\
& mcm(5,4) = 20 \\ \\
& x = 5k+6 \implies 6,11,16,\dots \\
& x = 4k+4 \implies 4,8,12,16,20,\dots \\ \\
& \text{Pertanto la soluzione del sistema è } [16]_{20} \\ \\
& \blacksquare 
\end{align}
$$

## Sistema Omogeneo Associato

Si dice **sistema omogeneo associato** un sistema di congruenze della forma:

$$
*_{(H)} \begin{cases}
x \equiv 0 \text{ mod } r_{1} \\
x \equiv 0 \text{ mod } r_{2} \\
\vdots \\
x \equiv 0 \text{ mod } r_{s}
\end{cases}
$$

Quali sono le soluzioni di questo sistema?
$$
\begin{align}
x \equiv_{r_{1}} 0 \iff r_{1} \mid x \\
x \equiv_{r_{2}} 0 \iff r_{2} \mid x
\end{align}
$$
Ma $r_{1},r_{2}$ sono primi fra loro, quindi $r_{1}r_{2} \mid x$. Iterando, otteniamo che $R:=r_{1}\dots r_{s} \mid x$.
Quindi l'insieme delle soluzioni di $*_{(H)}$ è $\varepsilon_{H} = R\mathbb{Z}$ ossia l'insieme dei multipli di $R$.