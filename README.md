# Équations différentielles linéaires

Soit l'***équation différentielle linéaire*** (EDL) suivante:

```math
a_{0}(x)y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
```

```math
y^{(p)}(x) + \frac{a_{1}(x)}{a_{0}(x)}y^{(p-1)}(x) + \frac{a_{2}(x)}{a_{0}(x)}y^{(p-2)}(x) + \dots + \frac{a_{p-1}(x)}{a_{0}(x)}y^{\prime}(x) + \frac{a_{p}(x)}{a_{0}(x)}y(x) = \frac{f(x)}{a_{0}(x)}
```

```math
y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
```

```math
\begin{align}
z_{1}(x) &= y(x) \\
z_{2}(x) &= y^{\prime}(x) = z_{1}^{\prime}(x) \\
z_{3}(x) &= y^{\prime\prime}(x) = z_{2}^{\prime}(x) \\
&\dots \\
z_{p-2}(x) &= y^{(p-3)}(x) = z_{p-3}^{\prime}(x) \\
z_{p-1}(x) &= y^{(p-2)}(x) = z_{p-2}^{\prime}(x) \\
z_{p}(x) &= y^{(p-1)}(x) = z_{p-1}^{\prime}(x)
\end{align}
```

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

---

Soit l'équation différentielle linéaire (EDL) du **premier order** suivante:

```math
a_{0}(x)y^{\prime}(x) + a_{1}(x)y(x) = f(x)
```

```math
y^{\prime}(x) + \frac{a_{1}(x)}{a_{0}(x)}y(x) = \frac{f(x)}{a_{0}(x)}
```

```math
y^{\prime}(x) + a_{1}(x)y(x) = f(x)
```

```math
\begin{align}
z_{1}(x) &= y(x)
\end{align}
```

```math
z_{1}^{\prime}(x) + a_{1}(x)z_{1}(x) = f(x)
```

---

Soit l'équation différentielle linéaire (EDL) du **second order** suivante:

```math
a_{0}(x)y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p-1}(x)y^{\prime}(x) + a_{p}(x)y(x) = f(x)
```

---

l'EDL ***homogène associée*** (EDLH) s'obtient  enreplaçant $b$ par la fonction nulle:

```math
a_{0}(x)y^{(p)}(x) + a_{1}(x)y^{(p-1)}(x) + a_{2}(x)y^{(p-2)}(x) + \dots + a_{p}(x)y(x) = 0
```

---

Soit l'équation différentielle linéaire (EDL) du premier ordre:

```math
a_{0}(x)y^{\prime}(x) + a_{1}(x)y(x) = f(x)
```

Soit l'équation différentielle linéaire homogène associée (EDLH) :

```math
a_{0}(x)y^{\prime}(x) + a_{1}(x)y(x) = 0
```

---

Soit l'équation différentielle linéaire (EDL) du second ordre:

```math
a_{0}(x)y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = b(x)
```

Soit l'équation différentielle linéaire homogène associée (EDLH) :

```math
a_{0}(x)y^{\prime\prime}(x) + a_{1}(x)y^{\prime}(x) + a_{2}(x)y(x) = 0
```

---

```math
y \mapsto Ly \coloneqq a_{0}y^{(p)} + a_{1}y^{(p-1)} + a_{2}y^{(p-2)} + \dots + a_{p}y
```
