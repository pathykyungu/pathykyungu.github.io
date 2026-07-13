# Calcul Sommatiel et Formules de Kyungu
### Par Pathy Kyungu Ngoïe

Ce dépôt présente les fondements théoriques de **l'Analyse Sommatielle**, ainsi que les méthodes d'inversion des transformées de Laplace et de Mellin développées par **Pathy Kyungu Ngoïe**. Ces travaux offrent un pont analytique entre les sommes discrètes, les intégrales continues et les distributions.

---

## 1. La Formule de Kyungu (Laplace Inverse)

Pour une fonction auxiliaire $\varphi(x) = F(1/x)$ analytique en $x=0$, la transformée de Laplace inverse s'exprime sous forme de série :

$$\mathcal{L}^{-1}\[F\](t) = \varphi(0)\delta(t) + \sum_{n=1}^{\infty}\frac{n}{(n!)^2} \varphi^{(n)}(0)t^{n-1}$$

### Forme Intégrale de la formule de Kyungu pour l'inversion de Laplace
$$\mathcal{L}^{-1}\[F\](t) = \frac{1}{2 \pi i} \oint_{\Gamma} \frac{\varphi(z)}{z^2} e^{t/z} dz$$

---

## 2. Le Sommatiel

Le sommatiel $S(x)$, noté $\[F]\_x$, est le prolongement analytique de la somme discrète $\sum\_{k=1}^{n} F(k)$ aux valeurs réelles ou complexes de $x$.

### Représentation intégrale
Le sommatiel admet une représentation intégrale s'établissant de l'origine gauche à l'infini positif :

$$ S(x) =\[F(x)]\_x = \int_{0^-}^{+\infty} \frac{1 - e^{-xt}}{e^t - 1} \mathcal{L}^{-1}\[F\](t)dt $$

*Note topologique : L'intégration réelle est étendue discrètement sur* $\mathbb{R}^-$ *par de petits contours isolés pour envelopper les singularités réelles négatives s'il en existe, neutralisant ainsi toute divergence vers l'infini négatif.*

## 3. L'Hypersommatiel $F,(s)$

L'hypersommatiel est défini comme la limite paramétrique du sommatiel. Sa notation spécifique utilise la virgule $F,(s)$ jouant le même rôle conceptuel que l'apostrophe $F'(x)$ pour la dérivée classique.

### Définition limite

$$ F,(s) = \lim_{x \to 0} \frac{[F(sx)]_x}{x} $$

### Le Critère de Licité (Hyperconvergence)
L'hypersommatiel est un operateur lineaire. l'operation terme à terme de cet outil mathematique devient delicate pour une serie de Taylor : La fonction doit être hyperconvergente: le rayon de convergence de la série hypersommée obtenue doit être non nul. Dans le cas des fonctions impaires, 
l'effacement structurel des monômes (notamment de degré impair $\ge 3$) dans la serie de Taylor, masque l'information analytique sur l'hyperconvergence, et le critère d'hyperconvergence s'étudie sur la dérivée $F'(s)$. En cas d'hyperdivergence, le recours à la formule intégrale complexe est obligatoire.

### Représentation intégrale de l'hypersommatiel
La forme  integrale de l'hypersommatiel s'énonce par :

$$ F,(s) = \int_{0^-}^{+\infty} \frac{\mathcal{L}^{-1}\[F\](t)}{e^{st} - 1} tdt $$

## 4. Formule d’Euler–Maclaurin Généralisée (Kyungu)

Cette formule étend la relation classique d'Euler-Maclaurin en introduisant un paramètre de décalage $c$ et les polynômes de Bernoulli $B_n(c)$ :

$$\sum_{k=a+c}^{b+c-1} F(k) = \int_{a}^{b} F(t)dt + \sum_{n=1}^{\infty} \frac{B_n(c)}{n!} \big(F^{(n-1)}(b) - F^{(n-1)}(a) \big)$$

---

## 5. Publications Officielles et Références (DOI)

Pour citer ces travaux, veuillez vous référer aux publications suivantes :

*   **Théorie Unifiée** : Kyungu, P. (2026). *Analyse Sommatielle : Théorie unifiée de la sommation et de l'intégration*. [DOI: 10.5281/zenodo.18517761](https://doi.org/10.5281/zenodo.18517761)
*   **Hypersommatiel** : Kyungu, P. (2025). *L'Hypersommatiel : un nouvel outil mathématique — Une transformée de Kyungu à support zêta*. [DOI: 10.5281/zenodo.17692063](https://doi.org/10.5281/zenodo.17692063)
*   **Calcul Sommatiel** : Kyungu, P. (2025). *Le Calcul Sommatiel : de l'intuition adolescente aux développements modernes*. [DOI: 10.5281/zenodo.17566411](https://doi.org/10.5281/zenodo.17566411)
*   **Euler-Maclaurin** : Kyungu, P. (2025). *Généralisation de la Formule d'Euler-Maclaurin*. [DOI: 10.5281/zenodo.17505791](https://doi.org/10.5281/zenodo.17505791)
*   **Laplace Inverse** : Kyungu, P. (2025). *Detailed Presentation of Kyungu's Formula for the Inverse Laplace Transform*. [DOI: 10.5281/zenodo.17341923](https://doi.org/10.5281/zenodo.17341923)
*   **Hypothèse de Riemann** : Kyungu, P. (2025). *Une étude de la fonction zêta et proposition d'une preuve de l'hypothèse de Riemann*. [DOI: 10.5281/zenodo.17389226](https://doi.org/10.5281/zenodo.17389226)

---

## Domaines d'application
- **Physique Théorique** : Analyse des singularités essentielles.
- **Théorie des Nombres** : Étude de la fonction Zêta de Riemann.
- **Calcul Numérique** : Convergence accélérée des transformées inverses.

---
© 2025-2026 Pathy Kyungu Ngoïe. Tous droits réservés.
