# Équations différentielles linéaires

## Définition

Soit l'***équation différentielle linéaire*** (EDL) scalaire suivante:

```math
a_{0}(x)y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
```

où les $a_{i}(x)$ et $f(x)$ sont des fonctions continues de $I \subseteq \mathbb{R}$ dans $\mathbb{K}$, $I$ étant connexe.

Sur tout intervalle où $a_{0}(x)$ ne s'annule pas, l'EDL peut se mettre sur la forme&nbsp;:

```math
y^{(p)}(x) + \frac{a_{1}(x)}{a_{0}(x)}y^{(p-1)}(x) + \frac{a_{2}(x)}{a_{0}(x)}y^{(p-2)}(x) + \dots + \frac{a_{p-2}(x)}{a_{0}(x)}y^{\prime\prime}(x) + \frac{a_{p-1}(x)}{a_{0}(x)}y^{\prime}(x) + \frac{a_{p}(x)}{a_{0}(x)}y(x) = \frac{f(x)}{a_{0}(x)}
```

ou encore

```math
y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
```

en modifiant $f(x)$ et les $a_{i}(x)$&nbsp;!

## Passage d'une EDL à un SDL

En posant $z_{k} \coloneqq y^{k-1}$ ou encore&nbsp;:

```math
\begin{align}
  z_{1}(x) &\coloneqq y(x) \\
  z_{2}(x) &\coloneqq y^{\prime}(x) = z_{1}^{\prime}(x) \\
  z_{3}(x) &\coloneqq y^{\prime\prime}(x) = z_{2}^{\prime}(x) \\
&\dots \\
z_{p-2}(x) &\coloneqq y^{(p-3)}(x) = z_{p-3}^{\prime}(x) \\
z_{p-1}(x) &\coloneqq y^{(p-2)}(x) = z_{p-2}^{\prime}(x) \\
  z_{p}(x) &\coloneqq y^{(p-1)}(x) = z_{p-1}^{\prime}(x)
\end{align}
```

on peut ramener l'EDL régulière d'ordre $p$

```math
y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-2}(x)y^{\prime\prime}(x) + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
```

au SDL constitué de $p$ EDL du 1<sup>ère</sup> ordre&nbsp;:

```math
\left\{ \begin{aligned} 
  z_{p}^{\prime}(x) + a_{1}(x)z_{p}(x) + a_{2}(x)z_{p-1}(x) + \dots + a_{p-1}(x)z_{2}(x) + a_{p}(x)z_{1}(x) &= f(x) \\
  z_{p-1}^{\prime}(x) &= z_{p}(x) \\
  z_{p-2}^{\prime}(x) &= z_{p-1}(x) \\
                      &\dots \\
  z_{2}^{\prime}(x) &= z_{3}(x) \\
  z_{1}^{\prime}(x) &= z_{2}(x)
\end{aligned} \right.
```

ou encore

```math
\left\{ \begin{aligned}
    z_{1}^{\prime}(x) &= z_{2}(x) \\
    z_{2}^{\prime}(x) &= z_{3}(x) \\
                      &\dots \\
  z_{p-2}^{\prime}(x) &= z_{p-1}(x) \\
  z_{p-1}^{\prime}(x) &= z_{p}(x) \\
  z_{p}^{\prime}(x) + a_{1}(x)z_{p}(x) + a_{2}(x)z_{p-1}(x) + \dots + a_{p-1}(x)z_{2}(x) + a_{p}(x)z_{1}(x) &= f(x)
\end{aligned} \right.
```

### Passage d'une EDL du 2<sup>ème</sup> ordre à un SDL de 2 EDL du 1<sup>er</sup> ordre

Soit l'équation différentielle linéaire (EDL) scalaire du **2<sup>ème</sup> ordre**:

```math
a_{0}(x)y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = f(x)
```

où $a_{0}(x)$, $a_{1}(x)$, $a_{2}(x)$ et $f(x)$ sont des fonctions continues de $I \subseteq \mathbb{R}$ dans $\mathbb{K}$, $I$ étant connexe.

Sur tout intervalle où $a_{0}(x)$ ne s'annule pas, l'EDL peut se mettre sur la forme&nbsp;:

```math
y^{\prime\prime}(x) + \frac{a_{1}(x)}{a_{0}(x)}y^{\prime}(x) + \frac{a_{2}(x)}{a_{0}(x)}y(x) = \frac{f(x)}{a_{0}(x)}
```

ou encore

```math
y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = f(x)
```

en modifiant $a_{0}(x)$, $a_{1}(x)$, $a_{2}(x)$ et $f(x)$&nbsp;!

En posant $z_{k} \coloneqq y^{k-1}$ ou encore&nbsp;:

```math
\begin{align}
  z_{1}(x) &\coloneqq y(x) \\
  z_{2}(x) &\coloneqq y^{\prime}(x) = z_{1}^{\prime}(x)
\end{align}
```

on peut ramener l'EDL régulière d'ordre $2$

```math
y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = f(x)
```

au SDL constitué de $2$ EDL du 1<sup>ère</sup> ordre&nbsp;:

```math
\left\{ \begin{aligned} 
  z_{2}^{\prime}(x) + a_{1}(x)z_{2}(x) + a_{2}(x)z_{1}(x) &= f(x) \\
  z_{1}^{\prime}(x) &= z_{2}(x)
\end{aligned} \right.
```

ou encore

```math
\left\{ \begin{aligned}
  z_{1}^{\prime}(x) &= z_{2}(x) \\
  z_{2}^{\prime}(x) + a_{1}(x)z_{2}(x) + a_{2}(x)z_{1}(x) &= f(x)
\end{aligned} \right.
```

## Problème de Cauchy
