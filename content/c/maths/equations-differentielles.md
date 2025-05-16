---
title: Equa diff et Primitives
date: '2025-05-15'
type: book
weight: 30
math: true
tags:
  - Analyse
  - Equations Différentielles
  - Primitives
---

Introduction à l'analyse (partie III).

<!--more-->

## Introduction aux équations différentielles

Les <mark>équations différentielles</mark> sont nombreuses en physique. Il s'agit d'équations dont l'inconnue est une fonction. 
Par exemple l'équation différentielle $y'=y$ a pour solution $f(x)=k\times e^x$ où $k$ est un nombre réel. Plus généralement, en notant $a$ et $b$ deux nombres réels, l'équation différentielle linéaire du premier ordre à coefficients constants
\begin{equation*}
 y’ = a \times y + b   
\end{equation*}
a pour solution générale
\begin{equation*}
 f(x)=k\times e^{a \times x} - \frac{b}{a}
\end{equation*}

On peut en effet vérifier que la fonction $f$ est solution de l'équation différentielle quelque soit la valeur de $k$. Lorsque b = 0, la somme de deux solutions et le produit d’une solution par une constante sont encore solutions.
Lorsque $a$ est négatif, le deuxième terme appelé solution particulière constante $- \frac{b}{a}$ correspond à la limite de $f(x)$ quand $x$ tend vers $+\infty$, par exemple la charge d'un condensateur $U_c(t)$ ou la température extérieur d'un système qui refroidit $T(t)$:

\begin{equation*}
 \frac{dU_c}{dt} = \frac{-1}{\tau} \times U_c + \frac{E}{\tau}  
\end{equation*}

\begin{equation*}
 \frac{dT}{dt} = \frac{-1}{\tau} \times (T - T_{ext})  
\end{equation*}

Pour une condition initiale donnée, par exemple $U_c(t=0)=0$ ou $T(t=0)=T_{0}$, il existe une unique solution aux équations différentielles précédentes. La condition initiale permet de trouver la valeur de $k$ et par conséquent de déterminer l'unique solution vérifiant simultanément l'équation différentielle et la condition initiale donnée. 

## Introduction aux primitives

On appelle <mark>primitive</mark> d’une fonction $f$ continue sur un intervalle $I$, une fonction $F$ qui vérifie $F'=f$, autrement dit une solution de l’équation différentielle $y’ = f$.  La recherche d’une primitive est l’opération inverse de la dérivation, ce qui permet de traiter les cas usuels par lecture inverse du tableau des dérivées.
A noter que deux primitives d’une même fonction continue sur un intervalle diffèrent seulement d’une constante $k$. 

| Fonction | Domaine $D_f$ | Primitive | Domaine $D_{F}$ |
|---|---|---|---|
| $f(x) = 1$ | $\mathbb{R}$ | $F(x) = x+k$  | $\mathbb{R}$ |
| $f(x) = x$ | $\mathbb{R}$ | $F(x) = \frac{1}{2}x^2+k$  | $\mathbb{R}$ |
| $f(x) = x^n$ |  Dépend de n | $F(x) = \frac{x^{n+1}}{n+1} + k$ | Dépend de n |
| $f(x) = e^x$ | $\mathbb{R}$ | $F(x) = e^x+k$  | $\mathbb{R}$ |
| $f(x) = sinus(x)$ |  $\mathbb{R}$ | $F(x) = -cosinus(x)$ | $\mathbb{R}$ |
| $f(x) = cosinus(x)$ |  $\mathbb{R}$ | $F(x) = sinus(x) + k$ | $\mathbb{R}$ |

<b>Théorème</b>: Toute fonction continue sur un intervalle admet des primitives. 

Remarque: Pour certaines fonctions, on ne dispose pas de primitive explicite. On peut approchée une solution par la méthode d’Euler.

## Exercices résolus

- [Livret de la 1ère à la terminale](https://lycee-henri4.com/wp-content/uploads/2024/07/Livret-1ere-Term-2024-07-.pdf): Exerices 18 à 28.
- [Livret de la terminale au supérieur](https://lycee-henri4.com/wp-content/uploads/2022/07/CPES-MATHS.pdf): Exerice 6.