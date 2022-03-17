---
layout: post
title: "Organiser son depot github comme un package python"
date: 2021-09-17 17:12:37 +0200
categories: python git github
---

```bash
pip install git+https://github.com/UTILISATEUR/DEPOT
```

```
mon_package/
    sources ...
MANIFEST.in
setup.py
```

Dans le `setup.py` :
```python
from setuptools import setup

setup(
    TODO
)
```
