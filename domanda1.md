# Analisi del Volo Planato di due Alianti a Pesi Differenti

## 1. Condizioni di Equilibrio e Angolo di Planata
Consideriamo un aliante in volo planato rettilineo e uniforme. Le forze agenti sul velivolo sono:
- Il peso $W$, diretto verticalmente verso il basso.
- La portanza $L$, ortogonale alla traiettoria.
- La resistenza aerodinamica $D$, parallela e opposta alla traiettoria.

Lungo gli assi parallelo e perpendicolare alla traiettoria, le equazioni di equilibrio statico sono:
$$L = W \cos \gamma$$
$$D = W \sin \gamma$$

Dividendo la seconda equazione per la prima, si ottiene il rapporto tra resistenza e portanza, che definisce l'angolo di planata $\gamma$:
$$\tan \gamma = \frac{D}{L} = \frac{C_D}{C_L}$$

Poiché i due alianti sono **geometricamente e aerodinamicamente identici** e volano allo **stesso assetto ($C_L$ identico)**, anche il coefficiente di resistenza $C_D$ e il rapporto $\frac{C_D}{C_L}$ sono identici. Di conseguenza, **l'angolo di planata $\gamma$ è lo stesso per entrambi** ($\gamma_1 = \gamma_2$).

---

## 2. Dimostrazione della Stessa Distanza Orizzontale
Nota la quota iniziale $h$ e l'angolo di planata $\gamma$, la distanza orizzontale percorsa $x$ rispetto alla massa d'aria è:
$$x = \frac{h}{\tan \gamma}$$

Poiché $h$ e $\tan \gamma$ sono identici per entrambi i velivoli, **i due alianti percorrono esattamente la stessa distanza orizzontale** ($x_1 = x_2$).

> **Nota fisica importante:** Geometricamente, la traiettoria (quota in funzione della distanza orizzontale) nello spazio **non dipende dal peso**, purché il coefficiente di portanza ($C_L$) sia lo stesso.

---

## 3. Velocità di Volo e Tempi di Volo ($t_2 / t_1$)
Dall'equazione della portanza ricaviamo la velocità di volo $V$:
$$L = \frac{1}{2} \rho V^2 S C_L = W \cos \gamma \implies V = \sqrt{\frac{2W}{\rho S C_L \cos \gamma}}$$

Dato che $W_2 > W_1$, la velocità del secondo aliante è maggiore:
$$V_2 > V_1 \quad \text{con} \quad \frac{V_2}{V_1} = \sqrt{\frac{W_2}{W_1}}$$

Il tempo di volo $t$ si calcola dividendo la distanza $x$ per la componente orizzontale della velocità ($V_x = V \cos \gamma$):
$$t = \frac{x}{V \cos \gamma}$$

Poiché $x$ e $\cos \gamma$ sono uguali ma $V_2 > V_1$, risulta $t_2 < t_1$: **l'aliante più pesante arriva per primo**.

Il rapporto tra i tempi di volo è:
$$\frac{t_2}{t_1} = \frac{V_1}{V_2} = \sqrt{\frac{W_1}{W_2}}$$

---

## 4. Discussione in Presenza di Vento Orizzontale
- **Aria calma o vento uniforme:** Per il principio di relatività galileiana, la fisica rispetto alla massa d'aria non cambia.
- **Vento orizzontale rispetto al suolo:**
  - *Vento frontale (headwind):* Poiché l'aliante più leggero impiega più tempo ($t_1 > t_2$), il vento frontale agisce su di esso più a lungo, arrestandolo maggiormente rispetto al suolo. **L'aliante più pesante percorrerà una distanza maggiore al suolo**.
  - *Vento in coda (tailwind):* Il vento in coda spinge maggiormente l'aliante più lento ($W_1$), riducendo il divario rispetto al suolo.