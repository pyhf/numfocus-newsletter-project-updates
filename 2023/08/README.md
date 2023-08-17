# [August 2023][newsletter] pyhf Project Update

We're happy to announce that [pyhf v0.7.3](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.3) is out on PyPI and Conda-forge ([Tweet](https://twitter.com/pyhf_/status/1692258901142413786))!
This is a small patch release with the following highlights:

* Use [`np.prod`](https://numpy.org/doc/stable/reference/generated/numpy.prod.html#numpy.prod) API over `np.product` as `np.product` is [deprecated as of NumPy `v1.25.0`](https://numpy.org/devdocs/release/1.25.0-notes.html#deprecations).
* Guard [`pyhf.optimize.opt_minuit.minuit_optimizer`](https://pyhf.readthedocs.io/en/v0.7.3/_generated/pyhf.optimize.opt_minuit.minuit_optimizer.html#pyhf.optimize.opt_minuit.minuit_optimizer) optimizer strategy from `None` to ensure [`iminuit.Minuit.strategy`](https://iminuit.readthedocs.io/en/stable/reference.html#iminuit.Minuit.strategy) strategies are correctly handled.

Please see the [release notes](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.3) for a full list of changes.

[newsletter]: https://numfocus.salsalabs.org/numfocus__newsletter_aug2023
