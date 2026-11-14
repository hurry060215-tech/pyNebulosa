# py-nebulosa-omicverse

An independently maintained packaging of patched [pyNebulosa](https://github.com/mdmanurung/pyNebulosa) for OmicVerse integration. Distribution: `py-nebulosa-omicverse`; import: `ov_nebulosa`. It does not install or overwrite the upstream `pynebulosa` namespace. Original attribution and license are retained.

## Status and installation

Version 0.1.0 is a candidate, not yet published to PyPI. Build and install this checkout for validation:

```sh
python -m pip install ".[test]"
python -m pytest -q
```

The reference comparison covers the patched weighted grid and cell mapping at an explicitly supplied bandwidth. Silverman and scipy ks approximations are not certified as equivalent to the R defaults. Upstream plotting/API behavior is retained; this is not a new biological method.

## Provenance

Validated base: `3f2678cb7b0825e669608e8734d894f6598efd86`. See [attribution](ATTRIBUTION.md), the unchanged [license](LICENSE), and [upstream documentation](UPSTREAM_README.md) for history. The historical upstream README/Conda recipe refers to the original distribution, not this candidate. This variant is not affiliated with or endorsed by the upstream authors.

## Release validation

CI builds a wheel from the source archive, installs it, and runs the retained reference tests outside the checkout. See [release instructions](RELEASE.md). Coexistence with the upstream distribution must pass before release. No numerical gate is widened.
