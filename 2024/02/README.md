# [February 2024][newsletter] pyhf Project Update

We're happy to announce that [pyhf v0.7.6](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.6) is out on PyPI and Conda-forge!
This is a small patch release with the following highlights:

* For the JAX backend access `jax.config` from the `jax` top level API to avoid support issues with `jax` and `jaxlib` `v0.4.20+`.
* Add information in the warnings for [`pyhf.infer.test_statistics.qmu`](https://pyhf.readthedocs.io/en/v0.7.6/_generated/pyhf.infer.test_statistics.qmu.html#pyhf.infer.test_statistics.qmu) and [`pyhf.infer.test_statistics.qmu_tilde`](https://pyhf.readthedocs.io/en/v0.7.6/_generated/pyhf.infer.test_statistics.qmu.html#pyhf.infer.test_statistics.qmu_tilde) that provides users with the higher level `pyhf.infer` APIs `kwarg` to set the correct test statistic.
* Correct the variable assignment for the one-sigma and two-sigma limit band artists in [`pyhf.contrib.viz.brazil.plot_brazil_band`](https://pyhf.readthedocs.io/en/v0.7.6/_generated/pyhf.contrib.viz.brazil.plot_brazil_band.html#pyhf.contrib.viz.brazil.plot_brazil_band) to match the stated return structure.

Please see the [release notes](https://github.com/scikit-hep/pyhf/releases/) for a full list of changes.

[newsletter]: https://numfocus.medium.com/whats-new-with-numfocus-projects-february-2024-fe253a5e843a
