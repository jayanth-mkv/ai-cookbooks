# Machine Learning & Data Science Cookbooks

A learning collection for studying classical machine-learning algorithms, neural-network fundamentals, preprocessing, relational data workflows, reinforcement learning, and scikit-learn.

> [!NOTE]
> This is a learning collection, not a single installable Python package. Environments and datasets vary, so review each exercise's imports, services, and paths before running it.

## Learning catalog

| Area | Included material |
| --- | --- |
| Neural networks | Perceptron, backpropagation, and practice notebooks |
| Supervised learning | Linear regression, regression trees, decision trees, K-nearest neighbors, and Naive Bayes |
| Optimization | Gradient-descent examples |
| Reinforcement learning | Q-learning |
| NLP | Sentiment-analysis notebook |
| Data preparation | Preprocessing and Colab practice |
| Data engineering | [Relational filtering, PostgreSQL queries, CTEs, and entity-attribute-value pivots](data-engineering/relational-query-playbooks/) |
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

Some exercises may need extra packages, downloaded datasets, a local PostgreSQL service, or compatibility changes that are not covered by the baseline command.

## How to use this repository

1. Pick a topic directory rather than running the full collection at once.
2. Read the notebook or script from top to bottom and inspect data paths and service settings before execution.
3. Restart the kernel and run all cells when validating a notebook.
4. Record any additional dependency versions beside the exercise when updating it.

## Maintenance status

This repository is retained as a growing cookbook. The relational query exercises were consolidated from the former [`ai-research-playbooks`](https://github.com/jayanth-mkv/ai-research-playbooks) repository, which remains available as the original historical record.

Useful future improvements include a shared environment file, per-exercise runtime notes, dataset provenance, cleaned notebook outputs, and automated execution checks.

## Limitations

- Dependencies and Python versions are not pinned.
- Notebook outputs are historical and are not proof that every exercise runs on a current environment.
- The collection mixes from-scratch exercises with library-based examples; inspect the implementation before reusing it.
- The PostgreSQL examples contain local placeholder connection values and expect a separately prepared database; replace them before use.
