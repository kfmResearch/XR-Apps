00 

Die Deckenplatte des in Bild 1 dargestellten Unterstellplatzes ist ausser durch ihre Eigenlast,
mit einer $h_b = 200 \text{mm}$ dicken Erdauflast und einer Schneelast gemäss Norm SIA 261
(Standort: Glarus, 550 m ü. M.) beansprucht. Die Platte weist eine Dicke von $h_P = 240 \text{mm}$,
eine Länge von $l_P = 9 \text{m}$ sowie eine Breite von $b_P = 5.5  \text{m}$ auf. Auf einer Längsseite ist die
Platte auf einer Wandscheibe einfach gelagert, auf der gegenüberliegenden Seite auf drei
symmetrisch angeordneten Stützen gemäss Bild 1. Es soll ein Beton C 20/25 mit einem
Grösstkorn von Dmax = 32 mm verwendet werden, die Bewehrungsüberdeckung beträgt 30 mm.

====
01 

Im Folgenden werden die Kennwerte der verwendeten Baumaterialien aufgezeigt.    

Beton\
C20/25\
$f_{cd} = 13.5\,\text{MPa}$\
$f_{ctm} = 2.2\,\text{GPa}$\
$\tau_{cd} = 0.9\,\text{MPa}$\
$D_{max} = 32\,\text{mm}$\
$c_{nom} = 30\,\text{mm}$\
\
Bewehrung\
B500B\
$f_{sd} = 435\,\text{MPa}$

====
02 

Für den Lastabtrag zu den Stützen werden versteckte Unterzüge mit einer Breite von 1 m eingeführt (graue Flächen).
Es kann frei gewählt werden, in welchem Verhältnis die Lasten abgetragen werden. In diesem Beispiel werden 70 % der Flächenlast in y-Richtung und 30 % in x-Richtung abgetragen.

Für die einfache Streifenmethode werden erst der Abtrag der Flächenlasten zu den Auflagern und Unterzügen berechnet (Schnitte A-A und C-C) und danach der Abtrag der Lasten der Unterzüge zu den Stützen berechnet (Schnitte B-B, D-D und E-E). 
Um die erweiterte Streifenmethode aufzuzeigen, werden noch die Flächenlasten über den Stützen zu Punktlasten umgewandelt.  

====
03 

Eigengewicht:
$$
g_{0,k} = h_p \cdot \gamma_c = 6\,\text{kN/m}^2
$$

Erdauflast:
$$
\gamma_b = 21\,\text{kN/m}^3
$$
$$
\Rightarrow g_{1,k} = h_b \cdot \gamma_b = 4.2\,\text{kN/m}^2 \quad \text{(Auflast)}
$$

Schneelast:
$$
q_{s,k} = \mu_i \cdot C_e \cdot C_T \cdot s_k
$$

$$
h_0 = 550\,\text{m} + 500\,\text{m}
$$

$$
s_k = \left[1 + \left(\frac{h_0}{350}\right)^2\right] \cdot 0.4\,\frac{\text{kN}}{\text{m}^2} = 4\,\frac{\text{kN}}{\text{m}^2}
$$

$$
\mu_i = 0.8
$$

$$
\Rightarrow q_{s,k} = 3.2\,\text{kN/m}^2 \quad \text{(Nutzlast)}
$$

d-Niveau:
$$
q_d = \gamma_G \cdot (g_{0,k} + g_{1,k}) + \gamma_Q \cdot q_{s,k} = 18.6\,\text{kN/m}^2
$$


====
04 

Im Folgendem gibt es einen Überblick über den Kraftfluss für die einfache
Streifenmethode. Wichtig ist, dass konsequent alle Kräfte in die Lager geleitet werden. Ein
möglicher Abtrag wird in der Folge skizziert und anschliessend durchgerechnet.

Als erstes wird die Belastung gemäss der gewählten Verteilung von 70% in y-
Richtung und 30% in x-Richtung in das Auflager und die versteckten Unterzüge
(Strongbands), die als indirekte Lager wirken, geleitet. 

====
05 

In der gewählten Modellvorstellung liegt der Strongband 3 (x - Richtung) auf den
Strongbands 1&2 auf. Auf ihn wirkt die Flächenlast gemäss dem Verteilschlüssel
($0.3 \cdot q_{d}$) sowie die Auflagerkraft aus dem Schnitt C-C mit umgekehrtem Vorzeichen
als Belastung: $q_c$.\
Das statische System des Schnitts B-B zeigt wiederum, wie die Belastung der Strongbands 1&2 ($q_{B,r}\text{ und }q_{B,m}$) berechnet werden.


====
06

Als Letztes werden die Strongbands in y-Richtung betrachtet. Sie erfahren ihren Anteil der Flächenlast (0.7 $q_{d}$), sowie Auflagerkräfte aus den Schnitten A-A und B-B.


====
07 

Die Schnitte A-A – E-E werden jetzt Schritt für Schritt durchgerechnet. Zuerst werden die Schnittkräfte aus Schnitt A-A mit der Kraftmethode ermittelt (siehe Musterlösung). Es handelt sich dabei um die elastischen Schnittgrössen, es wäre aber auch möglich, plastisch zu rechnen. Dabei werden die 1m breiten Strongbands als Punktauflager modelliert. 
Es resultieren folgende Schnittkräfte für die Annahme der strongbands als Punktauflager. 

====
08

Es resultieren folgende Schnittkräfte unter Berücksichtigung der versteckten Unterzüge als Flächenlager mit gleichmässiger Pressung:

Die Flächenlasten der Strongbands lassen sich jeweils direkt aus der Punktauflagerkraft und der Breite der Strongbands berechnen:

$$
q_{4,r} = \frac{(8.7 + 2.8)\,\text{kN/m}}{1\,\text{m}} = 11.5\,\text{kN/m}^2
$$

$$
q_{4,m} = \frac{2 \cdot 13.7\,\text{kN/m}}{1\,\text{m}} = 27.4\,\text{kN/m}^2
$$

Das maximale Moment über dem Mittelauflager unter Berücksichtigung der Flächenpressung kann wie folgt berechnet werden:

$$
q_{4,r} \cdot 1\,\text{m} \cdot l - 0.3 \cdot q_d \cdot \frac{(l + 0.5\,\text{m})^2}{2}
+ q_{4,m} \cdot \frac{(0.5\,\text{m})^2}{2} = -7.3\,\text{kN}
$$

====
09

Die Schnittkräfte im Schnitt C-C können wie folgt berechnet werden: 

$$
q_q = \frac{13\,\text{kN/m}^2 \cdot \frac{(5.5\,\text{m})^2}{2}}{5\,\text{m} \cdot 1\,\text{m}} = 39.3\,\text{kN/m}^2
$$

====
10

Die Schnittkräfte im Schnitt B-B können analog zum Schnitt A-A berechnet werden, wobei sie mit dem Faktor $r_{A \rightarrow B} = \frac{0.3 \cdot q_d + q_c}{0.3 \cdot q_d} = 8.0$
multipliziert werden müssen. Für die Auflagerkräfte $q_{B,r}$ und $q_{B,m}$ muss dann jeweils $q_c$ abgezogen werden, da diese Kraft über den Flächenauflagern nicht wirkt.

$$
q_{B,r} = r_{A \rightarrow B} \cdot q_{4,r} - q_c = 52.9\,\text{kN/m}^2
$$

$$
q_{B,m} = r_{A \rightarrow B} \cdot q_{4,m} - q_c = 180.4\,\text{kN/m}^2
$$

$$
v_{i,B} = r_{A \rightarrow B} \cdot v_{i,A}
$$

$$
m_{i,B} = r_{A \rightarrow B} \cdot m_{i,A}
$$


====
11

Analog zum Vorgehen in Schnitt B–B können für D–D die Schnitt- und Auflagerkräfte von Schnitt C–C mit dem Faktor
$r_{C \rightarrow D} = \frac{0.7 \cdot q_d + q_{A,r}}{0.7 \cdot q_d} = 1.88$
multipliziert werden.

Die resultierende Auflagerkraft $q_D$ berechnet sich zu:

$$
q_D = r_{C \rightarrow D} \cdot q_c + (q_{B,r} - q_{A,r}) = 115.5\,\text{kN/m}^2
$$

Die Schnittkräfte:

$$
v_{i,D} = r_{C \rightarrow D} \cdot v_{i,C}
$$

$$
m_{i,D} = r_{C \rightarrow D} \cdot m_{i,C}
$$

Die Position des Nullschnitts ist:

$$
x_0 = 3.02\,\text{m}
$$


====
12

Wiederum wird vom Schnitt C–C ausgegangen und mit dem Faktor 
$r_{C \rightarrow E} = \frac{0.7 \cdot q_d + q_{4,m}}{0.7 \cdot q_d} = 3.1$
multipliziert.

Die resultierende Auflagerkraft $q_E$ berechnet sich zu:

$$
q_E = r_{C \rightarrow E} \cdot q_c + (q_{B,m} - q_{4,m}) = 275.1\,\text{kN/m}^2
$$

Die Schnittgrößen transformieren sich zu:

$$
v_{i,E} = r_{C \rightarrow E} \cdot v_{i,C}
$$

$$
m_{i,E} = r_{C \rightarrow E} \cdot m_{i,C}
$$

Die Position des Nullschnitts ist:

$$
x_0 = 3.02\,\text{m}
$$

====
13

$$
f_{cd} = k_c \cdot f_{ck,0.95} \approx f_{ck,0.95} = 1.3 \cdot f_{cm} = 2.9\,\text{MPa}
$$

$$
m_r = \frac{b \cdot h^2}{6} \cdot f_{cd} = 27.5\,\text{kNm/m}
$$

$$
z \approx 0.8h \Rightarrow a_{s,\text{erf}} \approx \frac{m_r}{f_{sd} \cdot 0.8h} = 329\,\text{mm}^2/\text{m}
$$

$$
\text{Wahl: } \varnothing 10@200, \quad a_s = 390\,\text{mm}^2/\text{m}
$$

$$
\text{1./4. Lage in y-Richtung}
$$

$$
\text{2./3. Lage in x-Richtung}
$$

$$
\text{Statische Höhe: } \quad d_y = h - c_{\text{nom}} - \varnothing/2 = 205\,\text{mm}
$$

$$
d_x = h - c_{\text{nom}} - \varnothing/2 = 195\,\text{mm}
$$

$$
m_{Rd,y} = a_s f_{sd} \left( d_y - \frac{a_s f_{sd}}{2 b f_{cd}} \right) = 33.7\,\text{kNm/m} \quad \text{(1./4. Lage)}
$$

$$
m_{Rd,x} = a_s f_{sd} \left( d_x - \frac{a_s f_{sd}}{2 b f_{cd}} \right) = 32.0\,\text{kNm/m} \quad \text{(2./3. Lage)}
$$


====
14

Schnitt A–A

$$
m_d^+ = 6.1\,\text{kN} < m_{Rd,\min,x}
$$

$$
m_d^- = 7.3\,\text{kN} < m_{Rd,\min,x}
$$

$$
\Rightarrow \text{Mindestbewehrung reicht aus.}
$$

====
15

Schnitt C–C

$$
m_d^+ = 39.9\,\text{kN} \Rightarrow a_{s,\text{erf}} \approx \frac{m_d^+}{f_{sd} \cdot 0.8h} = 478\,\text{mm}^2/\text{m}
$$

$$
\text{Wahl: } \varnothing12@200, \quad a_s = 565\,\text{mm}^2/\text{m}, \quad m_{Rd} = 47.9\,\text{kN} > m_d^+
$$

====
16

Schnitt B–B

$$
m_d^+ = 48.9\,\text{kN} \quad \text{Wahl: } \varnothing12@200, \quad m_{Rd} = 45.7\,\text{kN} \approx m_d^+ \sim \text{i.O.}
$$

$$
m_d^- = 92.9\,\text{kN} \Rightarrow a_{s,\text{erf}} \approx \frac{m_d^-}{f_{sd} \cdot 0.8h} = 1112\,\text{mm}^2/\text{m}
$$

$$
\text{Wahl: Zulagen } 5 \times \varnothing10 + 5 \times \varnothing16, \quad a_s = 1398\,\text{mm}^2/\text{m}
$$

$$
d = h - c_{\text{nom}} - 12\,\text{mm} - 8\,\text{mm} = 190\,\text{mm}, \quad m_{Rd} = 101.8\,\text{kN} > m_d^-
$$


====
17

Schnitt D–D

$$
m_d^- = 14.4\,\text{kN} < m_{Rd,\min,y} = 33.7\,\text{kN}, \quad \text{die Bewehrung muss am Plattenrand voll verankert sein.}
$$

$$
m_d^+ = 75.2\,\text{kN} \Rightarrow a_{s,\text{erf}} \approx \frac{m_d^+}{f_{sd} \cdot 0.8h} = 900\,\text{mm}^2/\text{m}, \quad \text{die Hälfte davon muss verankert werden}
$$

$$
\text{Wahl: Zulagen } 5 \times \varnothing12, \quad a_s = (5 \times \varnothing10 + 5 \times \varnothing12) = 958\,\text{mm}^2/\text{m}
$$

$$
\text{Wahl Randbügel: } \varnothing12@200
$$

$$
d = 204\,\text{mm}, \quad m_{Rd} = 78.6\,\text{kN} > m_d^+
$$

====
18

Schnitt E–E

$$
m_d^- = 34.4\,\text{kN}, \quad \text{Wahl: Zulagen } 5 \times \varnothing10 \rightarrow \varnothing10@100, \quad a_s = 780\,\text{mm}^2/\text{m}, \quad m_{Rd} = 65.7\,\text{kN} > m_d^-
$$

$$
m_d^+ = 124.0\,\text{kN} \Rightarrow a_{s,\text{erf}} \approx \frac{m_d^+}{f_{sd} \cdot 0.8h} = 1485\,\text{mm}^2/\text{m}
$$

$$
\text{Wahl: } \varnothing14/16@100, \quad a_s = (5 \times \varnothing14 + 5 \times \varnothing16) = 1780\,\text{mm}^2/\text{m}
$$

$$
d = 202\,\text{mm}, \quad m_{Rd} = 134.2\,\text{kN} > m_d^+
$$

$$
\frac{x}{d} = 0.33 < 0.35 \Rightarrow \text{i.O. für sämtliche Schnitte!}
$$


====
19

Für die Querkrafttrag­sicherheit sind die Schnitte mit der größten Hauptquerkraft $\v_d$ in der Hauptrichtung $\varphi_0$ maßgebend.

Schnitt 1:
$$
v_{xd} = 87.2\,\text{kN/m}, \quad v_{yd} = 26.3\,\text{kN/m}
$$
$$
v_{0d} = \sqrt{v_{xd}^2 + v_{yd}^2} = 91.0\,\text{kN/m}
$$

Schnitt 2:
$$
v_{xd} = 10.9\,\text{kN/m}, \quad v_{yd} = 81.8\,\text{kN/m}
$$
$$
v_{0d} = \sqrt{v_{xd}^2 + v_{yd}^2} = 82.8\,\text{kN/m}
$$

Schnitt 3:
$$
v_{xd} = 10.9\,\text{kN/m}, \quad v_{yd} = 100.1\,\text{kN/m}
$$
$$
v_{0d} = \sqrt{v_{xd}^2 + v_{yd}^2} = 100.7\,\text{kN/m}
$$

Querkraftwiderstand einer Platte ohne Schubbewehrung:

$$
e_c = 1.5 \cdot \frac{f_{sd}}{E_s} = 3.18\% \quad \text{(Plastische Verformungen der Biegebewehrung nicht ausgeschlossen)}
$$

$$
d = d_s = d_{\text{min}} = 190\,\text{mm} \quad \text{(keine Aussparungen oder Einlagen)}
$$

$$
k_g = \frac{48}{16 + D_{\max}} = 1.0
$$

$$
k_d = \frac{1}{1 + e_c \cdot d \cdot k_g} = 0.62
$$


$$
v_{Rd} = k_d \cdot \tau_{cd} \cdot d = 107\,\text{kN/m} > v_{0d,\max} = 101\,\text{kN/m} \Rightarrow \text{i.O.}
$$

NB: Zusätzlich wäre eine Durchstanzbewehrung im Stützenbereich (konzentrierte Lasteinleitung) zu führen.  
Darauf wird hier verzichtet, näheres dazu in der Autographie 7.4 und Kolloquium 5.


====
20

Hier sieht man die gesamte Bewehrung der Platte.