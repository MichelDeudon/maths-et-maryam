---
title: Introduction aux suites réelles
date: '2025-05-15'
type: book
weight: 10
math: true
tags:
  - Analyse
  - Suites réelles
---

Cours d'analyse - partie I.

<!--more-->

## Introduction aux suites réelles

Les suites peuvent modéliser des phénomènes \textit{discrets}, comme l'évolution du stock de livres d'une médiathèque à l'année $n$, $n+1$... (temps \textit{discret}) ou l'évolution d’une population en écologie (on peut citer les modèles de Malthus et de Verhulst en dynamiques de populations, ou encore les modèles de proie prédateur avec 2-3 suites récurrentes couplées). Ce dernier cas permet d'étudier par exemple l'effet de la réintroduction de loups dans le parc de Yellowstone.
 
### Représentations d'une suite

#### Formule explicite
Certaines suites peuvent s'écrire comme des fonctions définies sur l'ensemble des entiers naturels. Pour tout entier naturel $n$,
\begin{equation*}
    u_{n}=f(n)
\end{equation*}
Par exemple, $u_n=2 \times n$ permet de définir la suite des nombres paires 0, 2, 4... notée $u_0$, $u_1$, $u_2$... La fonction $f$ dépend du problème étudié. Lorsqu'elle est \hl{\textbf{explicite}}, on peut calculer les termes d’une suite en \textit{remplacant} $n$ dans l'expression $u_n = f(n)$. Par exemple, pour calculer $u_3$ il suffit de calculer $u_3=2 \times 3 = 6$. On peut aussi lire $u_3$ graphiquement à partir de la courbe représentative de $f$.

\begin{figure}
	\centering
	\includegraphics[width=0.8\linewidth]{../img/suites.png}.
     \caption{Exemple d'une suite arithmétique (les nombres paires en bleu, $+2$) et d'une suite géométrique (les puissances de 2 en rouge, $\times 2$).}
\end{figure}

#### Relation de récurrence
Certaines suites s'écrivent à l'aide d'une \textit{condition initiale} (premier terme donné $u_0 = a$) et d'une \hl{\textbf{relation de récurrence}} qui traduit une évolution: Pour tout entier naturel $n$,
\begin{equation*}
  \begin{array}{l}
    u_{n+1} = u_n + gains - pertes
  \end{array}
\end{equation*}
Par exemple, $u_{0}=0$ et $u_{n+1} = u_n +2$ permet de définir la suite des nombres paires 0, 2, 4... Autre exemple, la suite de Fibonacci, définie par $u_0=0$, $u_1=1$ et $u_{n+1}=u_{n}+u_{n-1}$, est reliée au \textit{nombre d'or} qui a de nombreuses application artistiques, notamment en photographie.
On peut aussi modéliser l'évolution d'une population à l'aide de la suite $u_{n+1} = u_n + \tau \times u_n = (1 + \tau) \times u_n $, $\tau$ s'interprête comme le \hl{\textbf{taux d'accroissement}}.


Pour calculer les termes successifs d'une suite récurrente, il suffit de \textit{remplacer} $n$ dans l'expression précédente. En prenant $n=0$, on calcule $u_{1}$ à partir du premier terme $u_0$, puis avec $n=1$, on calcule $u_{2}$ à partir de $u_1$, etc. On peut aussi construire successivement $u_1$, $u_2$, $u_3$... graphiquement, en utilisant la droite d'équation $y=x$.

### Sens de variation et limite

\paragraph{Définition} La suite $(u_n)$ \hl{\textbf{tend vers $+ \infty$}}, notée $\lim\limits_{\substack{n \to +\infty}} u_n = +\infty$, si tout intervalle de la forme [A;$+\infty$[ contient toutes les valeurs $u_n$ à partir d'un certain entier $n^*$.
%De manière analogue, on définit une suite qui tend vers $-\infty$.
La suite $(u_n)$ \hl{\textbf{converge vers le réel $l$}}, notée $\lim\limits_{\substack{n \to +\infty}} u_n = l$, si tout intervalle ouvert contenant $l$ contient toutes les valeurs $u_n$ à partir d'un certain entier $n^*$.

\paragraph{Théorème}: Toute suite croissante majorée (ou décroissante minorée) converge.

\paragraph{Corollaire}: Toute suite croissante non majorée (ou décroissante non minorée) diverge vers $\pm \infty$.

### Suites arithmétiques et géométriques

\paragraph{Définition}
Une \hl{\textbf{suite arithmétique}} est une suite dans laquelle chaque terme s'obtient à partir du précédent, en lui ajoutant une constante $\textbf{r}$ appelée raison (ou gain). 
Une \hl{\textbf{suite géométrique}} est une suite dans laquelle chaque terme s'obtient à partir du précédent, en le multipliant par un facteur constant $\textbf{q}$ appelé raison (ou gain). 

\begingroup
\setlength{\tabcolsep}{10pt} % Default value: 6pt
\renewcommand{\arraystretch}{1.2} % Default value: 1
\begin{center}
\begin{tabular}{ |c|c|c| }
 \hline
  & \textbf{Suite arithmétique} & \textbf{Suite géométrique} \\ 
 \hline
 Exemple & Les nombres paires $(2n)_{n\in\mathbb{N}}$ & Les puissances $(2^n)_{n\in\mathbb{N}}$ \\  
 \hline
 1er termes &2,4,6,8... & 2,4,8,16... \\  
 \hline
 Formule explicite & $u_{n}=u_{0}+n \times  r$ & $u_{n}=u_{0}\times q^{n}$ \\
 \hline
 Récurrence & $u_{n+1}=u_{n}+r$ & $u_{n+1}=q\times u_{n}$  \\
 \hline
 Caractérisation & $u_{n+1}-u_n=r$ (constant) & $\frac{u_{n+1}}{u_n}=q$ (constant) \\  
 \hline
 Variations & Constantes & Proportionnelles à $u_n$ \\  
 \hline
 Évolution & Linéaire / Affine & Exponentielle \\  
% & & \\
% à partir d'un rang $p$ &  $u_{n}=u_{p}+(n-p)r$ & $u_{n}=u_{p}q^{n-p}$ \\   
 \hline
 Cas particulier & $r=0$  & $q=1$ ou $u_0= 0$ \\  
 Suite constante &  & \\ 
 \hline
 Sens de variation & $\nearrow$ si $r > 0$  & $\nearrow$ si $q>1$ et $u_0\geq 0$ \\  
  & & ou $q\in [0;1[$ et $u_0 \leq 0$\\ 
  & $\searrow$ si $r < 0$ & $\searrow$ si $q\in [0;1[$ et $u_0\geq 0$\\  
  & & ou $q > 1$ et $u_0\leq 0$\\  
  & & Non monotone si $q < 0$ \\
 \hline
 Limite & $\lim\limits_{\substack{n \to +\infty}} u_n = +\infty$ si $r > 0$ & $\lim\limits_{\substack{n \to +\infty}} u_n = 0$ si $|q|<1$ \\  
 & $\lim\limits_{\substack{n \to +\infty}} u_n = -\infty$ si $r < 0$ & $\lim\limits_{\substack{n \to +\infty}} |u_n| = +\infty$ si $|q|>1$  \\  
% &  & Pas de limite si  $q\leq -1$\\ 
 \hline
$u_0 + u_1 + ... + u_n = $  & $(n+1)u_0 + \frac{n(n+1)r}{2}$ & $u_{0}{\frac {1-q^{n+1}}{1-q}}$ \\  
 \hline
Cas particulier  & $1+2+...+n= \frac{n(n+1)}{2}$ & $1 + q + … + q^n = {\frac {1-q^{n+1}}{1-q}}$ \\  
 \hline
\end{tabular}
\end{center}
\endgroup

### Exercices résolus
\begin{itemize}
 \item \href{https://lycee-henri4.com/wp-content/uploads/2023/06/Livret-1ere-Term.pdf}{Livret de la 1ère à la terminale}: Exerices 18 à 28 sur les suites.
 \item \href{https://lycee-henri4.com/wp-content/uploads/2022/07/CPES-MATHS.pdf}{Livret de la terminale au supérieur}: Exerice 6 sur les suites.
\end{itemize}