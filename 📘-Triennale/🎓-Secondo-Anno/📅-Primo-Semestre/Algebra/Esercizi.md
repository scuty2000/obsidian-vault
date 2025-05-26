# Settimana 1, es. 1

> Determinare il grafico della corrispondenza tra $X := \{ 1,2,3,4 \}$ ed $Y := \{ 1,3,5 \}$ definita nella seguente maniera:
> $$
 x \text{ "è minore o uguale a" } y
 $$

Stiamo quindi considerando la corrispondenza $\mathcal{C} = (X,Y,\Gamma)$ per cui:
$$
\begin{align}
& X = \{ 1,2,3,4 \} \\
& Y = \{ 1,3,5 \} \\
& \Gamma \subset X \times Y = \{ (x,y) : (x \in X, y \in Y) \land x \leq y \} \\
\end{align}
$$

Determiniamo le coppie del prodotto cartesiano $X \times Y$:
$$
X \times Y = \{ (1,1), (1,3), (1,5), (2,1), (2,3), (2,5), (3,1), (3,3), (3,5), (4,1), (4,3), (4,5) \}
$$
Ed applichiamo la seconda condizione dell'appartenenza al grafo della corrispondenza $\mathcal{C}$:
$$
\Gamma = \{ (1,1), (1,3), (1,5), (2,3), (2,5), (3,3), (3,5), (4,5) \}
$$
$\blacksquare$

# Settimana 1, es. 7

> Dire quale delle seguenti relazioni è antisimmetrica:
> 	a) $x \text{ è minore o uguale } y$
> 	b) $x \text{ è minore } y$
> 	c) $x + 2y = 10$
> 	d) $x \text{ divide } y$

Intuitivamente, possiamo escludere _b)_ e _d)_ dai nostri ragionamenti, in quanto sappiamo che queste relazioni non possono essere antisimmetriche.

Altrettanto intuitivamente, possiamo dire che _a)_ è antisimmetrica, in quanto $x \leq y \land y \leq x \implies x = y$.

Per _c)_ invece possiamo ragionare come segue:
$$
\begin{cases}
x + 2y = 10 \\
y + 2x = 10
\end{cases}
\iff
\begin{cases}
x = 10 - 2y \\
y + 2x = 10
\end{cases}
\implies
y + 2(10-2y) = 10 \implies y + 20 -4y = 10 \implies 3y = 10 \implies y = \frac{10}{3} \implies x = 10 - 2(\frac{10}{3}) \implies x = 10 - \frac{20}{3} \implies x = \frac{10}{3}
$$
Ottenendo quindi che:
$$
\begin{cases}
x = \frac{10}{3} \\
y = \frac{10}{3}
\end{cases}
$$
pertanto $x \mathrel{\mathcal{R}} y \implies y \mathrel{\mathcal{R}} x \iff x = y$ ed è quindi antisimmetrica.

Sono quindi _a)_ e _c)_ le relazioni antisimmetriche.

$\blacksquare$

# Settimana 1, es 20

> **Definizione costruttiva di** $\mathbb{Q}$ **a partire da** $\mathbb{Z}$
> Definiamo in $\mathbb{Z} \times \mathbb{N^*}$ (dove $\mathbb{N^*} = \mathbb{N} \setminus \{ 0 \}$) la relazione
> $$(m,n) \sim (m',n') \iff mn' = nm'$$
> a) Verificare che $\sim$ è una relazione di equivalenza;
> b) Verificare che le coppie del tipo $(m,n) \in \mathbb{Z} \times \mathbb{N^*}$, con $m$ ed $n$ primi tra loro, sono un insieme di rappresentanti per le classi di $\sim \text{-equivalenza}$.

## Punto a)

Per verificare che la relazione proposta sia una relazione di equivalenza, dobbiamo verificare le tre condizioni necessarie e sufficienti: riflessività, simmetria, transitività.

### Riflessività

Per ogni $(m,n) \in \mathbb{Z} \times \mathbb{N^*}$:
$$
(m,n) \sim (m,n) \iff mn = nm
$$
Che è sempre vera. Pertanto la relazione $\sim$ è riflessiva.

### Simmetria

Dobbiamo verificare che $(m,n) \sim (m',n') = (m',n') \sim (m,n)$

$$
\begin{cases}
(m,n) \sim (m',n') \iff mn' = nm'\\
(m',n') \sim (m,n) \iff m'n = n'm
\end{cases}
$$

Possiamo intuitivamente constatare che la relazione è simmetrica.

### Transitività

Siano
$$
(m,n) \sim (m',n') \text{ e } (m',n') \sim (m'', n'')
$$
Vale quindi:
$$
\begin{cases}
mn' = nm' \\
m'n'' = n'm''
\end{cases}
$$
Moltiplichiamo (1) per $n''$ e (2) per $n$
$$
\begin{cases}
nm'n'' = mn'n'' \\
nm'n'' = nn'm''
\end{cases}
$$
Essendo i membri sinistri uguali, uguagliamo i membri sinistri:
$$
mn'n'' = nn'm'' \implies mn'' = nm'' \implies (m,n) \sim (m'',n'')
$$
Pertanto la relazione $\sim$ è transitiva.

### Conclusione

Essendo la relazione $\sim$ riflessiva, simmetrica e transitiva possiamo constatare è una relazione d'equivalenza.

## Punto b

