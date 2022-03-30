[TOC]



Lineare Algebra
1. Algebraische Strukturen
1.1 Gruppen
1.2 Ringe
1.3 Körper
1.4 Vektorräume
2. Grundbegriffe der Linearen Algebra
2.1 Erzeugendensystem
2.2 Lineare Unabhängigkeit
2.3 Austauschsatz
2.4 Basen
2.5 Dimension
3. Hilberträume
3.1 Skalarprodukt
3.2 Zusammenhang mit normierten Räumen
3.3 Projektion und ihre Anwendungen
3.4 Orthogonalität
4. Lineare Abbildungen
4.1 Linearität
4.2 Lösen von Gleichungen
4.3 Situation in endlich dimensionalen Räumen
5. Determinanten
5.1 Permutationen
5.2 Definition
5.3 Eigenschaften
5.4 Der Entwicklungssatz von Laplace
5.5 Vandermonde Determinante
5.6 Determinantenmultiplikationssatz
5.7 Ableiten von Determinanten
6. Diagonalisierung
6.1 Ähnlichkeit
6.2 Diagonalisierung
6.3 Eigenwerte und Eigenvektoren
6.4 Matrixpotenzen und ihre Anwendungen
6.5 Transitionsmatrizen
6.6 Quadratische Formen
6.7 Abschließende Bemerkungen7. Der Satz von Hamilton-Cayley
7.1 Formulierung und Beweis
7.2 Berechnung von Eigenvektoren
7.3 Berechnung von Matrixpotenzen
7.4 Berechnung von Transitionsmatrizen
7.5 Adjunktenformel
8. Die Jordansche Normalform
8.1 Hauptvektoren
8.2 Übergang zur JNF
8.3 Das Minimalpolynom
8.4 Matrixpotenzen
8.5 Transitionsmatrizen











# ——————— A N A L Y S I S ———————



# 1. Grundlagen



## 1.1 Notationen

| Quantoren                                | Zahlenmengen                             | Sonstige                            |
| ---------------------------------------- | ---------------------------------------- | ----------------------------------- |
| $\exists,~\lor$  es gibt                 | $\N$  natürlich,    $\N_0$  nat. + 0     | #  Anzahl                           |
| $\exists_1,~\dot\lor$  es gibt genau ein | $\Z$  ganze,    $\Q$  rationale          | q.e.d. / w.w.w.w.w  Ende Herleitung |
| $\forall, \land$  für alle               | $\R$  reelle,    $\R^+$  positive reelle |                                     |
|                                          | $\C$  komplexe                           |                                     |



## 1.2 [Vollständige Induktion](https://youtu.be/z4PmJ5rC4jA)

$$
A(n):\quad \overset{linke~Seite}{L(n)}=\overset{rechte~Seite}{R(n)}\qquad \forall~n\in\N
$$

| Induktions-                |                 | zu tun                         |                                                  |
| -------------------------- | --------------- | ------------------------------ | ------------------------------------------------ |
| a) Anfang                  | n=1             | $A(n=1)$                       | kleinste natürliche Zahl                         |
| b) Vorraussetzung          | $\exist~n\in\N$ | $L(n)=R(n)$                    | es gibt eine natürliche Zahl, für Annahme stimmt |
| c) Behauptung / zu zeigen: |                 | $A(n+1):\quad L(n+1)=R(n+1)$   | gilt für alle n                                  |
| d) Schritt                 | $1→n\\n→n+1$    | $L(n+1)=L(n)+…\\R(n+1)=R(n)+…$ |                                                  |



## 1.5 Normen

$$
||A·\vec x||_V\le||A||·||\vec x||_V
$$

|             | Vektor                              | Matrix                                                       | Funktion |
| ----------- | ----------------------------------- | ------------------------------------------------------------ | -------- |
|             | $\vec x = \pmatrix{x_1\\x_2}$       | $A=\pmatrix{a&b\\c&d}$                                       | $f(x)$   |
|             |                                     | $\parallel A\cdot B\parallel~\le~\parallel A\parallel\cdot\parallel B\parallel$ |          |
| Allgemein   | $||x||_p=\sqrt[p]{\sum_i|x_i|^p}$   | $\displaystyle\parallel A\parallel_p=\left(\sum_{i=1}^m\sum_{j=1}^n\vert a_{ij}\vert^p\right)$ |          |
| "Manhatten" | $||x||_1=|x_1|+|x_2|$               | Spaltensummennorm<br />$||A||_1=\max\big\{|a|+|c|,~|b|+|d|\big\}$ |          |
| "Euklid"    | $||x||_2=\sqrt{{x_1}^2+{x_2}^2}$    | $\displaystyle\parallel A\parallel_p=\left(\sum_{i=1}^m\sum_{j=1}^n\vert a_{ij}\vert^p\right)$ |          |
| unendlich   | $||x||_\infty=\max\{|x_1|,~|x_2|\}$ |                                                              |          |
| F           |                                     |                                                              |          |



1.6 Matrixnormen
1.7 Relationen
1.8 Mächtigkeit von Mengen
2. Reelle und komplexe Folgen
2.1 Grenzwerte
2.2 Eigenschaften konvergenter Folgen
2.3 Monotone Folgen
2.4 Häufungswerte
2.5 Vollständigkeit
3. Unendliche Reihen
3.1 Grundlagen
3.2 Reihen mit nicht-negativen Gliedern
3.3 Integralkriterium
3.4 Alternierende Reihen
3.5 Absolute Konvergenz
3.6 Unbedingte Konvergenz
3.7 Geometrische Reihe
4. Differentialrechnung
4.1 Grenzwerte von Funktionen
4.2 Stetigkeit
4.3 Eindimensionale Differenzierbarkeit
4.4 Satz von Taylor
4.5 Mehrdimensionale Differenzierbarkeit
4.6 Landau-Symbole
5. Riemann-Integral
5.1 Definition
5.2 Riemannsches Integrabilitätskriterium
5.3 Hauptsatz der DI
5.4 Praktische Bestimmung des Integrals
5.5 Ausblick aufs Lebesgue-Integral
6. Potenzreihen
6.1 Einführendes Beispiel
6.2 Gleichmäßige Konvergenz
6.3 Satz von Cauchy-Hadamard
6.4 Identitätssatz
6.5 Reihenmultiplikation7. Lineare Differentialgleichungen mit variablen Koeffizienten
7.1 Potenzreihenansatz
7.2 Frobenius
7.3 Reduktion nach d'Alembert
7.4 Variation der Konstanten
7.5 Iteratives Lösen von DGln
8. Komplexe Analysis
8.1 Komplexe Differenzierbarkeit
8.2 Komplexe Integration
8.3 Integralsatz von Cauchy
8.4 Cauchysche Integralformeln
8.5 Potenzreihenentwicklungen
8.6 Der Fundamentalsatz der Algebra
8.7 Laurentreihenentwicklungen
8.8 Residuen
8.9 Residuensatz
8.A Berechnung reeller Integrale
8.B Inverse z-Transformation
8.C Inverse Laplace-Transformation
9. Iterationsfolgen
9.1 Einführendes Beispiel
9.2 Banachscher Fixpunktsatz
9.3 Beispiele
9.4 Chaos
A. Distributionen
A.1 Grundlagen
A.2 Integraldarstellung
A.3 Lineare Transformationen
A.4 Multiplikation mit einer Funktion
A.5 Funktionale Ableitung
A.6 Funktionaler Grenzwert
A.7 Fouriertransformation





# ——————— S T A T I S T I K ———————

1. Verteilungen für gedächtnislose Vorgänge
    1.1 Poisson-Prozesse
    1.2 Poisson-Verteilung
    1.3 Exponentialverteilung

# 2. Erzeugende Funktionen

> diskret

2.1 Definition und Beispiele

| Allgemein             | Diskrete Verteilung                       | Binomialverteilung             | Poisson                                 |
| --------------------- | ----------------------------------------- | ------------------------------ | --------------------------------------- |
| $P_X$                 | $\array{X&0&1&2\\\hline f_X&p_1&p_2&p_3}$ | $P(X=k)=\binom nk·p^k·q^{n-k}$ | $P_X=\dfrac{\lambda^k}{k!}e^{-\lambda}$ |
| $g_X(z)=\sum_kP_Xz^k$ | $g_X(z)=p_1z^0+p_2z^1+p_3z^2$             | $g_X(z)=(pz+q)^n$              | $g_X(z)=e^{\lambda(z-1)}$               |

2.2 Bestimmung von Parametern
2.3 Der Poissonschen Grenzwertsatzes
2.4 Addition von unabhängigen Zufallsvariablen

# 3. Charakteristische Funktionen

> stetig	

3.1 Definition und Beispiele

$f_{X+Y}=f_X\circledast f_Y  -- \varphi_X(t)\cdot\varphi_Y(t)$

| Zufallsvariable | Dichte                          | Charakteristische Funktion                                   |
| --------------- | ------------------------------- | ------------------------------------------------------------ |
| $X$             | $f_X(x)=\sum_iP_i\delta(x-x_i)$ | $\varphi_X(t)=\int f_X(x)·e^{jtx}~dx\\=\sum_{i=-\infty}^\infty P_ie^{jtx_i}\underset{x_i=i}=g_X(e^{jt})$    (inverse Fourier Transformation) |

|                | Exponentialverteilung                                   | Normalverteilung                            | ==a, b durch mü, sigma ersetzen==<br />Normalverteilung Allgemein  $a>0$ |
| -------------- | ------------------------------------------------------- | ------------------------------------------- | ------------------------------------------------------------ |
| Verteilung     | $F_X(x)=(1-e^{-\frac x\alpha})·\varepsilon(x)$          | $f_X(x)=\dfrac1{\sqrt2\pi}e^{-\frac{x^2}2}$ | $F_{aX+b}=F_X(\frac{x-b}a)$                                  |
| Dichte         | $f_X(x)=\dfrac1\alpha e^{-\frac x\alpha}\varepsilon(x)$ |                                             | $f_{aX+b}=\dfrac1a·f_X(\frac{x-b}a)$                         |
| Char. Fkt.     | $\varphi_X(t)=\dfrac1{1-jtx}$                           | $\varphi_X(t)=e^{-\frac{t^2}2}$             | $\varphi_{aX+b}(t)=\varphi_X(at)·e^{jtb}$                    |
| Erwartungswert |                                                         |                                             | $E(aX+b)=a·E(X)+b$                                           |
| Varianz        |                                                         |                                             | $Var(aX+b)=a^2·Var(X)$                                       |

3.2 Lineare Variablen-Transformation
3.3 Anwendung auf Normalverteilung
3.4 Bestimmung von Parametern
3.5 Addition von unabhängigen Zufallsvariablen

1. Grenzwertsätze
    4.1 Tschebyschewsche Ungleichung
    4.2 Die Gesetze der Großen Zahl
    4.3 Zentraler Grenzwertsatz
    4.4 Visualisierung der Grenzwertsätze
5. Stochastische Prozesse
5.1 Einführendes Beispiel
5.2 Grundbegriffe
5.3 Erwartungswerte 1. Ordnung
5.4 Erwartungswerte 2. Ordnung
5.5 Stationarität und Ergodizität
5.6 Spektraldarstellung
5.7 Übertragung von stochastischen Prozessen
