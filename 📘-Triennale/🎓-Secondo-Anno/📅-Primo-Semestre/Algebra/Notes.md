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

