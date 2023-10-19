url: https://tutorial.math.lamar.edu/Problems/CalcI/Functions.aspx

# 1. Évaluer des fonctions

## 1.(i) Évaluer $f(x) = 3-5x - 2x^2$

### 1.(i).a) Pour $f(4)$

$$
\begin{aligned}
f(4) &= 3 - 5*4 - 2*4*4 \\ 
    &= 3 - 20 - 32 \\
    &= -17 - 32 \\
    &= -49 \\
\end{aligned}
$$

### 1.(i). b) Pour $f(0)$

$$
\begin{align}
f(0) &= 3 - 5*0 - 2*0*0 \\
    &= 3 - 0 - 0 \\
    &= 3 - 0 \\
    &= 3
\end{align}
$$

### 1.(i). c) Pour $f(-3)$

$$
\begin{align}
f(-3) &= 3 - 5*(-3) - 2 *(-3) * (-3) \\
    &= 3 - (-15) - 2*9 \\
    &= 3 + 15 - 18 \\
    &= 18 - 18 \\
    &= 0
\end{align}
$$

### 1.(i). d) Pour $f(6-t)$

$$
\begin{align}
f(6 - t) &= 3 - 5 * (6-t) - 2 * (6-t)^2 \\
        &= 3 - 5*6 + 5t - 2* (6^2 - 2*6*t + t^2) \\
        &= 3 - 30 + 5t - 2* (36 - 12t + t^2) \\
        &= -27 + 5t - 2*36 + 2*12t - 2*t^2 \\
        &= - 2*t^2 + 5t + 2*12t - 27 - 2*36 \\
        &= -2t^2 + 5t + 24t - 27 - 72 \\
        &= -2t^2 + 29t - 99 
\end{align}
$$

J'ai eu quelques erreurs de calculs dans la résolution de celle-ci (oubli de la multiplication par deux du $(6-t)^2$)

### 1.(i). e) Pour $f(7-4x)$

$$
\begin{align}
f(7-4x) &= 3 - 5*(7 - 4x) - 2 * (7 - 4x)^2 \\
       &= 3 - 5*7 + 5*4x - 2*(7^2 - 2*7*4x + (4x)^2) \\
       &= 3 - 35 + 20x - 2*(49 - 14*4x + 16x^2) \\
       &= -32 + 20x - 2*49 + 2*56x - 2*16x^2 \\
       &= -2*16x^2 - 32 - 2*49 + 20x + 2*56x \\
       &= -32x^2 - 32 - 98 + 20x + 112x \\
       &= -32x^2 - 130 + 132x \\
       &= -32x^2 + 132x - 130 \\
\end{align}
$$

J'ai oublié de prendre en compte le signe du deux au "$+16x^2$" dans la même sous-opération qu'au précédent exercice.

### 1.(i). d) Pour $f(x+h)$

$$
\begin{align}
f(x+h) &= 3 - 5*(x+h) - 2*(x+h)^2 \\
      &= 3 - 5*x - 5*h - 2*(x^2 + 2xh + h^2) \\
      &= 3 - 5x - 5h - 2*x^2 - 4xh - 2h^2 \\
      &= -2x^2 - 2h^2 - 4hx - 5x - 5h + 3 \\
\end{align}
$$

## 1.(ii) Évaluer $g(t) = \frac{t}{2t+6}$

### 1.(ii).a) Pour $g(0)$

$$
\begin{align}
g(0) &= \frac{0}{2*0 + 6} \\
    &= \frac{0}{6} \\
    &= 0
\end{align}
$$

### 1.(ii).b) Pour $g(-3)$

$$
\begin{align}
g(-3) &= \frac{-3}{2 * (-3) + 6*} \\
     &= \frac{-3}{-6 + 6} \\
     &= \frac{-3}{0} \\
g(-3) &\rightarrow \text{n'existe pas}
\end{align}
$$

### 1.(ii).c) Pour $g(10)$

$$
\begin{align}
g(10) &= \frac{10}{2*10 + 6} \\
     &= \frac{10}{20 + 6} \\
     &= \frac{10}{26} \\
     &= \frac{5}{13}
\end{align}
$$

### 1.(ii).d) Pour $g(x^2)$

$$
\begin{align}
g(x^2) &= \frac{x^2}{2*x^2 + 6}
	  &= \frac{x^2}{2x^2 + 6}
\end{align}
$$

### 1.(ii).e) Pour $g(t + h)$

$$
\begin{align}
g(t+h) &= \frac{(t+h)}{2*(t+h) + 6} \\
      &= \frac{t+h}{2t + 2h + 6} \\
\end{align}
$$

### 1.(ii).f) Pour $g(t^2 - 3t + 1)$

$$
\begin{align}
g(t^2 - 3t + 1) &= \frac{(t^2 - 3t + 1)}{2*(t^2 - 3t + 1) + 6} \\
               &= \frac{t^2 - 3t + 1}{2t^2 - 6t + 2 + 6}\\
               &= \frac{t^2 - 3t + 1}{2t^2 - 6t + 8} \\
\end{align}
$$

Mon premier résultat était faux. J'essayais de simplifier la fraction de manière erronée et j'obtenais $\frac{1}{8}$ :

$$
\begin{align}
g(t^2 - 3t + 1) &= \frac{(t^2 - 3t + 1)}{2*(t^2 - 3t + 1) + 6} \\
               &= \frac{t^2 - 3t + 1}{2t^2 - 6t + 2 + 6}\\
               &= \frac{t^2 - 3t + 1}{2t^2 - 6t + 8} \\
               &= \frac{1}{2 - 2 + 8} \\
               &= \frac{1}{0 + 8} \\
               &= \frac{1}{8}
\end{align}
$$

## 1.(iii) Évaluer $h(z) = \sqrt{1  - z^2}$

### 1.(iii).a) Pour $h(0)$

$$
\begin{align}
h(0) &= \sqrt{1 - 0^2} \\
    &= \sqrt(1 - 0) \\
    &= \sqrt{1} \\
    &= 1
\end{align}
$$

### 1.(iii).b) Pour $h(-\frac{1}{2})$

$$
\begin{align}
h(-\frac{1}{2}) &= \sqrt{1 - (-\frac{1}{2})^2} \\
               &= \sqrt{1 - (\frac{1}{4})} \\
               &= \sqrt{\frac{3}{4}} \\
               &= \frac{\sqrt{3}}{\sqrt{4}} \\
               &= \frac{\sqrt{3}}{2}
\end{align}
$$

Il me manquait apparemment les deux dernières étapes de simplification

### 1.(iii).c) Pour $h(\frac{1}{2})$

$$
\begin{align}
h(\frac{1}{2}) &= \sqrt{(1 - (\frac{1}{2})^2} \\
              &= \sqrt{1 - (\frac{1}{4})} \\
              &= \sqrt{\frac{3}{4}} \\
              &= \frac{\sqrt{3}}{\sqrt{4}} \\
              &= \frac{\sqrt{3}}{2}
\end{align}
$$

### 1.(iii).d) Pour $h(9z)$

$$
\begin{align}
h(9z) &= \sqrt{1 - (9z)^2} \\
     &= \sqrt{1 - 81z^2}
\end{align}
$$

### 1.(iii).e) Pour $h(z^2 - 2z)$

$$
\begin{align}
h(z^2 - 2z) &= \sqrt{1 - (z^2 - 2z)^2} \\
           &= \sqrt{1 - ((z^2)^2 - 2*(z^2)*(2z) + (2z)^2)} \\
           &= \sqrt{1 - (z^4 - 2*z^2*2z + 4z^2)} \\
           &= \sqrt{1 - (z^4 - 2z^2*2z + 4z^2)} \\
           &= \sqrt{1 - z^4 + 2z^2*2z - 4z^2} \\
           &= \sqrt{-z^4 - 4z^2 + 2z^2*2z + 1} \\
           &= \sqrt{-z^4 - 4z^2 + 4z^3 + 1} \\
           &= \sqrt{-z^4 + 4z^3 - 4z^2 + 1}
\end{align}
$$

J'ai eu un souci : j'ai fait une multiplication par deux au dernier terme de l'espansion de l'[[Identité Remarquable]] ($(a-b)^2 \rightarrow a^2 - 2ab + 2b^2$).

J'avais aussi fait une erreur de signe, en oubliant le "moins" du "$1 - z$"".

### 1.(iii).f) Pour $h(z+k)$

$$
\begin{align}
h(z+k) &= \sqrt{1 - (z + k)^2} \\
      &= \sqrt{1 - (z^2 + 2zk + k^2)} \\
      &= \sqrt{1 - z^2 - 2zk - k^2}
\end{align}
$$

## 1.(iv) Évaluer $R(x) = $\sqrt{3 + x} - \frac{4}{x+1}$

### 1.(iv).a) Pour $R(0)$

$$
\begin{align}
R(0) &= \sqrt{3 + 0} - \frac{4}{0+1} \\
    &= \sqrt{3} - \frac{4}{1} \\
    &= \sqrt{3} - 4
\end{align}
$$

### 1.(iv).b) Pour $R(6)$

$$
\begin{align}
R(6) &= \sqrt{3 + 6} - \frac{4}{6 + 1} \\
    &= \sqrt{9} - \frac{4}{7} \\
    &= 3 - \frac{4}{7} \\
    &= \frac{21 - 4}{7} \\
    &= \frac{17}{7}
\end{align}
$$

J'ai fait une simple erreur au début : $6+1 \rightarrow 7$...

### 1.(iv).c) Pour $R(-9)$

$$
\begin{align}
R(-9) &= \sqrt{3 + (-9)} - \frac{4}{-9 + 1} \\
     &= \sqrt{3 - 9} - \frac{4}{-8} \\
     &= \sqrt{-6} + \frac{4}{8} \\
     &= \sqrt{-6} + \frac{1}{2} \\
R(-9) &\rightarrow \text{n'existe pas (racine d'un nombre negatif)}
\end{align}
$$

### 1.(iv).d) Pour $R(x+1)$

$$
\begin{align}
R(x+1) &= \sqrt{3 + (x + 1)} - \frac{4}{(x+1) + 1} \\
      &= \sqrt{3 + 1 + x} - \frac{4}{x + 1 + 1} \\
      &= \sqrt{4 + x} - \frac{4}{x + 2} \\
\end{align}
$$

### 1.(iv).e) Pour $R(x^4 - 3)$

$$
\begin{align}
R(x^4 - 3) &= \sqrt{3 + (x^4 - 3)} - \frac{4}{(x^4 - 3) + 1} \\
          &= \sqrt{3 + x^4 - 3} - \frac{4}{x^4 - 3 + 1} \\
          &= \sqrt{x^4} - \frac{4}{x^4 - 2} \\
          &= x^2 - \frac{4}{x^4 - 2}
\end{align}
$$

### 1.(iv).f) Pour $R(\frac{1}{x} - 1)$

$$
\begin{align}
R(\frac{1}{x} - 1) &= \sqrt{3 + (\frac{1}{x} - 1)} - \frac{4}{(\frac{1}{x} - 1) + 1} \\
                  &= \sqrt{3 - 1 + \frac{1}{x}} - \frac{4}{\frac{1}{x} - 1 + 1} \\
                  &= \sqrt{2 + \frac{1}{x}} - \frac{4}{\frac{1}{x}} \\
                  &= \sqrt{\frac{2x + 1}{x}} - \frac{4}{1} * \frac{x}{1} \\
                  &= \sqrt{\frac{2x + 1}{x}} - \frac{4x}{1} \\
                  &= \sqrt{\frac{2x + 1}{x}} - 4x
\end{align}
$$

La solution officielle est un tout petit peu différente, ne créant simplement pas l'écriture fractionnaire de la racine que j'ai choisie ($\frac{2x+1}{x}$) mais gardant la forme $2 + \frac{1}{x}$.

# 2. Évaluer le [[Quotient Différentiel]] de différentes fonctions

## 2.(i) Évaluer le quotient différentiel de $f(x) = 4x - 9$

$$
\begin{align}
quotient(f(x)) &= \frac{(4*(x+h) - 9) - (4x - 9)}{h} \\
              &= \frac{4x + 4h - 9 - 4x + 9}{h} \\
              &= \frac{4x - 4x + 9 - 9 + 4h}{h} \\
              &= \frac{4h}{h}\\
              &= 4
\end{align}
$$

## 2.(ii) Évaluer le quotient différentiel de $g(x) = 6 - x^2$

$$
\begin{align}
quotient(g(x)) &= \frac{(6 - (x + h)^2) - (6 - x^2)}{h} \\
              &= \frac{(6 - (x^2 + 2xh + h^2)) - 6 + x^2}{h} \\
              &= \frac{(6 - x^2 - 2xh - h^2) - 6 + x^2}{h} \\
              &= \frac{6 - x^2 - 2xh - h^2 - 6 + x^2}{h} \\
              &= \frac{x^2 - x^2 - 2xh - h^2 + 6 - 6}{h} \\
              &= \frac{-2xh - h^2}{h} \\
              &= -2x - h
\end{align}
$$

## 2.(iii) Évaluer le quotient différentiel de $f(t) = 2t^2 - 3t + 9$

$$
\begin{align}
quotient(f(t)) &= \frac{(2(t+h)^2 - 3(t+h) + 9) - (2t^2 - 3t + 9)}{h} \\
              &= \frac{(2(t^2 + 2th + h^2) - 3t + 3h + 9) - 2t^2 + 3t - 9}{h} \\
              &= \frac{2t^2 + 4th + 2h^2 - 3t - 3h + 9 - 2t^2 + 3t - 9}{h} \\
              &= \frac{2t^2 - 2t^2 + 3t - 3t + 9 - 9 - + 2h^2 + 4th -3h}{h} \\
              &= \frac{2h^2 + 4th - 3h}{h} \\
              &= 2h + 4t - 3
\end{align}
$$

J'ai oublié de distribuer l'identité remarquable la première fois...

## 2.(iv) Évaluer le quotient différentiel de $y(z) = \frac{1}{z + 2}$

$$
\begin{align}
quotient(y(z)) &= \frac{\frac{1}{z+h+2} - \frac{1}{z+2}}{h} \\
              &= \frac{\frac{z+2 - z+h+2}{(z+h+2) * (z+2)}}{h} \\
              &= \frac{\frac{z - z + 2 - 2 -h}{z^2 + 2z + zh + 2h +2z + 4}}{h} \\
              &= \frac{\frac{-h}{z^2 + 2z + 2z + zh + 4}}{h} \\
              &= \frac{-\frac{h}{z^2 + 4z + zh + 4}}{h} \\
              &= - \frac{\frac{h}{z^2 + 4z + zh + 4}}{h} \\
              &= - \frac{1}{z^2 + 4z + zh + 4} \\
              
\end{align}
$$

J'avais oublié comment additionner/soustraire deux fractions avec des dénominateurs différents (multiplication de chacune par le dénominateur de l'autre),

Aussi, le dénominateur du résultat était resté sous forme factorisée ($(z+h+2)(z+2)$) dans le résultat officiel.

## 2.(v) Évaluer le quotient différentiel de $A(t) = \frac{2t}{3 - t}$

$$
\begin{align}
quotient(A(t)) &= \frac{\frac{2(t+h)}{3-(t+h)} - \frac{2t}{3-t}}{h} \\
              &= \frac{\frac{2t+2h}{3-t-h} - \frac{2t}{3-t}}{h} \\
              &= \frac{\frac{(2t+2h)(3-t) - 2t(3-t-h)}{(3-t-h)(3-t)}}{h} \\
              &= \frac{\frac{2t*3 - 2t*t + 2h*3 - 2h*t - 2t*3 + 2t*t + 2t*h}{(3-t-h)(3-t)}}{h} \\
              &= \frac{\frac{6t - 2t^2 + 6h - 2ht - 6t + 2t^2 + 2ht}{(3-t-h)(3-t)}}{h} \\
              &= \frac{\frac{2t^2 - 2t^2 + 6t - 6t + 2ht - 2ht + 6h}{(3-t-h)(3-t)}}{h} \\
              &= \frac{\frac{6h}{(3-t-h)(3-t)}}{h} \\
              &= \frac{6}{(3-t-h)(3-t)}
\end{align}
$$

# 3. Déterminer des racines de fonctions

## 3.(i) Déterminer les racines de $f(x) = x^5 - 4x^4 - 32x^3$

Réécrivons $f(x)$ :

$$
\begin{align}
f(x) &= x^5 - 4x^4 - 32x^3 \\
    &= (x^3)(x^2 - 4x - 32)
\end{align}
$$

Selon la règle du produit nul, $f(x)$ possède donc 3 racines : celles de $x^3$ (une seule, qui est triviale : $x_1 = 0$) d'une part, et celles du polynôme $x^2 - 4x - 32$ d'autre part. Calculons le discriminant $\Delta$ de ce polynôme

$$
\begin{align}
\Delta &= (-4)^2 - 4*1*(-32) \\
      &= 16 + 128 \\
      &= 144
\end{align}
$$

$\Delta \gt 0$, donc le polynôme a deux racines $x_2$ et $x_3$ :

$$
\begin{align}
x_2 &= \frac{4 - \sqrt{144}}{2} \\
   &= \frac{4 - 12}{2}\\
   &= \frac{-8}{2} \\
   &= -4
\\ \\
x_3 &= \frac{4 + \sqrt{144}}{2} \\
   &= \frac{4 + 12}{2} \\
   &= \frac{16}{2} \\
   &= 8
\end{align}
$$

J'ai ajouté un négatif au $b^2$ dans la formule du discriminant la première fois (dont je ne me souvenais d'ailleurs plus trop).  
La solution officielle ne résous pas de [[Polynôme du Second Degré]]. À la place, elle poursuit la [[Factorisation]] de départ en obtenant $x^3(x - 8)(x + 4)$. Je n'ai pas remarqué cette possibilité lors de ma résolution

## 3.(ii) Déterminer les racines de $R(y) = 12y^2 + 11y -5$

$R(y)$ est un polynôme du second degré. Recherchons son discriminant $\Delta$ :

$$
\begin{align}
\Delta &= 11^2 - 4*12*(-5) \\
      &= 121 - 48*(-5) \\
      &= 121 + 240 \\
      &= 361
\end{align}
$$

On a $\Delta \gt 0$, donc on a deux racines $y_1$ et $y_2$ :

$$
\begin{align}
y_1 &= \frac{-11 - \sqrt{361}}{2*12} \\
   &= \frac{-11 - 19}{24} \\
   &= \frac{-30}{24} \\
   &= -\frac{30}{24} \\
   &= -\frac{15}{12} \\
   &= -\frac{5}{4}
\\ \\
y_2 &= \frac{-11 + \sqrt{361}}{2*12} \\
   &= \frac{-11 + 19}{24} \\
   &= \frac{8}{24} \\
   &= \frac{1}{3}
\end{align}
$$

Encore une fois, la version officielle ne résous pas de polynôme et se contente de factoriser vers $(4y+5)(3y-1)$.

## 3.(iii) Déterminer les racines de $h(t) = 18 - 3t -2t^2$

$h(t)$ est un polynôme du second degré. Calculons son déterminant $\Delta$ :

$$
\begin{align}
\Delta &= (-3)^2 - 4*18*(-2) \\
      &= 9 - 72*(-2) \\
      &= 9 + 144 \\
      &= 153
\end{align}
$$

On a $\Delta \gt 0$, donc $h(t)$ a 2 racines $t_1$ et $t_2$ :

$$
\begin{align}
t_1 &= \frac{3 - \sqrt{153}}{2*(-2)} \\
   &= \frac{3 - 3\sqrt{17}}{-4} \\
   &= -\frac{3 - 3\sqrt{17}}{4}  \\
   &= -\frac{3}{4} (1 - \sqrt{17}) \\
\\ \\
t_2 &= \frac{3 + \sqrt{153}}{2*(-2)} \\
   &= \frac{3 + 3\sqrt{17}}{-4} \\
   &= -\frac{3 + 3\sqrt{17}}{4} \\
   &= -\frac{3}{4} (1 + \sqrt{17})
\end{align}
$$

## 3.(iv) Déterminer les racines de $g(x) = x^3 + 7x^2 - x$

On réécrit :

$$
  
g(x) = x(x^2+7x-x)
$$

On a 0 comme solution triviale $x_1$ (par la [[Règle du Produit Nul]]). Cherchons le discriminant $\Delta$ du polynôme en deuxième terme :

$$
\begin{align}
\Delta &= 7^2 - 4*1*(-1) \\
      &= 49 + 4 \\
      &= 53
\end{align}
$$

On a $\Delta \gt 0$, donc on a deux autres racines $x_2$ et $x_3$ :

$$
\begin{align}
x_2 &= \frac{-7 - \sqrt{53}}{2} \\
\\ \\
x_3 &= \frac{-7 + \sqrt{53}}{2}
\end{align}
$$

Petite erreur d'inatention au début (mais en même temps je suis fatiguée) : $49+4 \rightarrow 43$
