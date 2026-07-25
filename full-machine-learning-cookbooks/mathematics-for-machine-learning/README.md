<div align="center">

# Mathematics for Machine Learning — Course Cookbooks

**Eight legacy practice notebooks covering linear algebra and multivariate calculus, plus principal-component-analysis references.**

[Notebook catalog](#notebook-catalog) · [Quick start](#quick-start) · [Compatibility](#compatibility-and-missing-course-files) · [Limitations](#limitations)

</div>

## What is included?

This directory preserves course-work exercises for mathematical ideas commonly used in machine learning. The notebooks are learning material—not a Python library, a complete course, or a verified modern training environment.

The original Git tree used colons in all three course directory names. Those paths could not be checked out on Windows. They have been replaced with portable lowercase, hyphenated directories while preserving the original notebook blobs byte-for-byte.

## Notebook catalog

### Linear algebra

| Notebook | Topic |
| --- | --- |
| [Gram–Schmidt process](mathematics-linear-algebra/gram-schmidt-process.ipynb) | Build an orthonormal basis and use it to determine dimensionality |
| [PageRank](mathematics-linear-algebra/page-rank.ipynb) | Explore eigenvectors, transition matrices, and the PageRank iteration |
| [Reflecting Bear](mathematics-linear-algebra/reflecting-bear.ipynb) | Construct a reflection transformation in a nonstandard basis |

### Multivariate calculus

| Notebook | Topic |
| --- | --- |
| [Backpropagation](mathematics-multivariate-calculus/backpropagation.ipynb) | Train a small neural network to represent a two-dimensional curve |
| [Fitting a height distribution](mathematics-multivariate-calculus/fitting-height-distribution.ipynb) | Fit a Gaussian model with steepest descent |
| [Gradient descent sandpit](mathematics-multivariate-calculus/gradient-descent-sandpit.ipynb) | Develop intuition for gradients and local descent |
| [The Sandpit](mathematics-multivariate-calculus/sandpit.ipynb) | Explore Jacobians and multivariable optimization visually |
| [The Sandpit — Part 2](mathematics-multivariate-calculus/sandpit-part-2.ipynb) | Examine harder descent scenarios and common limitations |

### Principal component analysis

[PCA resources](mathematics-pca/resources.txt) contains historical links to the associated notebook download and offline-environment instructions. Those external resources may change or disappear.

## Quick start

Python 3.9 or 3.10 is recommended for the legacy NumPy compatibility range.

```bash
git clone https://github.com/jayanth-mkv/full-machine-learning-cookbooks.git
cd full-machine-learning-cookbooks/mathematics-for-machine-learning
python -m venv .venv
```

Activate the environment:

```bash
# Linux or macOS
source .venv/bin/activate

# Windows PowerShell
.venv\Scripts\Activate.ps1
```

Then install the compatibility baseline and start JupyterLab:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

The environment describes the imports visible in the repository. It has not been presented as a guarantee that every historical cell executes successfully.

## Suggested learning path

1. Start with Gram–Schmidt and Reflecting Bear.
2. Continue to PageRank for an eigenvector application.
3. Work through the first Sandpit notebook and its gradient-descent companion.
4. Continue with height-distribution fitting and Sandpit Part 2.
5. Finish with the backpropagation exercise and PCA references.

## Compatibility and missing course files

- PageRank imports `readonly.PageRankFunctions`, Reflecting Bear imports `readonly.bearNecessities`, and the height-distribution exercise imports `readonly.HeightsModule`. Those course-provided modules are not tracked here, so the affected notebooks are incomplete offline.
- Several historical cells use `np.float`, which was removed in NumPy 1.24. The compatibility file therefore keeps NumPy below 1.24.
- Notebook outputs were preserved as learning context. They do not prove clean execution with the documented environment.
- The old colon-containing paths no longer exist on the current branch, so normal Windows cloning is supported.

## Repository layout

```text
mathematics-linear-algebra/          3 notebooks
mathematics-multivariate-calculus/   5 notebooks
mathematics-pca/                     historical resource links
requirements.txt                     legacy local baseline
```

## Consolidation status

This material is maintained inside [`full-machine-learning-cookbooks`](https://github.com/jayanth-mkv/full-machine-learning-cookbooks). It was consolidated from [`ml-courses-cookbooks`](https://github.com/jayanth-mkv/ml-courses-cookbooks), which preserves the original standalone history.

## Limitations

- Dataset, exercise, and helper-module provenance should be confirmed before redistribution.
- No automated notebook execution or output comparison is configured.
- The PCA section currently contains links rather than tracked notebooks.
- Some external links and course-specific instructions may be outdated.
- There is no license file; source availability does not grant permission to reuse the material.
