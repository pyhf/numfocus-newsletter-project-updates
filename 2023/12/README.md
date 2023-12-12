# [December 2023][newsletter] pyhf Project Update

We're happy to announce that [pyhf v0.7.4](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.4) and [pyhf v0.7.5](https://github.com/scikit-hep/pyhf/releases/tag/v0.7.5) are out on PyPI and Conda-forge!
These releases are small patch releases with the following highlights:

* v0.7.4:
   - Skip callbacks with dead weakrefs while iterating over callbacks in `pyhf` events, like [`pyhf.set_backend`](https://pyhf.readthedocs.io/en/v0.7.4/_generated/pyhf.set_backend.html), to avoid the possibility of accessing dead weakrefs before they could be garbage collected.

   The fixed bug was subtle and occurred nondeterministically when the [`pyhf.tensorlib`](https://pyhf.readthedocs.io/en/v0.7.4/_generated/pyhf.tensorlib.html) was changed repeatedly causing dead weakrefs to be accessed before Python's garbage collection could remove them. Most users should be unaffected.
* v0.7.5:
   - Remove operating system dependent components of schema validation to allow for validation on Windows.

   This release is the first to support the pyhf Python API on Windows, though the command line API is not yet fully supported.


Please see the [release notes](https://github.com/scikit-hep/pyhf/releases/) for a full list of changes.

## Event followup

* Following the inaugural [pyhf Users and Developers Workshop](https://indico.cern.ch/event/1294577/) earlier this December, the recorded workshop sessions will be captioned and uploaded to the [IRIS-HEP YouTube channel](https://www.youtube.com/@iris-hep/videos) later this month.

[newsletter]: https://numfocus.salsalabs.org/numfocus__newsletter_dec2023
