Python-TSNE
===========

Python library containing T-SNE algorithms.

Algorithms
----------

### Barnes-Hut-SNE

A python ([cython](http://www.cython.org)) wrapper for [Barnes-Hut-SNE](http://homepage.tudelft.nl/19j49/t-SNE.html) aka fast-tsne.

I basicly took [osdf code](https://github.com/osdf/py_bh_tsne) and made it pip compilant.

The wrapper was successfully tested on OSX (10.6/10.7), Ubuntu (11.04) and Arch Linux.

Requirements
------------

* [numpy](numpy.scipy.org)==1.7.1
* [scipy]()==0.12.0
* [cython](cython.org)===0.19.1
* [openblas](https://github.com/xianyi/OpenBLAS). Tested version is v0.2.5 and v0.2.6 (not necessary for OSX).

Installation
------------

`pip install tsne`

Usage
-----

Basic usage:

```
from tsne import bh_sne
X_2d = bh_sne(X)
```

[Iris example](http://nbviewer.ipython.org/urls/raw.github.com/danielfrg/py_tsne/master/examples/iris.ipynb)

More Information
----------------
See *Barnes-Hut-SNE*, L.J.P. van der Maaten. It is available on [arxiv](http://arxiv.org/abs/1301.3342).
