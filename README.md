# Équations différentielles linéaires

## Définition

Soit l'***équation différentielle linéaire*** (EDL) scalaire suivante:

$$
a_{0}(x)y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
$$

où les $a_{i}(x)$ et $f(x)$ sont des fonctions continues de $I \subseteq \mathbb{R}$ dans $\mathbb{K}$, $I$ étant connexe.

Sur tout intervalle où $a_{0}(x)$ ne s'annule pas, l'EDL peut se mettre sur la forme&nbsp;:

$$
y^{(p)}(x) + \frac{a_{1}(x)}{a_{0}(x)}y^{(p-1)}(x) + \frac{a_{2}(x)}{a_{0}(x)}y^{(p-2)}(x) + \dots + \frac{a_{p-2}(x)}{a_{0}(x)}y^{\prime\prime}(x) + \frac{a_{p-1}(x)}{a_{0}(x)}y^{\prime}(x) + \frac{a_{p}(x)}{a_{0}(x)}y(x) = \frac{f(x)}{a_{0}(x)}
$$

ou encore

$$
y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
$$

en modifiant $f(x)$ et les $a_{i}(x)$&nbsp;!

## Passage d'une EDL à un SDL

En posant $z_{k}(x) \coloneqq y^{k-1}(x)$ ou encore&nbsp;:

$$
\begin{align*}
  z_{1}(x) &\coloneqq y(x) \\
  z_{2}(x) &\coloneqq y^{\prime}(x) = z_{1}^{\prime}(x) \\
  z_{3}(x) &\coloneqq y^{\prime\prime}(x) = z_{2}^{\prime}(x) \\
&\dots \\
z_{p-2}(x) &\coloneqq y^{(p-3)}(x) = z_{p-3}^{\prime}(x) \\
z_{p-1}(x) &\coloneqq y^{(p-2)}(x) = z_{p-2}^{\prime}(x) \\
  z_{p}(x) &\coloneqq y^{(p-1)}(x) = z_{p-1}^{\prime}(x)
\end{align*}
$$

on peut ramener l'EDL régulière d'ordre $p$

$$
y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
$$

au SDL constitué de $p$ EDL du 1<sup>ère</sup> ordre&nbsp;:

$$
\left\{ \begin{aligned} 
  z_{p}^{\prime}(x) + a_{1}(x)z_{p}(x) + a_{2}(x)z_{p-1}(x) + \dots + a_{p-1}(x)z_{2}(x) + a_{p}(x)z_{1}(x) &= f(x) \\
  z_{p-1}^{\prime}(x) &= z_{p}(x) \\
  z_{p-2}^{\prime}(x) &= z_{p-1}(x) \\
                      &\dots \\
  z_{2}^{\prime}(x) &= z_{3}(x) \\
  z_{1}^{\prime}(x) &= z_{2}(x)
\end{aligned} \right.
$$

ou encore

$$
\left\{ \begin{aligned}
    z_{1}^{\prime}(x) &= z_{2}(x) \\
    z_{2}^{\prime}(x) &= z_{3}(x) \\
                      &\dots \\
  z_{p-2}^{\prime}(x) &= z_{p-1}(x) \\
  z_{p-1}^{\prime}(x) &= z_{p}(x) \\
  z_{p}^{\prime}(x) + a_{1}(x)z_{p}(x) + a_{2}(x)z_{p-1}(x) + \dots + a_{p-1}(x)z_{2}(x) + a_{p}(x)z_{1}(x) &= f(x)
\end{aligned} \right.
$$

### Passage d'une EDL du 2<sup>ème</sup> ordre à un SDL de 2 EDL du 1<sup>er</sup> ordre

Soit l'équation différentielle linéaire (EDL) scalaire du **2<sup>ème</sup> ordre**:

$$
a_{0}(x)y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = f(x)
$$

où $a_{0}(x)$, $a_{1}(x)$, $a_{2}(x)$ et $f(x)$ sont des fonctions continues de $I \subseteq \mathbb{R}$ dans $\mathbb{K}$, $I$ étant connexe.

Sur tout intervalle où $a_{0}(x)$ ne s'annule pas, l'EDL peut se mettre sur la forme&nbsp;:

$$
y^{\prime\prime}(x) + \frac{a_{1}(x)}{a_{0}(x)}y^{\prime}(x) + \frac{a_{2}(x)}{a_{0}(x)}y(x) = \frac{f(x)}{a_{0}(x)}
$$

ou encore

$$
y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = f(x)
$$

en modifiant $a_{0}(x)$, $a_{1}(x)$, $a_{2}(x)$ et $f(x)$&nbsp;!

En posant $z_{k}(x) \coloneqq y^{k-1}(x)$ ou encore&nbsp;:

$$
\begin{align*}
  z_{1}(x) &\coloneqq y(x) \\
  z_{2}(x) &\coloneqq y^{\prime}(x) = z_{1}^{\prime}(x)
\end{align*}
$$

on peut ramener l'EDL régulière du 2<sup>ème</sup> ordre&nbsp;:

$$
y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = f(x)
$$

au SDL constitué de $2$ EDL du 1<sup>ère</sup> ordre&nbsp;:

$$
\left\{ \begin{aligned} 
  z_{2}^{\prime}(x) + a_{1}(x)z_{2}(x) + a_{2}(x)z_{1}(x) &= f(x) \\
  z_{1}^{\prime}(x) &= z_{2}(x)
\end{aligned} \right.
$$

ou encore

$$
\left\{ \begin{aligned}
  z_{1}^{\prime}(x) &= z_{2}(x) \\
  z_{2}^{\prime}(x) + a_{1}(x)z_{2}(x) + a_{2}(x)z_{1}(x) &= f(x)
\end{aligned} \right.
$$

## Problème de Cauchy

### Problème de Cauchy pour un SDL de $m$ EDL du 1<sup>er</sup> ordre

Soient $x_{0} \in I$ et les $y_{0,m} \in \mathbb{K}$ appelés données initiales.

I s'agit de déterminer les fonctions $y_{m}(x)$ de $I$ dans $\mathbb{K}$ qui sont solutions du SDL suivant&nbsp;:

$$
\left\{ \begin{alignat*}{15}
    y_{1}^{\prime}(x) &= a_{1,1}(x)y_{1}(x) &&+ a_{1,2}(x)y_{1}(x) &&+ a_{1,3}(x)y_{3}(x) &&+ \dots &&+ a_{1,m-2}(x)y_{m-2}(x) &&+ a_{1,m-1}(x)y_{m-1}(x) &&+ a_{1,m}(x)y_{m}(x) &&+ f_{1}(x) \\
    y_{2}^{\prime}(x) &= a_{2,1}(x)y_{1}(x) &&+ a_{2,2}(x)y_{2}(x) &&+ a_{2,3}(x)y_{3}(x) &&+ \dots &&+ a_{2,m-2}(x)y_{m-2}(x) &&+ a_{2,m-1}(x)y_{m-1}(x) &&+ a_{2,m}(x)y_{m}(x) &&+ f_{2}(x) \\
    y_{3}^{\prime}(x) &= a_{3,1}(x)y_{1}(x) &&+ a_{3,2}(x)y_{2}(x) &&+ a_{3,3}(x)y_{3}(x) &&+ \dots &&+ a_{3,m-2}(x)y_{m-2}(x) &&+ a_{3,m-1}(x)y_{m-1}(x) &&+ a_{3,m}(x)y_{m}(x) &&+ f_{3}(x) \\
                      &\dots&&&&&&&&&&&&&& \\
    y_{m-2}^{\prime}(x) &= a_{m-2,1}(x)y_{1}(x) &&+ a_{m-2,2}(x)y_{2}(x) &&+ a_{m-2,3}(x)y_{3}(x) &&+ \dots &&+ a_{m-2,m-2}(x)y_{m-2}(x) &&+ a_{m-2,m-1}(x)y_{m-1}(x) &&+ a_{m-2,m}(x)y_{m}(x) &&+ f_{m-2}(x) \\
    y_{m-1}^{\prime}(x) &= a_{m-1,1}(x)y_{1}(x) &&+ a_{m-1,2}(x)y_{2}(x) &&+ a_{m-1,3}(x)y_{3}(x) &&+ \dots &&+ a_{m-1,m-2}(x)y_{m-2}(x) &&+ a_{m-1,m-1}(x)y_{m-1}(x) &&+ a_{m-1,m}(x)y_{m}(x) &&+ f_{m-1}(x) \\
    y_{m}^{\prime}(x) &= a_{m,1}(x)y_{1}(x) &&+ a_{m,2}(x)y_{2}(x) &&+ a_{m,3}(x)y_{3}(x) &&+ \dots &&+ a_{m,m-2}(x)y_{m-2}(x) &&+ a_{m,m-1}(x)y_{m-1}(x) &&+ a_{m,m}(x)y_{m}(x) &&+ f_{m}(x)
\end{alignat*} \right.
$$

et qui satisfont les conditions intiales&nbsp;:

$$
\left\{ \begin{aligned}
  y_{1}(x_{0}) &= y_{0,1} \\
  y_{2}(x_{0}) &= y_{0,2} \\
  y_{3}(x_{0}) &= y_{0,3} \\
               &\dots \\
  y_{m-2}(x_{0}) &= y_{0,m-2} \\
  y_{m-1}(x_{0}) &= y_{0,m-1} \\
  y_{m}(x_{0}) &= y_{0,m}
\end{aligned} \right.
$$

### Problème de Cauchy pour une EDL d'ordre $p$

Soient $x_{0} \in I$ et les $y_{0,p} \in \mathbb{K}$ appelés données initiales.

I s'agit de déterminer les fonctions $y(x)$ de $I$ dans $\mathbb{K}$ qui sont solutions de l'EDL suivante&nbsp;:

$$
a_{0}(x)y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
$$

et qui satisfont les conditions intiales&nbsp;:

$$
\left\{ \begin{aligned}
  y(x_{0}) &= y_{0,0} \\
  y^{\prime}(x_{0}) &= y_{0,1} \\
  y^{\prime\prime}(x_{0}) &= y_{0,2} \\
               &\dots \\
  y^{(p-3)}(x_{0}) &= y_{0,p-3} \\
  y^{(p-2)}(x_{0}) &= y_{0,p-2} \\
  y^{(p-1)}(x_{0}) &= y_{0,p-1}
\end{aligned} \right.
$$

Nous notrons la solution unique de ce problème de Cauchy de la manière suivante&nbsp;:

$$
y(x) = y(x; x_{0}; (y_{0,0}, y_{0,1}, y_{0,2}, \dots, y_{0,p-3}, y_{0,p-2}, y_{0,p-1}); f(x))
$$
