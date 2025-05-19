---
title: Introduction
date: '2025-05-15'
type: book
weight: 10
math: true
tags:
  - Analyse
  - Algèbre
---

Notations, ensembles et logique

<!--more-->

## Notations

Les symboles et les notations apportent un gain en efficacité mais peuvent aussi rendre difficile la compréhension de définitions ou de propriétés. En règle générale, on utilise des notations qui sont proches des objets étudiés, par exemple nous notons un ensemble $E$, une fonction $f$, le temps $t$, une distance $d$... ce qui permet d'écrire des relations entre ces variables et d'exprimer une variable en fonction des autres. Par exemple $d=v \times t$ où $v$ est la vitesse, $A = \pi r^2$ où $A$ est l'aire (surface) d'un cercle et $r$ son rayon, ou encore $V=c^3$ où $V$ est le volume d'un cube de côté $c$. Le chapitre sur les fonctions s'appuyera notamment sur ces variables pour exprimer la dépendance d'une variable $f$ par rapport à une autre, comme le temps, notée $f(t)$. En pratique, on utilise souvent $x$ ou $t$ comme variable et la notation $f(x)$ ou $f(t)$.
 
{{< figure src="maths/sets.png" caption="Illustration de deux sous-ensembles A et B d'un ensemble E et des notions d'union (A <mark>ou</mark> B, deux cercles) et d'intersection (A <mark>et</mark> B, ellipse au centre)">}}

### Ensembles

On utilise en général une lettre majuscule pour représenter un ensemble, par exemple $\mathbb{N}$ pour l'ensemble des entiers naturels $\{0,1,2,3,4...\}$, et une lettre miniscule pour représenter un élément de cet ensemble, par exemple $n=4$. On note $n\in \mathbb{N}$ pour dire que $n$ "appartient" à l'ensemble $\mathbb{N}$.
On peut considérer un sous-ensemble d'un ensemble, comme les entiers naturels  $Pairs=\{0,2,4...\}$. On note $Pairs \subset \mathbb{N}$ pour dire que le sous-ensemble est contenu (inclus) dans $\mathbb{N}$.
On utilise le symbole $\cup$ pour représenter l'union de deux ensembles et le symbole $\cap$ pour représenter leur intersection. 
Pour l'ensemble des entiers naturels $\mathbb{N}$ par exemple, on a $Pairs \cup Impairs = \mathbb{N}$ et  $Pairs \cap Impairs = \{\}$ (ensemble vide aussi noté $\emptyset$). Plus généralement, en notant $A$ un sous-ensemble de $E$, on utile la notation $\overline{A}$ pour désigner le complémentaire de $A$, c'est à dire le sous-ensemble $B$ qui vérifie $A\cup B=E$ et $A\cap B=\{\}$ .

### Nombres réels

{{< figure src="maths/ensembles.png" caption="Ensemble et sous-ensembles des nombres réels $\mathbb{R}$.">}}

Parmi l'ensemble des nombres réels $\mathbb{R}$ (tous les nombres possibles permettant de mesurer des grandeurs), on distingue divers sous-ensembles:
* Les entiers naturels $\mathbb{N}$ , par exemple $1$, $2$, $3$ ou $4$ ans (âge).
* Les entiers relatifs $\mathbb{Z}$, par exemple $2$ ou $-2^{\circ}C$ (température).
* Les nombres décimaux $\mathbb{D}$, par exemple $0.25$€ (prix au marché). En pratique on peut encadrer un nombre réel par un nombre décimal à $10^{-n}$ près (chiffres significatifs en physique), par exemple $\pi=3.1415...$ et $\sqrt{2}=1.4142...$.
* Les nombres rationels $\mathbb{Q}$ qui peuvent s'écrire sous la forme d'une fraction, par exemple $\frac{1}{2}=0.5$ où $1$ est le numérateur et $2$ le dénominateur, ou encore $\frac{1}{4}=0.25$, $\frac{3}{4}=0.75$, $\frac{1}{5}=0.2$, $\frac{1}{3}=0.333...$, $\frac{2}{3}=0.666...$.
\end{itemize} 

Pour rappel, voici quelques règles de calcul pour les fractions:

\begin{equation*}
    \frac{k \times 1}{k\times 3} = \frac{1}{3}
\end{equation*}

\begin{equation*}
    \frac{1}{3}+\frac{2}{3} = \frac{1 + 2}{3}
\end{equation*}

\begin{equation*}
    \frac{1}{2} \times \frac{3}{4} = \frac{1 \times 3}{2 \times 4}
\end{equation*}

\begin{equation*}
    \frac{\frac{1}{2}}{\frac{3}{4}} = \frac{1}{2} \times \frac{4}{3}
\end{equation*}

### Intervalles de $\mathbb{R}$

On note $[0,1]$ l'ensemble des nombres réels compris entre 0 et 1, c'est un sous ensemble de $\mathbb{R}$.
Graphiquement, les crochets $[A,B]$ permettent de représenter un segment et les parenthèses $()$ une droite. En combinant ces notations, on peut représenter des demi droites, par exemple l'ensemble des nombres réels positifs peut s'écrire $[0,+\infty)$ et l'ensemble des nombres réels négatifs $(-\infty,0]$.

### Autres symboles
Le symbole $\forall$, appelé quantificateur universel, signifie "pour tout". Par exemple, pour tout entier naturel n... peut s'écrire $\forall n \in \mathbb{N}$... Le symbole $\exists$, appelé quantificateur existentiel, signifie "il existe". Par exemple, il existe un entier naturel... peut s'écrire $\exists n \in \mathbb{N}$... 

## Logique

En sciences on est amené à manipuler des variables et des propositions (vraies ou fausses), par exemple "tous les entiers sont pairs" (faux).
On peut aussi formuler la négation de propositions simples, par exemple "il existe des entiers qui ne sont pas paires" (vrai).
On peut combiner plusieurs propositions à l'aide de connecteurs logique, par exemple "je veux" <mark>OU</mark> "je peux" (noté $A \| B$), ou "je veux" <mark>ET</mark> "je peux" (noté $A \& B$). On peut aussi formuler des implications "je peux" donc "je veux" (noté $A \Rightarrow B$), la réciproque d’une implication "je veux" donc "je peux" (noté $B \Rightarrow A$) ou sa contraposée "je veux pas" donc "je peux pas" (noté $\overline{B} \Rightarrow \overline{A}$). On dit dans ce cas que B est une condition nécessaire pour A et A une condition suffisante pour B.
A noter que si A implique B et vice versa, alors on dit que A et B sont équivalents, noté $A \Leftrightarrow  B$ 

Pour démontrer une propriété, on peut raisonner par implications directes ($A \Rightarrow B \Rightarrow C$...) jusqu'au résultat, ou par équivalence si c'est possible ($A \Leftrightarrow B \Leftrightarrow C$...). On peut aussi démontrer une propriété en raisonnant par contraposée ($A \Rightarrow B$ est vrai si et seulement si $\overline{B} \Rightarrow \overline{A}$) ou en raisonnant par disjonctions des cas ou encore par récurrence.
On peut aussi montrer qu'une proposition est fausse en mobilisant simplement un contre-exemple, ou raisonner par l'absurde en supposant que la propriété (fausse) est vraie pour aboutir à une absurdité ou contradiction.

## Exercices résolus
- [Livret de la 3ème à la 2nde](https://www.louislegrand.fr/wp-content/uploads/2021/07/Livret-3eme-2nde.pdf): Exercices 1 à 7 sur le calcul fractionnaire et 68 à 74 sur le raisonnement.
- [Livret de la 2nde à la 1ère](https://lycee-henri4.com/wp-content/uploads/2023/06/Livret-2nde-1ere.pdf): Exerices 1 à 12 sur le calcul numérique.