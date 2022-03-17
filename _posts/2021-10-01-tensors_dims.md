---
layout: post
title: "Organiser son depot github comme un package python"
date: 2021-09-17 17:12:37 +0200
categories: python
---

Quand on commence à manipuler des données en grand nombre, on se retrouve souvent à manipuler des tenseurs.
Du moins, c'est le cas en Machine Learning.

# Broadcasting
Le broadcasting désigne les traitements effectués implicitement pour permettre des opérations entre deux tenseurs.

Par exemple, si on tente d'additionner le vecteur (1, 1, 1) à la matrice $$((2, 2, 2), (3, 3, 3))$$, ce n'est normalement pas possible.
Pour autant, l'addition de ces deux valeurs en numpy va donner quelques chose :
```python
>>> import numpy as np
>>> a = np.array([1, 1, 1])
>>> b = np.array([[2, 2, 2], [3, 3, 3]])
>>> a + b
array([[3, 3, 3],
	   [4, 4, 4]])
```

