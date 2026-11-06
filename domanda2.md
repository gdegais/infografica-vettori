# Analisi Aerodinamica dei Diruttori (Freni Aerodinamici) e della Polare del Velivolo

## 1. Che cosa sono i diruttori e come modificano la polare

I **diruttori** (o _airbrakes_ / freni aerodinamici) sono superfici mobili azionate dal pilota per aumentare deliberatamente la resistenza aerodinamica del velivolo senza alterare in modo significativo la portanza generata. Vengono impiegati per:

- Aumentare l'angolo di discesa (pendenza della rampa) in fase di avvicinamento e atterraggio senza incrementare la velocità.
    
- Limitare la velocità massima in picchiata (_candela_ o volo verticale).
    
- Ridurre la corsa di atterraggio dopo il contatto con il suolo.
    

### Modifica del modello della polare parabolica

La polare di un velivolo in configurazione pulita è descritta dall'equazione parabolica:

$$C_D = C_{D0} + K C_L^2$$

dove:

- $C_{D0}$ è il coefficiente di resistenza parassita a portanza nulla.
    
- $K$ è il fattore di resistenza indotta ($K = \frac{1}{\pi A e}$, con $A$ allungamento alare ed $e$ fattore di Oswald).
    

Quando i diruttori vengono estesi, essi provocano una separazione controllata della vena fluida e un incremento della resistenza di pressione. Questo si traduce in un aumento della resistenza a portanza nulla, mentre l'incremento sul fattore indotto $K$ è generalmente trascurabile o secondario. La nuova polare diventa:

$$C'_D(C_L) = C'_{D0} + K C_L^2$$

avendo posto:

$$C'_{D0} = C_{D0} + \Delta C_D$$

dove $\Delta C_D > 0$ è il contributo addizionale fornito dai diruttori.

## 2. Variazione delle grandezze caratteristiche in funzione di $C'_{D0}$

### A. Efficienza Massima ($E_{\max}$)

L'efficienza aerodinamica è definita come il rapporto tra portanza e resistenza:

$$E = \frac{L}{D} = \frac{C_L}{C_D}$$

Per una polare parabolica, l'efficienza massima si ottiene quando la resistenza parassita eguaglia la resistenza indotta ($C_{D0} = K C_L^2$). Il suo valore è:

$$E_{\max} = \frac{1}{2 \sqrt{K C_{D0}}}$$

Con l'inserimento dei diruttori, sostituendo $C_{D0}$ con $C'_{D0}$, la nuova efficienza massima $E'_{\max}$ diventa:

$$E'_{\max} = \frac{1}{2 \sqrt{K C'_{D0}}} = E_{\max} \sqrt{\frac{C_{D0}}{C'_{D0}}}$$

Poiché $C'_{D0} > C_{D0}$, il rapporto $\frac{C_{D0}}{C'_{D0}} < 1$, dimostrando che **l'efficienza massima diminuisce** all'aumentare di $C'_{D0}$.

### B. Angolo di Rampa Minimo ($\gamma_{\min}$)

In volo librato o in discesa a motore ridotto, l'angolo di rampa $\gamma$ è legato all'efficienza dalla relazione:

$$\sin(\gamma) \approx \gamma = \frac{D}{L} = \frac{1}{E}$$

L'angolo di rampa minimo corrisponde al punto di massima efficienza:

$$\sin(\gamma_{\min}) = \frac{1}{E_{\max}}$$

Con i diruttori inseriti, il nuovo angolo di rampa minimo $\gamma'_{\min}$ risulta:

$$\sin(\gamma'_{\min}) = \frac{1}{E'_{\max}} = \frac{1}{E_{\max}} \sqrt{\frac{C'_{D0}}{C_{D0}}}$$

Poiché $\sqrt{\frac{C'_{D0}}{C_{D0}}} > 1$, **l'angolo di rampa aumenta sensibilmente** ($\gamma'_{\min} > \gamma_{\min}$), permettendo al velivolo di perdere quota più rapidamente a parità di velocità orizzontale.

### C. Velocità Limite in Candela ($V_{\lim}$)

In una picchiata verticale pura (candela), la spinta è nulla o trascurabile e il velivolo raggiunge una velocità limite $V_{\lim}$ quando la resistenza aerodinamica eguaglia esattamente il peso ($W = D$):

$$W = \frac{1}{2} \rho V_{\lim}^2 S C_D$$

Poiché in volo verticale il coefficiente di portanza $C_L \approx 0$, la resistenza coincide con quella a portanza nulla ($C_D = C'_{D0}$). Esplicitando la velocità limite:

$$V_{\lim} = \sqrt{\frac{2W}{\rho S C'_{D0}}}$$

La dipendenza da $C'_{D0}$ è inversamente proporzionale alla radice quadrata:

$$V_{\lim} \propto \frac{1}{\sqrt{C'_{D0}}}$$

All'aumentare di $C'_{D0}$ tramite l'apertura dei diruttori, **la velocità limite in candela diminuisce drasticamente**, impedendo al velivolo di fuoriuscire dai limiti strutturali di velocità Vne (_Velocity Never Exceed_).

## 3. Perché bastano superfici di pochi decimi di metro quadrato?

La resistenza generata da un corpo aerodinamico è espressa dalla formula:

$$D = q \cdot S_{\text{rif}} \cdot C_D$$

dove $q = \frac{1}{2} \rho V^2$ è la **pressione dinamica**.

Nei velivoli moderni (specialmente a quote medio-alte o in fase di discesa ad alta velocità), la pressione dinamica $q$ è elevatissima a causa della velocità $V$ elevata ($q \propto V^2$). Di conseguenza:

1. Anche se la superficie geometrica dei diruttori ($S_{\text{dir}}$) è piccola (pochi decimi di metro quadrato rispetto ai metri quadri dell'ala), il coefficiente di resistenza locale della piastra investita è molto alto ($C_{D,\text{piastra}} \approx 1.2 - 2.0$).
    
2. Il contributo adimensionale globale sulla polare è dato da:
    
    $$\Delta C_D = \frac{S_{\text{dir}}}{S_{\text{ala}}} \cdot C_{D,\text{piastra}}$$
    
    Pur avendo un rapporto di superficie $\frac{S_{\text{dir}}}{S_{\text{ala}}}$ piccolo (es. 0.02 - 0.05), il prodotto con l'elevata resistenza di forma della piastra genera un incremento $\Delta C_D$ considerevole.
    
3. Inoltre, i diruttori perturbano il flusso sulla parte posteriore dell'ala, incrementando ulteriormente la resistenza parassita complessiva.
    

## 4. Cosa accade se il nuovo assetto ottimo $C^{*'}_L$ supera $C_{L,\max}$?

Il coefficiente di portanza ottimale per ottenere l'efficienza massima con i diruttori inseriti è:

$$C^{*'}_L = \sqrt{\frac{C'_{D0}}{K}}$$

Poiché $C'_{D0} > C_{D0}$, il valore di $C^{*'}_L$ richiesto per volare alla massima efficienza con i freni inseriti è **maggiore** del $C^{*}_L$ in configurazione pulita.

Se l'incremento di resistenza parassita $\Delta C_D$ è talmente elevato da spingere il valore teorico di $C^{*'}_L$ **al di sopra del coefficiente di portanza massimo dell'ala ($C_{L,\max}$)**, si verificano importanti conseguenze operative:

- **Impossibilità fisica di raggiungere l'ottimo:** Il velivolo entrerebbe in stallo (_stall_) prima di poter raggiungere l'angolo d'attacco corrispondente a quel $C^{*'}_L$.
    
- **Limitazione operativa:** Il pilota non può volare alla velocità di efficienza massima teorica calcolata con i diruttori aperti, ma è costretto a mantenere un coefficiente di portanza inferiore ($C_L \le C_{L,\max}$), accettando un compromesso aerodinamico in cui la portanza massima disponibile vincola la manovrabilità e la gestione della discesa.