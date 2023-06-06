# [June 2023][newsletter] pyhf Project Update

We're happy to announce that [pyhf v0.7.2](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2) is out on PyPI and Conda-forge ([Tweet](https://twitter.com/pyhf_/status/1659575568143200258))!
This is a small patch release with the following highlights:

* Guard against modifiers like shapefactor, shapesys, and staterror from being used as parameters of interest by raising a pyhf.exceptions.InvalidModel if a multiple component parameter of interest is used.
* Use typing.TYPE_CHECKING guard to avoid causing a ModuleNotFoundError when the version of NumPy installed is older than v1.21.0, which is the first NumPy release to include [numpy.typing](https://numpy.org/doc/stable/reference/typing.html#module-numpy.typing) (with numpy.typing.NDArray support).

Please see the [release notes](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.2) for a full list of changes.

[newsletter]: https://numfocus.salsalabs.org/numfocus__newsletter_june2023

