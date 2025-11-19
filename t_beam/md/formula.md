
00
Das dargestellte System besteht aus mehreren Plattenbalken nebeneinander. Diese überspannen als einfache Balken 16 m. 

Baustoffe: 
$$\text{Beton C25/30} \rightarrow f_{cd} = 16.5 \text{ MPa}$$
$$\text{Betonstahl B500B} \rightarrow f_{sd} = 435 \text{ MPa}$$
$$c_{nom} = 30 \text{ mm}$$

====
01

Zusätzlich zum Eigengewicht wirken eine Auflast $$g_{a,k} = 1 \text{kN}/\text{m}^2$$ und eine Nutzlast von $$q_{k} = 3 \text{kN}/\text{m}^2$$

====
02

Die Platte spannt in Querrichtung als Durchlaufträger zwischen den Balken. 

Einwirkungen: 

$$g_k = 0.18 \cdot 25 = 4,5 \text{ kN/m}^2$$
$$g_{a,k} = 1 \text{ kN/m}^2$$
$$q_k = 3 \text{ kN/m}^2$$

Daraus resultierende Gesamtlast in Querrichtung: 
$$g_{d,Platte} + q_{d,Platte} = 1.35 \cdot (4.5+1)+1.5\cdot3 = 11.9 \text{ kN/m}^2$$

Daraus resultierendes Moment: 
$$\left| m_{d,tot} \right| = 11.9 \cdot 5.0^2 / 8 = 37.2 \text{ kN/m}^2$$

====
03

Für dieses Quermoment muss eine Biegebewehrung der Platte angeordnet werden. 

Als Bewehrung wird folgende gleichmäßige Plattenbewehrung gewählt:\
4 Lagen ⌀10/200, 1. und 4. Lage in Querrichtung, $c_{nom} = 30 \text{ mm}$

Der daraus resultierende Widerstand berechnet sich wie folgt:

$$m_{Rd}^+ = a_s \cdot f_{sd} \cdot (d-\frac{a_s\cdot f_{sd}}{2\cdot f_{sd}}) = 393 \cdot 435 \cdot (145 - \frac{393\cdot 435}{2\cdot 1'000 \cdot 16.5}) = 23.9 \text{kNm/m}$$


$$m_{Rd,erf}^{-} = \left| m_{d,\text{tot}} \right| - m_{Rd}^{+} = 37.2 - 23.9 = 13.3\,\text{kNm/m}$$

Bemerkung:\
$m_{Rd}^- = m_{Rd}^+$, aber:\
Die obere Querbewehrung muss neben dem negativen Moment auch den Querzug aus dem Schubanschluss aufnehmen\
$\rightarrow$ Superposition der Kräfte ergibt erforderliche Bewehrung (siehe später)


====
04

In Längsrichtung wird ein einzelner Balken als Ausschnitt aus der Decke betrachtet.\
In Längsrichtung ergeben sich die folgenden Einwirkungen:

$$g_d + q_d = 5.00 \cdot (g_{d,Platte} + q_{d,Platte}) = 1.35 \cdot 0.4 \cdot 1.02 \cdot 25 = 73.4 \text{kN/m}$$
$$\rightarrow M_d = 73.4 \cdot 16^2/8 = 2'349 \text{ kNm}$$
$$(\rightarrow V_d = 73.4 \cdot 16/2 = 587 \text{ kN})$$

====
05

Für diesen muss zunächst die mittragende Plattenbreite bestimmt werden.\
Die mittragende Plattenbreite berechnet sich wie folgt nach SIA 262:\
$$b_{eff,1} = b_{eff,2} = 0.2 b_1 + 0.1 l_0 = 0.2 \cdot 2.3 + 0.1 \cdot16 = 2.06\text{ m}$$
$$b_{eff} = \Sigma b_{eff,i} + b_w = 2 \cdot 2.06 + 0.4 = 4.52 \text{ m}(< b = 5.00 \text{ m})$$

====
06

Hier dargestellt ist das zugehörige Fachwerkmodell für Steg und Flansch.

====
07

Für die Berechnung des Biegewiderstands wird die erforderliche Längsbewehrung geschätzt.  
$$d \approx 1'100 \text{ mm (Annahme: 2 Lagen Längsbewehrung)}$$
$$z \approx 0.95 \cdot d \approx 1'050 \text{ mm (0.95 anstatt 0.9 da bei Plattenbalken die Druckzone breiter ist)}$$
$$A_{s,erf} = \frac{M_d}{z\cdot f_{sd}} = \frac{2'349\cdot10^6}{1'050\cdot435} = 5'140 \text{ mm}^2 \rightarrow 7\text{⌀}30 \text{=} 4'950 \text{ mm}^2$$

Daraus ergibt sich als effektiver Biegewiderstand: 

$$d = 1'200 - \frac{5\cdot55 + 2\cdot115}{7} = 1'128 \text{ mm}$$
$$M_{Rd} = A_s \cdot f_{sd}(d-\frac{A_s \cdot f_{sd}}{2 \cdot b_{eff} \cdot f_{cd}}) = 4'950 \cdot 435 \cdot (1'128 - \frac{4'950 \cdot 435}{2 \cdot 4'250 \cdot 16.5}) = 2'398 \text{ kNm} \geq M_d = 2'349 \text{ kNm}$$

====
08

Zur Sicherstellung der Querkrafttragsicherheit wird eine Bügelbewehrung Ø8@125 gewählt, dies ergibt sich aus der Mindestbewehrung nach SIA 262. 

$$\rho _{min} = 0.2 \%$$
$$a_{s,min} = \rho _{min} \cdot b_w = 0.002 \cdot 400 \text{ mm} \cdot 1'000 \text{ mm/m} = 800 \text{ mm}^2\text{/m}$$
$$\rightarrow 2\text{Ø8@125, } a_s = 2 \cdot 402 = 804 \text{ mm}^2\text{/m (2-schnittig)}$$

====
09

Die notwendige Querbewehrung der Platte ergibt sich als Überlagerung aus der Beanspruchung durch Querbiegemoment und Ausbreitung der Flanschdruckkräfte, denn daraus ergibt sich eine Querzugkraft, welche mit dem Querbiegemoment superponiert werden muss. (Für eine genaue Berechnung siehe Vorlesung 3.4 Querkraft)

Die Gleichgewichtsbedingungen am Schnittkörperdiagramm liefern die Druckkraft und die Kraft in der vierten Bewehrungslage: 

$$a_s \sigma _{s,IV} = 566.1 \text{ kN/m}$$

gewählt: 

$$a_s \cdot f_{sd} = \frac{16^2*\pi}{4 \cdot 0.15} \cdot 0.435 = 583 \text{ kN/m} > 566.1 \text{ kN/m, i.O.}$$

Die ursprünglich gewählte Plattenbewehrung von Ø10@200 reicht nicht aus, um die Kräfte aus Querbiegung und Querzug aufzunehmen. Sie wird
auf Ø16@150 ($a_s = 1’340 \text{mm}^2$/m) verstärkt.

====
10

Zusätzliche konstruktive Mindestbewehrung wird in Längsrichtung angeordnet. 

====
11

Es ergibt sich der dargestellte Bewehrungskorb.
