---
title: Fonctions réelles
date: '2025-05-15'
type: book
weight: 30
math: true
tags:
  - Analyse
  - Fonctions réelles
---

Introduction à l'analyse (partie II).

<!--more-->

## Introduction aux fonctions d'une variable réelle

Les fonctions permettent de modéliser et étudier divers phénomènes, issus de la biologie, de la physique, des sciences économiques et sociales... Elle peuvent par exemple modéliser l'évolution du stock de livre d'une médiathèque chaque mois (le temps est discret) ou modéliser des températures et des marées (le temps est continu).

On appelle <mark>courbe représentative</mark> de la fonction $f$, l'ensemble des points M du plan de coordonnées $(x,y)$ qui vérifient l'équation $y = f(x)$. On dit dans ce cas que le point M appartient à la courbe représentative de f.

On appelle <mark>image</mark> d'un nombre $x$ par la fonction f, la valeur $f(x)$. Par exemple l'image de 2 par la fonction f est $f(2)$. On peut calculer des images à l'aide de l'expression de $f$ ou à l'aide d'une représentation graphique de $f$.

On appelle <mark>antécédent(s)</mark> d'un nombre $k$ par la fonction f, les nombres $x$ qui vérifient $f(x)=k$. En particulier, on appelle <mark>racine(s)</mark> d'une fonction (ou d'une équation, d'un polynome) les antécédents de 0 par la fonction f, c'est à dire les solutions de l'équations $f(x)=0$.
On peut calculer des antécédents à l'aide de l'expression de $f$ ou à l'aide d'une représentation graphique de $f$: on cherche les points d'intersection de la courbe représentative de $f$ avec la droite d'équation $y=k$. Un programme ou un tableau de valeur peut aussi être utilisé pour déterminer le nombre de solutions d’une équation du type $f(x) = k$ et déterminer un encadrement ou des valeurs approchées. De même, on peut résoudre algébriquement ou graphiquement une inéquation du type $f(x) \leq k$.

### Fonctions usuelles et représentations graphiques

{{< figure src="maths/fonctions-usuelles.png" caption="Fonctions linéaire (verte), carré (rouge), racine carré (bleu).">}}

Une <mark>fonction affine</mark> est une fonction représentée par une droite et qui peut s'écrire sous la forme $f(x)=a \times x + b$ où $a$ et $b$ sont des constantes appelées pente et ordonnée à l'origine. En effet, on a $f(0)=b$. Dans le cas où $b=0$, on l'appelle <mark>fonction linéaire</mark>, représentée par une droite passant par l'origine O. Dans ce cas la pente $a$ est aussi appelée coefficient de proportionnalité. 

On appelle <mark>fonction carré</mark> la fonction qui à $x$ associe $f(x)=x\times x$ noté $x^2$, représentée par la parabole d'équation $y=x^2$. De même on définit la <mark>fonction cube</mark> comme la fonction qui à $x$ associe $f(x)=x\times x \times x$ noté $x^3$. Enfin, pour un entier naturel $n$, on appelle <mark>fonction puissance n</mark>, la fonction qui à $x$ associe $f(x)=x\times ... \times x= x^n$ (n fois). On peut généraliser cette définition en notant que $x^{-1}=\frac{1}{x}$ et $x^\frac{1}{2}=\sqrt{x}$.
Pour rappel, pour trois nombres entiers $a$, $b$ et $n$, on a les règles suivantes de calcul sur les puissances:

\begin{equation*}
    2^a \times 2^b = 2^{a+b}
\end{equation*}

\begin{equation*}
    \frac{2^a}{2^b} = 2^{a-b}
\end{equation*}

\begin{equation*}
    2^a \times 10^a = (2 \times 10)^a
\end{equation*}

\begin{equation*}
    (2^a)^n = 2^{a \times n}
\end{equation*}

On appelle fonction <mark>racine carré</mark>, notée $f(x)=\sqrt{x}$ ou encore $x^{\frac{1}{2}}$ la fonction réciproque de la fonction carrée, définie pour tout réel $x$ positif. Autrement dit, pour tout nombre $x \geq 0$, $\sqrt{x^2}=x$ et $(\sqrt{x})^2=x$.

On appelle <mark>valeur absolue</mark>, la fonction qui à $x$ associe $x$ si $x$ est positif et $-x$ sinon, notée $f(x)=|x|$. Elle permet de mesurer la distance entre deux nombres réels. Par exemple, la distance entre 6 et 4 est $|4-6|=|-2|=2$.

On appelle <mark>fonction inverse</mark>, représentée par une hyperbole, la fonction qui à tout réels $x$ non nul associe $f(x)=\frac{1}{x}$ aussi noté $x^{-1}$.

On appelle <mark>fonctions trigonométriques</mark> les fonctions cosinus, sinus et tangente.

{{< figure src="maths/trigo.png" caption="Fonctions trigonométriques cosinus et sinus. On dit que la fonction cosinus est <mark>paire</mark>, elle vérifie $f(-x)=f(x)$ pour tout réel x (la courbe est symétrique par rapport à l'axe (Oy)). On dit que la fonction sinus est <mark>impaire</mark>, elle vérifie $f(-x)=-f(x)$ pour tout réel x (la courbe est symétrique par rapport à l'origine O). On dit aussi que ces fonctions sont <mark>périodiques</mark>, de période $2\times \pi$: pour tout réel $x$, elles vérifient $f(x+2\times\pi) = f(x)$.">}}

### Continuité et limites

On dit qu'une fonction $f$ admet une <mark>limite</mark> finie $l$ en un point, notée $\lim\limits_{x \to a}f(x)=l$ si tout intervalle ouvert contenant $l$ contient toutes les valeurs $f(x)$ au voisinage de $a$ ou à partir d'un certain rang lorsque $a=\pm \infty$. On dit qu'une fonction $f$ admet une limite infinie en un point si $l=\pm \infty$.

A titre d'exemple, les fonctions carré, cube et racine carrée, tendent vers $+ \infty$ quand x tend vers $+\infty$, et on a les propriétés suivantes sur les limites: Si f et g tendent vers $+\infty$ quand x tend vers $a$, alors $f+g$ et $f\times g$ tendent vers $+\infty$ quand x tend vers $a$. En revanche, on ne peut rien dire de $f-g$ et de $\frac{f}{g}$ (forme indéterminée), cela dépend de la vitesse à laquelle chacun tend vers $+\infty$. De même, si f tend vers $+\infty$ quand x tend vers $a$ et g tend vers $0$, on ne peut rien dire de la limite de $f \times g$ en $a$. Des méthodes existent pour déterminer la limite de formes indéterminées, par exemple en factorisant par le terme prépondérant dans une somme.

On dit que la courbe d'une fonction $f$ admet une <mark>asymptote horizontale</mark> d'équation $y=l$ si $\lim\limits_{x \to \pm \infty}f(x)=l$. On dit que la courbe d'une fonction $f$ admet une <mark>asymptote verticale</mark> d'équation $x=a$ si $\lim\limits_{x \to a}f(x)=\pm \infty$. On dit que $f$ admet la droite d'équation $y=a\times x + b$ comme <mark>asymptote oblique</mark> si la courbe représentative de $f$ tend à se confondre avec la droite quand $x$ tend vers $\pm \infty$.

#### Notions de continuité

{{< figure src="maths/continue.png" caption="Fonctions continue et discontinues.">}}

On dit qu'une fonction $f$ est <mark>continue</mark> en un point $a$ si $\lim\limits_{x \to a}f(x)=f(a)$. On dit que $f$ est <mark>continue</mark> sur un intervalle si elle est continue en chaque point. Graphiquement, une fonction continue se trace sans lever la main.

<b>Théorème des valeurs intermédiaires</b>: Si $f$ est continue sur $[a,b]$ et $k$ est compris entre $f(a)$ et $f(b)$, alors l'équation $f(x) = k$ admet des solutions (démonstration par dichotomie). Lorsque $f$ est strictement monotone, la solution est unique.

### Variations, dérivabilité et extremum

#### Nombre dérivé (local)

{{< figure src="maths/tangente.png" caption="Représentation graphique du taux de variation, nombre dérivée et tangente comme limite en faisant tendre B vers A. Application en cinématique: Un taux de variation comme une vitesse moyenne et un nombre dérivé comme une vitesse instantanée.">}}

On appelle <mark>taux de variation</mark> d’une fonction en deux points $A$ et $B$, la pente (ou coefficient directeur) de la droite passant par $A$ et $B$.

Calcul du taux de variation $\tau_{A,B}$ entre A et B:

\begin{equation*}
    \tau_{A,B} = \frac{f(x_b) - f(x_a)}{x_b-x_a}
\end{equation*}

En prenant $x_b=x_a+h$, on obtient

\begin{equation*}
    \tau_{A,h} = \frac{f(x_a + h) - f(x_a)}{h}
\end{equation*}

On appelle <mark>nombre dérivé</mark> d’une fonction en un point $a$, noté $f'(a)$, la limite du taux de variation à la courbe représentative d’une fonction en un point donné.

\begin{equation*}
    f'(a) = \lim\limits_{h \to 0} \tau_{A,h}
\end{equation*}

Pour les fonctions carré, inverse, racine carrée et fonctions du second degré, on peut  faire apparaître une approximation linéaire pour h petit qui permet de calculer le nombre dérivé en un point.

On appelle <mark>tangente</mark> à la courbe représentative de $f$ au point d’abscisse a, la droite d’équation $y = f(a) + f’(a)(x - a)$ dont la pente $f’(a)$ correspond au nombre dérivé de $f$ en $a$. La tangente est la limite de la droite donné pour un taux d'accroissement. Elle permet d'approximer au mieux la courbe $f$ au voisinage de $a$.

Remarque:
Pour une fonction affine, le coefficient directeur correspond au nombre dérivé (constant). S'il est positif, la fonction croit. Sinon, la fonction décroit.

On appelle <mark>extremum</mark> de la courbe un minimum ou maximum de cette courbe. Il peut être local ou global.

<b>Propriété</b>: Si $f$ est dérivable en $a$ et $a$ est un extremum de la courbe de $f$, alors $f'(a)=0$. Dans ce cas, la tangente à la courbe représentative est horizontale.

#### Fonction dérivée (globale)}

On dit qu'une fonction $f$ est <mark>dérivable</mark>
sur un intervalle $I$ si elle admet un nombre dérivée en chaque point. Dans ce cas on appelle <mark>fonction dérivée</mark> la fonction $f'(x)$. Elle est utile pour étudier le sens de variation et les extremums d'une fonction. En effet, si $f'$ est positif, la fonction $f$ croit et si $f'$ est négatif, la fonction $f$ décroit. Ceci permet de dresser un tableau de variations de la fonction $f$ et chercher d'éventuels extremum (problème d'optimisation) en cherchant les antécédants de $0$ par $f'$. 

<b>Propriété</b>: Une fonction dérivable sur un intervalle est continue. La réciproque est fausse (exemple de la fonction fonction racine carrée et valeur absolue en 0).

<b>Propriété</b>: Le tableau suivant donne les fonctions dérivées des fonctions usuelles,

| Fonction | Domaine $D_f$ | Dérivée | Domaine $D_{f'}$ |
|---|---|---|---|
| $f(x) = x$   | $\mathbb{R}$ | $f'(x) = 1$        | $\mathbb{R}$ |
| $f(x) = x^2$ | $\mathbb{R}$ | $f'(x) = 2\times x$       | $\mathbb{R}$ |
| $f(x) = x^3$ | $\mathbb{R}$ | $f'(x) = 3\times x^2$     | $\mathbb{R}$ |
| $f(x) = x^n$ |  Dépend de n | $f'(x) = n\times x^{n-1}$ | Dépend de n  |


On a aussi les propriétés suivantes pour des fonctions dérivables: 

\begin{equation*}
    (f+g)'=f'+g'
\end{equation*}

\begin{equation*}
    (f\times g)'=f'\times g+ f \times g'
\end{equation*}

\begin{equation*}
    (\frac{f}{g})'= \frac{f'\times g - f  \times  g'}{g^2}
\end{equation*}

\begin{equation*}
    (f(g))'= g' \times f'(g)
\end{equation*}

La dernère égalité, donnée pour calculer la dérivée d’une fonction composée, aussi noté $f o g$, permet de calculer les fonctions dérivées suivantes

| Fonction composée | Dérivée |
|---|---|
| $x \rightarrow f(a\times x + b)$   | $x \rightarrow a\times f'(a\times x + b)$ |
| $x \rightarrow u(x)^2$ | $x \rightarrow 2 \times u(x) \times u'(x)$ |
| $x \rightarrow e^{u(x)}$ | $x \rightarrow u'(x) \times e^{u(x)}$ |
| $x \rightarrow ln(u(x))$ | $x \rightarrow \frac{u'(x)}{u(x)}$ |

### Fonctions convexes

{{< figure src="maths/convexe.png" caption="Exemple d'une fonction concave puis convexe. A est appelé <mark>point d'inflexion</mark>, c'est un point où la courbe représentative d'une fonction change de convexité.">}}

On dit qu'une fonction $f$ est <mark>convexe</mark> (respectivement <mark>concave</mark>) 
sur un intervalle $I$ si la courbe représentative de $f$ est au dessus (respectivement en dessous) de ses sécantes.
Lorsque $f$ est dérivable, cela se traduit par la courbe représentative de $f$ est au dessus (respectivement en dessous) de ses tangentes. Cette caractérisation se traduit par la croissance (respectivement la décroissance) de $f’$. 

<b>Propriété</b>: Si $f$ est deux fois dérivables sur un intervalle et si $f''$ est positive, alors la fonction $f$ est convexe et réciproquement. Si $f''$ est négative, alors la fonction $f$ est concave et réciproquement.

### Fonction exponentielle

On appelle <mark>fonction exponentielle</mark>, notée $f(x)=exp(x)=e^x$, l'unique fonction dérivable sur $\mathbb{R}$ vérifiant $f’ = f$ et $f(0) = 1$. Elle est strictement positive et croissante. Sa limite en $-\infty$ est $0$ et sa limite en $+\infty$ est $+\infty$.

<b>Propriété</b>: Pour tous réels x et y, on a
\begin{equation*}
    e^{x + y} = e^x \times e^y
\end{equation*}
\begin{equation*}
    e^{-x} = \frac{1}{e^x}
\end{equation*}

On appelle fonction <mark>logarithme népérien</mark>, notée $f(x)=ln(x)$ la fonction réciproque de la fonction exponentielle, définie pour tout réel $x > 0$. Autrement dit, pour tout nombre $x > 0$, $e^{ln(x)}=x$ et $ln(e^x)=x$. Sa limite en $0$ est $-\infty$ et sa limite en $+\infty$ est $+\infty$.

<b>Propriété</b>: Pour tout entier n, et pour tout réels x et y strictement positifs, on a 

\begin{equation*}
    ln(x \times y) = ln(x) + ln(y)
\end{equation*}

\begin{equation*}
    ln(x^n) = n  \times  ln(x)
\end{equation*}

\begin{equation*}
    ln(\frac{1}{x})=-ln(x)
\end{equation*}

<b>Propriété</b>: Pour tout entier naturel $n>0$,

\begin{equation*}
    \lim\limits_{x \to 0} x \times ln(x) = 0
\end{equation*}

\begin{equation*}
    \lim\limits_{x \to +\infty} \frac{ln(x)}{x}  = 0
\end{equation*}

\begin{equation*}
    \lim\limits_{x \to +\infty} \frac{e^x}{x^n}  = 0 
\end{equation*}

## Exercices résolus
- [Livret de la 3ème à la 2nde](https://www.louislegrand.fr/wp-content/uploads/2021/07/Livret-3eme-2nde.pdf): Exercices 8 à 13 et 61 à 67.
- [Livret de la 2nde à la 1ère](https://lycee-henri4.com/wp-content/uploads/2023/06/Livret-2nde-1ere.pdf): Exerices 59 à 73.
- [Livret de la 1ère à la terminale](https://lycee-henri4.com/wp-content/uploads/2024/07/Livret-1ere-Term-2024-07-.pdf): Exerices 33 à 49.
- [Livret de la terminale au supérieur](https://lycee-henri4.com/wp-content/uploads/2022/07/CPES-MATHS.pdf): Exerices 4 et 5.