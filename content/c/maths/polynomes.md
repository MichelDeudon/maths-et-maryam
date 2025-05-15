---
title: Polynomes du 2nd degré
date: '2025-05-15'
type: book
weight: 20
math: true
tags:
  - Analyse
  - Suites réelles
---

Introduction à l'algèbre (partie I).

<!--more-->

## Rappel sur le calcul littéral

<mark>Développer</mark> veut dire passer d'un produit (x) à une somme (+), par exemple $3\times (5+2)=3\times 5+3\times 2$.

<mark>Factoriser</mark> veut dire passer d'une somme (+) à un produit (x).

### Identités remarquables
En pratique, c'est plus difficile de factoriser que de développer. Les identités remarquables peuvent aider à factoriser une expression et donc étudier le signe d'une expression écrite sous la forme d'un produit.

\begin{equation*}
    (a - b)\times (a + b) = a^2 - b^2
\end{equation*}
    
\begin{equation*}
    (a - b)^2 = a^2 - 2\times a\times b + b^2
\end{equation*}

\begin{equation*}
    (a + b)^2 = a^2 + 2\times a\times b + b^2
\end{equation*}
    
On appelle <mark>forme factorisée</mark> (sous forme d'une multiplication) le terme de gauche et <mark>forme développée</mark> (sous forme d'une addition) le terme de droite dans les égalités précédentes.

## Équations, polynômes du second degré

On appelle <mark>polynôme</mark> du second degré une fonction qui peut s'écrire sous la forme développée

\begin{equation*}
    f(x)=a\times x^2 + b \times x + c
\end{equation*}

où $(a,b,c)$ sont trois nombres réels. On peut généraliser cette définition à des polynômes de degré $n$ en prenant $n+1$ nombres réels.

{{< figure src="maths/parabole.png" caption="Parabole représentative d’une fonction polynôme du second degré d’équation $y = a\times x^2 + b \times x + c$. La parabole est symétrique par rapport à la droite d'équation $x_s=\frac{-b}{a}$. Le sens de variation de la fonction dépend de la valeur de $a$.">}}

On appelle <mark>racines</mark> d'un polynome ou d'une équation les solutions de l'équation $f(x)=0$, c'est à dire les antécédents de 0 par la fonction $f$.

<b>Propriété</b>
Un polynôme de degré n admet au plus n racines. 

### Forme factorisée
Lorsqu'une équation du second degré admet deux racines, en les notant $x_1$ et $x_2$, nous pouvons écrire $f(x)$ sous la forme factorisée:


\begin{equation*}
    f(x) = a \times (x - x_1) \times (x - x_2)
\end{equation*}

La forme factorisée d'un polynome est adaptée pour étudier le signe de $f(x)$ en fonction de $x$ à l'aide d'un tableau de signes. En développant la forme factorisée, on peut montrer par identification que la somme et le produit des racines se lisent sur le polynôme, ce qui donne une méthode pour déterminer les racines:

\begin{equation*}
    x_1 + x_2 = \frac{-b}{a}
\end{equation*}

\begin{equation*}
    x_1 \times x_2 = \frac{c}{a}
\end{equation*}

On appelle <mark>discriminant</mark> d'un polynome ou d'une équation du second degré le nombre réel 

\begin{equation*}
    \Delta = b^2 - 4 \times a \times c
\end{equation*}

Lorsque $\Delta$ est strictement négatif, le polynome ne s'annule jamais, son signe est toujours positif ou toujours négatif. Lorsque $\Delta \geq 0$, il existe deux racines (éventuellement confondues) qu'on peut déterminer à l'aide des formules suivantes en vue d'une éventuelle factorisation. 

\begin{equation*}
    x_1 = \frac{-b-\sqrt{\Delta}}{2\times a}
\end{equation*}

\begin{equation*}
    x_2 = \frac{-b+\sqrt{\Delta}}{2\times a}
\end{equation*}

### Forme canonique

Enfin, la forme canonique d’un polynôme du second degré s'écrit sous la forme suivante. Elle est adaptée pour résoudre une équation, inéquation ou étudier les variations et extremum d'un polynôme.

\begin{equation*}
    f(x) = a \times (x - x_s)^2 + \beta
\end{equation*}

### Exercices résolus
- [Livret de la 3ème à la 2nde](https://www.louislegrand.fr/wp-content/uploads/2021/07/Livret-3eme-2nde.pdf): Exercices 21 à 43.
- [Livret de la 2nde à la 1ère](https://lycee-henri4.com/wp-content/uploads/2023/06/Livret-2nde-1ere.pdf): Exercices 13 à 22 et 35 à 58.
- [Livret de la 1ère à la terminale](https://lycee-henri4.com/wp-content/uploads/2024/07/Livret-1ere-Term-2024-07-.pdf): Exercices 1 à 17.
- [Livret de la terminale au supérieur](https://lycee-henri4.com/wp-content/uploads/2022/07/CPES-MATHS.pdf): Exercices 1 à 3.