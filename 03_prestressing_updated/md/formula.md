00

Das Dach einer Bushaltestelle mit einer Grundrissfläche von 20 x 35 m ist als Platte mit
obenliegenden in y-Richtung verlaufenden Querträgern und einem obenliegenden in xRichtung verlaufenden vorgespannten Hauptträger ausgebildet. Hauptträger und Stützen bilden zusammen einen über 20 m gespannten Zweigelenkrahmen mit beidseitigen Randüberständen von 7.5 m. 

====
01

Im Folgenden werden die Kennwerte der verwendeten Baumaterialien aufgezeigt.    

Beton\
C30/37\
$f_{cd} = 20\,\text{MPa}$\
$E_c = 33.6\,\text{GPa}$\
\
Spannstahl\
Y1860\
$A_p = 19.150\,\text{mm}^2$\
$f_{pk} = 1860\,\text{MPa}$\
$E_p = 195\,\text{GPa}$\
$c_{nom,p} = 50\,\text{mm}$


====
02

Zur Vorspannung des Hauptträgers wird ein symmetrisch aufgebautes Spanngliedsystem mit zwei Kabeln verwendet. 
Die verwendeten Spanngliedeinheiten sind die VSL 6-19 mit je 19 Litzen à 0.6“ der Festigkeitsklasse Y1860. Diese werden auf eine initiale Vorspannung von 0.75∙fpk vorgespannt werden. 
Um die Reibungsverluste auszugleichen wird ein Kabel von links (x = -17.5 m) und ein Kabel von rechts (x = 17.5 m) vorgespannt.

====
03

Hier ist der qualitative Momentenverlauf des Balkens gezeigt. Dieser wird benötigt, um die effektive Breite eines Plattenbalkens zu berechnen. 

====
04

Jetzt kann die effektive Breite des Trägers nach SIA 262 berechnet werden.


$l_0 = 0.7 \cdot L = 14\,\text{m}$\
$b_{\text{eff},i} = 0.2 \cdot b_f + 0.1 \cdot l_0 = 3.3\,\text{m} \leq 0.2 \cdot l_0 \Rightarrow b_{\text{eff},i} = 0.2 \cdot l_0 = 2.8\,\text{m}$\
$b_{\text{eff}} = 2 \cdot b_{\text{eff},i} + b_w = 6.6\,\text{m}$\

====
05

Mit der effektiven Breite des Trägers, kann man die effektiven Querschnittswerte berechnen. In diesem Beispiel wird nur die effektive Breite des Innenfelds berücksichtigt, da die Steifigkeit der Randüberstände nicht benötigt wird für die Berechnung der Zwangsschnittgrößen. 


$A_b = h \cdot b_w + 2 \cdot t \cdot b_eff,i = 2.544 \text{m}^2$\
$\zeta _1 = \frac{h}{2} = 600 \text{mm}, \zeta _2 = \frac{t}{2} + \frac{6}{95} \cdot \frac{b_eff,i}{2} = 208.4 \text{mm}$\
$\zeta_c = \frac{h \cdot b_w \cdot s_1 + 2 \cdot t \cdot b_{\text{eff},i} \cdot s_2}{A_b} = 393.1\,\text{mm}$\
$I_b = \frac{h^3 b_w}{12} + 2 \cdot \frac{b_{\text{eff},i} \cdot t^3}{12} + b_w \cdot h \cdot (\zeta _1 - \zeta_c)^2 + 2 \cdot b_{\text{eff},i} \cdot t \cdot (\zeta_c - \zeta _2)^2 = 0.2477\,\text{m}^4$

====
06

Die Kabelgeometrie orientiert sich ungefähr am Momentenverlauf des Trägers. Für die genauere Berechnung des Verlaufs, sind die folgenden Herstellerangaben ausschlaggebend:  

- Spanngliedeinheit VSL 6-19 Y1860, $A_p = 19.150\,\text{mm}^2 = 2850\,\text{mm}^2$
- Rundes Stahlhüllrohr 90/97 (Øᵢ = 90 mm, Øₐ = 97 mm, Δs = 12 mm)

- Min. Radius: $R_{\text{min}} = k \cdot \sqrt{P_{pk}\,[\text{MN}]} = 3 \cdot \sqrt{A_p f_{pk}\,[\text{MN}]} = 6.9\,\text{m}$

- Minimaler Randabstand der Verankerung EC 30:

    $R_4 = \frac{X}{2} + c_{\text{nom},p} - 10 = 270\,\text{mm}$\
    $X = 460\,\text{mm}$\

- Minimaler Randabstand auf freier Länge:

    $R_F = c_{\text{nom},p} + \frac{97\,\text{mm}}{2} + 12\,\text{mm} = 111\,\text{mm}$

====
07

Die Berechnung der Kabelgeometrie erfolgt anhand der Herstellerangaben des Trägers und der Trägergeometrie. 

Randfeld: 

$k = 0$\
$f_0 = h - \zeta_c - R_F = 696\,\text{mm}$\
$l = a = 7500\,\text{mm}$\
$b = \frac{2 R_{\text{min}} \cdot f_0}{a} = 1281\,\text{mm}$\
$c = \frac{2 R_{\text{min}} \cdot f_0^2}{a^2} = 119\,\text{mm}$\
$f = \frac{f_0 \cdot l^2}{4 \left(a^2 - 2 R_{\text{min}} \cdot f_0 \right)} = 210\,\text{mm}$\

Innenfeld: 

$F_0 = h - 2 R_F = 978\,\text{mm}$\
$L = 20000\,\text{mm}$\
$B = \frac{4 R_{\text{min}} \cdot F_0}{L} = 1350\,\text{mm}$\
$C = \frac{8 R_{\text{min}} \cdot F_0^2}{L^2} = 132\,\text{mm}$\
$F = \frac{F_0 \cdot L^2}{L^2 - 8 R_{\text{min}} \cdot F_0} = 1131\,\text{mm}$\

Die Umlenkkräfte im Randfeld $u = \frac{8 \cdot P\cdot f}{l^2} = \frac{P}{33.5 \text{m}}$ sind etwas grösser als diejenigen im Mittelfeld $u = \frac{8 \cdot P\cdot f}{l^2} = \frac{P}{44.2 \text{m}}$.

====
08

Die Spannkraft reduziert sich über den Verlauf des Kabels. Dies liegt an Verlusten durch Reibung und den Keileinzug. \
Verluste infolge Reibung: $\mu = 0.18,\Delta \phi = 5 \text{mrad/m}$



$\delta \varphi_x = \frac{2 \left| e_j - e_{j-1} \right|}{x_j - x_{j-1}}$\
$\varphi_x = \sum \delta \varphi_x$\
$P(x) = P_{\text{max}} \cdot e^{-\mu (\varphi_x + \Delta \varphi \cdot x)}$\
$P_{\text{max}} = 0.75 \, A_p f_{pk} = 3976\,\text{kN}$

Für die genaue Berechnung der Spannkraftverluste, siehe Musterlösung der Hausübung 2. 

Am passiven Ende verbleiben nach Abzug der Reibungsverluste knapp 74% der maximalen Spannkraft am
aktiven Ende.

====
09

Verluste infolge Keileinzug: $\Delta = 6 \text{mm}$ \
Der Keileinzug beeinflusst das aktive Ende bis über den ersten Wendepunkt des Spannglieds.\

$\Delta P = 2 \left( l_1 \frac{dP_1}{dx} + l_2 \frac{dP_2}{dx} \right)$\
$\Delta P_2 = 2 \cdot l_2 \cdot \frac{dP_2}{dx}$\
$\Delta = \frac{l_1 \left( \Delta P + \Delta P_2 \right)}{2 E_p A_p} + \frac{l_2 \cdot \Delta P_2}{2 E_p A_p} \overset{!}{=} 6\,\text{mm}$

Aus den drei Gleichungen mit den Unbekannten $l_2$, $\Delta P$ und $\Delta P_2$ folgt:

$l_2 = 1.70 \text{m}$\
$\Delta P = 643 \text{kN}$\
$\Delta P_2 = 339 \text{kN}$

$\frac{\Delta P_2}{dx}$ entspricht der gemittelten Änderung der Vorspannkraft zwischen dem ersten ud zweiten Wendepunkt. 

====
10

Verlauf der Vorspannkraft für Kabel A. \
Der Verlauf des Kabel B ist gespiegelt bezüglich x = 17.5m. Aus der Superposition der beiden
Spannkrafverläufe resultiert die tatsächliche Vorspannkraft in jedem Querschnitt. 

Bei der Verankerung:  
$P = 3333\,\text{kN} + 2928\,\text{kN} = 6261\,\text{kN}$

In Feldmitte:  
$P = 2 \cdot 3412\,\text{kN} = 6824\,\text{kN}$

Über den Stützen:  
$P = 3612\,\text{kN} + 3151\,\text{kN} = 6765\,\text{kN}$

---

Die Spannkräfte wurden hier zwischen den Wendepunkten gemittelt. Vergleicht man die Spannkraft über der Stütze bei $x = 27{,}5\,\text{m}$ mit dem exakten Wert aus der Tabelle auf S. 4 der Musterlösung, wird ersichtlich, dass der Unterschied marginal ist.

====
11

Hier sieht man das Gesamtsystem inklusive der zwei Vorspannkabel, welche wir in der Hausübung 2 bemessen haben. 
