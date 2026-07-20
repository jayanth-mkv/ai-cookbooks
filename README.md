# Machine Learning Cookbooks

A notebook collection for studying classical machine-learning algorithms, neural-network fundamentals, preprocessing, reinforcement learning, and scikit-learn workflows.

> [!NOTE]
> This is a learning archive, not a single installable Python package. Notebook environments and datasets vary, so review each notebook's imports and paths before running it.

## Notebook catalog

| Area | Included material |
| --- | --- |
| Neural networks | Perceptron, backpropagation, and practice notebooks |
| Supervised learning | Linear regression, regression trees, decision trees, K-nearest neighbors, and Naive Bayes |
| Optimization | Gradient-descent examples |
| Reinforcement learning | Q-learning |
| NLP | Sentiment-analysis notebook |
| Data preparation | Preprocessing and Colab practice |
| Libraries | scikit-learn exercises and a combined `Complete.ipynb` notebook |

## Getting started

Create an isolated notebook environment, then install dependencies as the selected notebook requires:

```bash
git clone https://github.com/jayanth-mkv/full-machine-learning-cookbooks.git
cd full-machine-learning-cookbooks
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install jupyterlab numpy pandas matplotlib scikit-learn
jupyter lab
```

Some notebooks may need extra packages, downloaded datasets, or compatibility changes that are not covered by the baseline command.

## How to use this repository

1. Pick a topic directory rather than running the full collection at once.
2. Read the notebook from top to bottom and inspect data paths before execution.
3. Restart the kernel and run all cells to check reproducibility.
4. Record any additional dependency versions beside the notebook when updating it.

## Maintenance status

This repository is retained as a growing cookbook. Useful future improvements include a shared environment file, per-notebook runtime notes, dataset provenance, cleaned output cells, and automated notebook execution checks.

## Limitations

- Dependencies and Python versions are not pinned.
- Notebook outputs are historical and are not proof that every notebook runs on a current environment.
- The collection mixes from-scratch exercises with library-based examples; inspect the implementation before reusing it.

