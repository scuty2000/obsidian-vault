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

# Settimana 5

## es 8 foglio 3

$$
\begin{align}
& \text{Trovare tutti gli interi } x \in \mathbb{Z} \text{ che soddisfino} \\
& \text{(i) } 4x \equiv 7 \text{ (mod }15 \text{)} \\
& \text{(ii) } 6x \equiv 8 \text{ (mod }9 \text{)} \\
& \text{(iii) } \begin{cases}
1025x \equiv 5312065 \text{ (mod }8 \text{)} \\
36x \equiv 322 \text{ (mod }5 \text{)} \\
4x \equiv 7 \text{ (mod }3 \text{)}
\end{cases} \\
& \text{(iv) } 4x \equiv 3 \text{ (mod }385 \text{)}
\end{align}
$$

### (i)

$$
\begin{align}
& 4x \equiv 7 \text{ (mod }15 \text{)} \\ \\
& \text{Verifichiamo che ammetta soluzione:} \\
& MCD(4,15) = 1,\, 1 \mid 7 \implies \text{ammette soluzione} \\ \\
& \text{Cerchiamo ora l'inverso di } 4 \text{ in modo da portare } 4x \text{ a } 1x \text{:} \\
& \exists n \in \mathbb{Z} : 4 *n \equiv_{15} 1 \text{ (es. 4)} \\ \\
& \text{Trasformo } 4x \text{ in } 1x \text{ moltiplicando per 4 a destra e sinistra:} \\
& 4*4x \equiv_{15} 7*4 \implies x \equiv_{15} 28 \implies x \equiv_{15} 13 \\
& \text{Le soluzioni sono quindi } \varepsilon = 15\mathbb{Z} + 13 \text{ (ovvero i multipli di 15 con resto 13)}
\end{align}
$$

### (ii)

$$
\begin{align}
& 6x \equiv_{9} 8 \\
& MCD (9,6) = 3,\, 3 \not \mid 8 \implies \text{ non ammette soluzione}
\end{align}
$$

### (iii)

$$
\begin{align}
& \begin{cases}
1025x \equiv 5312065 \text{ (mod }8 \text{)} \\
36x \equiv 322 \text{ (mod }5 \text{)} \\
4x \equiv 7 \text{ (mod }3 \text{)}
\end{cases} \\
& ------------- \\
& MCD(8,5) = MCD(8,3) = MCD(5,3) = 1,\, 1 \mid 5312065,322,7 \implies \text{ ammette soluzione} \\
& ------------- \\
& \text{Semplifichiamo le equazioni:} \\ \\
& \text{1 sinistra) } 1025 \implies 1024 + 1 \implies (1024 \equiv_{8} 0) + 1 \implies 1 \pmod{8} \\
& \text{1 destra) } \begin{cases}
5312065 \text{ per questo sono cazzi amari.} \\
8 \mid 56 \implies 8 \mid 5600000 \implies 5312065 \equiv_{8} -287935 \\
8 \mid 290000 \implies -287935 \equiv_{8} 2065 \\
8 \mid 2048 \implies 2065 \equiv_{8} 17 \\
8 \mid 16 \implies 17 \equiv_{8} 1
\end{cases} \\
& \text{ invece di questo bordello immane basta usare i criteri di divisibilità:}  \\
& 8 \mid 5312064 \implies 5312065 \equiv_{8} 1 \\
& ------------- \\
& \text{2 sinistra) } 36 = 35 + 1 \implies (35 \equiv_{5} 0) + 1 = 1 \\
& \text{2 destra) } 322 = 320 + 2 \implies (320 \equiv_{5} 0) + 2 = 2 \\
& ------------- \\
& \text{3 sinistra) } 4 = 3 +1 = (3 \equiv_{3} 0) + 1 = 1 \\
& \text{3 destra) } 7 = 6 + 1 = (6 \equiv_{3} 0) + 1 = 1 \\
& ------------- \\ \\
& \text{Ora il sistema è:} \\
& \begin{cases}
x \equiv 1 \pmod{8} \\
x \equiv 2 \pmod{5} \\
x \equiv 1 \pmod{3}
\end{cases} \\ \\
& \text{Troviamo } R:= mcm(8,5,3) = 120 \\
& x = 8k +1 \implies 1,9,17,25,33,41,49,57,65,73,81,89,97,105,113 \\
& x = 5k +2 \implies 2,7,12,17,22,27,32,37,42,47,52,57,62,67,72,77,82,87,92,97,102,107,112,117 \\
& x = 3k + 1 \implies 4,7,10,13,16,19,22,25,28,31,34,37,40,43,46,49,52,55,58,61,64,67,70,73,76,79,82,85,88,91,94,97,100,104,107,110,113,116,119 \\ \\
& \text{Quindi la soluzione particolare è } 97, \text{ mentre quella generale è } \varepsilon = 120\mathbb{Z} + 97
\end{align}
$$

