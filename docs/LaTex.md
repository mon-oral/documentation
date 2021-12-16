[$\LaTeX$](https://fr.wikipedia.org/wiki/LaTeX) est, en premier lieu, un système de composition de documents mais sa syntaxe permet aussi de représenter des écritures scientifiques plus ou moins complexes (notations, équations, systèmes d'équations...).

L'intégration et l'écriture du code $\LaTeX$ sont simples  et il est inutile de maitriser l'ensemble de l'environnement $\LaTeX$ pour pouvoir utiliser sa syntaxe. La maitrise de quelques règles suffit pour pouvoir écrire des expressions mathématiques, physiques ou chimiques.

Vous trouverez ci-dessous une synthèse des éléments principaux à connaitre.


## 1. Déclaration du code Latex

Deux cas se présentent. Soit on souhaite écrire une formule ou une écriture scientifique simple au sein d'une ligne de texte (présentation en ligne), soit on souhaite présenter l'écriture scientifique centrée dans un nouveau paragraphe (présentation en paragraphe).

### 1.1. Présentation en ligne

Pour une présentation en ligne le code LaTeX doit être encadré par des `$`.

**Exemple**:

> `Ceci est une formule : $F(k) = \int_{-\infty}^{\infty} f(x) e^{2\pi i k} dx$`
> 
> Ceci est une formule : $F(k) = \int_{-\infty}^{+\infty} f(x) e^{2\pi i k} dx$
 

### 1.2. Présentation en paragraphe

Pour une présentation en paragraphe, le code LaTeX doit être encadré part des `$$` ou par `\begin{xxx} ... \end{xxx}` (avec xxx qui peut être `aligned`, `matrix`, `bmatrix`, `pmatrix`, `equation`, `eqnarray`...).


**Exemple 1** :

> `$$F(k) = \int_{-\infty}^{+\infty} f(x) e^{2\pi i k} dx$$`
> 
> $$F(k) = \int_{-\infty}^{+\infty} f(x) e^{2\pi i k} dx$$

**Exemple 2** :

> ```
> \begin{aligned}
> \dot{x} & = \sigma(y-x) \\
> \dot{y} & = \rho x - y - xz \\
> \dot{z} & = -\beta z + xy
> \end{aligned}
>```
> 
> $$
\begin{aligned}
\dot{x} & = \sigma(y-x) \\
\dot{y} & = \rho x - y - xz \\
\dot{z} & = -\beta z + xy
\end{aligned}
$$

**Exemple 3** : 

> ```
> \begin{matrix}
> 1&0&0\\
> 0&1&0\\
> 0&0&1\\
> \end{matrix}
> ``` 
>
> \begin{matrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{matrix}

**Exemple 4** : 

> ```
> \begin{bmatrix}
> 1&0&0\\
> 0&1&0\\
> 0&0&1\\
> \end{bmatrix}
> ``` 
>
> \begin{bmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{bmatrix}

**Exemple 5** :

> ```
> \begin{equation}
> \left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
> \end{equation}
> ```
>
> \begin{equation}
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
\end{equation}

**Exemple 6** :

> ```
> \begin{eqnarray}
> x' &=& &x \sin\phi &+& z \cos\phi \\
> z' &=& - &x \cos\phi &+& z \sin\phi \\
> \end{eqnarray}
>```
>
> \begin{eqnarray}
x' &=& &x \sin\phi &+& z \cos\phi \\
z' &=& - &x \cos\phi &+& z \sin\phi \\
\end{eqnarray}

## 2. Syntaxe

Les listes ci-dessous ne sont pas exhaustives.

### 2.1. Mathématiques et Physique

Vous pouvez aussi consulter cette [page](http://ftp.ktug.org/tex-archive/info/undergradmath/undergradmath.pdf).
 
 
| syntaxe              | résultat                           | 
|---------------- |----------------------- |
| `a_{n-1}`                | $a_{n-1}$                   |
| `a^{n+1}`                | $a^{n+1}$                  |
| `\frac{a}{b}`          | $\frac{a}{b}$            |
| `\frac{a}{b}`          | $\frac{a}{b}$            | 
| `\vect{a}`              | $\vec{a}$                     |
| `\sum_{k-1}^n`    | $\sum_{k-1}^n$       |
| `\prod_{k=1}^n`    | $\prod_{k=1}^n$    | 
| `\sqrt[3]{8}`         | $\sqrt[3]{8}$             |
| `\int`                      | $\int$                             |
| `\int_a^b`              | $\int_a^b$                   |
| `\sin`                      | $\sin$                             |
| `\cos`                      | $\cos$                            |
| `\tan`                      | $\tan$                            |
| `\lim_{x \to a}`      | $\lim_{x \to a}$   |
| `\mathbb{R}`        | $\mathbb{R}$             |
| `\mathbb{N}`        | $\mathbb{N}$             |
| `\mathbb{Z}`        | $\mathbb{Z}$             |
| `\times`                 | $\times$                       |
| `\gg`                      | $\gg$                             |
| `\geq`                    | $\geq$                           |
| `\leq`                     | $\leq$                             |
| `\neq`                    | $\neq$                          | 
| `\partial`              | $\partial$                    |
| `\approx`             | $\approx$                    |
| `\sim`                   | $\sim$                           |
| `\infty`                 | $\infty$                         |
| `\exists`              | $\exists$                       |
| `\in`                      | $\in$                              |
| `\notin`                 | $\notin$                       |
| `\cup`                   | $\cup$                           |
| `\cap`                   | $\cap$                           |
| `\subset`               | $\subset$                    |
| `\forall`                 | $\forall$                       |
| `\rightarrow`        | $\rightarrow$           |
| `\Rightarrow`       | $\Rightarrow$            |
| `\Leftrightarrow`  | $\Leftrightarrow$  |
| `\dot{a}`                 | $\dot{a}$                    |
| `\hat{a}`                 | $\hat{a}$                    |
| `\bar{a}`                 | $\bar{a}$                    |
| `\tilde{a}`               | $\tilde{a}$                  |
| `\cdot`                   | $\cdot$                         |
| `\cdots`                 | $\cdots$                        |
| `\vdots`                 | $\vdots$                        |
| `\ddots`                 | $\ddots$                        |
 
### 2.2. Chimie
 
| syntaxe                        | résultat                                      |
|--------------------- |----------------------------- |
| `Ca^{2+} `                     | $Ca^{2+}$                             |
| `H_{2}O `                       | $H_{2}O$                               |
| `H^{+}_{(aq)} `              | $H^{+}_{(aq)}$                |
| `30^{\circ}C`                 | $30^{\circ}C$                  |
| `\rightarrow`                | $\rightarrow$                   |
| `\rightleftharpoons`   | $\rightleftharpoons$  |

**Exemple** : `CH_{4(g)} + 20_{2(g)} \rightarrow CO_{2(g)} + 2H_{2}O_{(l)}`

**Résultat** : $CH_{4(g)} + 20_{2(g)} \rightarrow CO_{2(g)} + 2H_{2}O_{(l)}$

**Exemple** : `H_2O_{(l)} + H_2O_{(l)} \rightleftharpoons H_3O^{+}_{(aq)} + HO^{-}_{(aq)}`

**Résultat** : $H_2O_{(l)} + H_2O_{(l)} \rightleftharpoons H_3O^{+}_{(aq)} + HO^{-}_{(aq)}$

 ### 2.3. Lettres grecques
 
 
| syntaxe             | réultat                       |
|--------------- |------------------- |
| `\alpha`            | $\alpha$               |
| `\beta`              | $\beta$                  | 
| `\gamma`         | $\gamma$               |
| `\delta`              | $\delta$               | 
| `\epsilon`          | $\epsilon$          |
| `\varepsilon`     | $\varepsilon$  | 
| `\zeta`                | $\zeta$                 |
| `\eta`                  | $\eta$                   | 
| `\theta`              | $\theta$               |
| `\vartheta`        | $\vartheta$        | 
| `\iota`                | $\iota$                 |
| `\kappa`            | $\kappa$              | 
| `\lambda`          | $\lambda$           |
| `\mu`                 | $\mu$                      | 
| `\nu`                  | $\nu$                      |
| `\xi`                    | $\xi$                    | 
| `\pi`                   | $\pi$                     |
| `\varpi`             | $\varpi$              | 
| `\rho`                | $\rho$                   |
| `\varrho`           | $\varrho$           | 
| `\sigma`           | $\sigma$              |
| `\varsigma`      | $\varsigma$      | 
| `\tau`                | $\tau$                   |
| `\upsilon`         | $\upsilon$        | 
| `\phi`                | $\phi$                  |
| `\varphi`          | $\varphi$           |
| `\chi`                | $\chi$                  |
| `\psi`                | $\psi$                  |
| `\omega`         | $\omega$             |
| `\Gamma`       | $\Gamma$             |
| `\Delta`           | $\Delta$             |
| `\Theta`          | $\Theta$             |
| `\Lambda`      | $\Lambda$          |
| `\Xi`                 | $\Xi$                    |
| `\Pi`                  | $\Pi$                   |
| `\Sigma`          | $\Sigma$            |
| `\Upsilon`       | $\Upsilon$       |
| `\Phi`               | $\Phi$                 |
| `\Psi `              | $\Psi$                 |
| `\Omega`        | $\Omega$            |


## 3. Autres exemples

**Exemple** :
`$$\left( \frac{p}{q} \right)$$`

**Résultat** :

$$\left( \frac{p}{q} \right)$$

<br />

**Exemple** :
`$$f'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$$`

**Résultat** :
$$f'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$$

<br />

**Exemple** :
`$$e^x = \sum_{k=0}^{\infty} \frac{x^k}{k!}$$`

**Résultat** :
$$e^x = \sum_{k=0}^{\infty} \frac{x^k}{k!}$$

<br />

**Exemple** :
```
$$
\begin{bmatrix}
\frac{\partial f_1}{\partial x_1} & \cdots &
\frac{\partial f_1}{\partial x_n} \\
\vdots & \ddots & \vdots \\
\frac{\partial f_m}{\partial x_1} & \cdots &
\frac{\partial f_m}{\partial x_n}
\end{bmatrix}
$$
```

**Résultat** :
$$
\begin{bmatrix}
\frac{\partial f_1}{\partial x_1} & \cdots &
\frac{\partial f_1}{\partial x_n} \\
\vdots & \ddots & \vdots \\
\frac{\partial f_m}{\partial x_1} & \cdots &
\frac{\partial f_m}{\partial x_n}
\end{bmatrix}
$$

<br />


**Exemple** :
`$$K_a  = \frac{{\left[ {H^ +  } \right]\left[ {A^ -  } \right]}}{{\left[ {HA} \right]}}$$`

**Résultat** :
$$K_a  = \frac{{\left[ {H^ +  } \right]\left[ {A^ -  } \right]}}{{\left[ {HA} \right]}}$$

<br />

**Exemple** :
`$$x = \frac {-b \pm \sqrt{b^2 -4ac}} {2a}$$`

**Résultat** :
$$x = \frac {-b \pm \sqrt{b^2 -4ac}} {2a},$$

<br />

**Exemple** :
`$$\left\| \frac a b \right\|$$`

**Résultat** :
$$\left\| \frac a b \right\|$$

<br />

**Exemple** :
```
\begin{eqnarray}
  & f={1}/{T} \quad \omega={2\pi}/{T}=2\pi f = \sqrt{{k}/{m}} & \\
  & \left\{ \begin{array}{l}
  x = A \cos\phi = A \cos \omega t,    \\
  v = -A \omega \sin\omega t            \\
  a = -A \omega^2 \cos\omega t
  \end{array} \right. &
\end{eqnarray}
```

**Résultat** :
\begin{eqnarray}
  & f={1}/{T} \quad \omega={2\pi}/{T}=2\pi f = \sqrt{{k}/{m}} & \\
  & \left\{ \begin{array}{l}
  x = A \cos\phi = A \cos \omega t,    \\
  v = -A \omega \sin\omega t            \\
  a = -A \omega^2 \cos\omega t
  \end{array} \right. &
\end{eqnarray}
