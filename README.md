<div align="center">
  <h1>AI Cookbooks</h1>
  <p><strong>A growing library of practical learning paths across foundational, applied, and generative AI.</strong></p>
  <p>Learning material for exploration and study—not a single installable package or unified production system.</p>

  [![Jupyter notebooks](https://img.shields.io/badge/Jupyter-notebook%20collections-F37626?logo=jupyter&logoColor=white)](#collections)
  [![Machine learning](https://img.shields.io/badge/track-machine%20learning-3776AB)](full-machine-learning-cookbooks/)
  [![Generative AI](https://img.shields.io/badge/track-generative%20AI-8B5CF6)](generative-ai-cookbooks/)

  [Collections](#collections) · [Start here](#start-here) · [Repository layout](#repository-layout) · [Reproducibility](#reproducibility-status)
</div>

## What is this?

AI Cookbooks brings two complementary learning collections into one repository while keeping their original folder boundaries and Git history intact:

- **Machine learning cookbooks** cover mathematics, classical algorithms, neural-network fundamentals, data preparation, data engineering, reinforcement learning, and scikit-learn.
- **Generative AI cookbooks** cover federated learning and the data, model, training, and evaluation stages of LLM pre-training.

Each notebook or exercise should be treated as an independent learning unit. Review its code, dataset requirements, and runtime assumptions before running it.

Topics and implementations can grow over time; the repository is organized to keep each learning path discoverable without presenting the collection as one fixed curriculum or runtime.

## Catalog direction

Future tracks can cover additional AI concepts, implementation patterns, and applied learning material. A topic is added only when its notebooks or source material are committed and its place in the catalog is documented; the collections below describe what is available today.

## Collections

| Collection | Covers | Start here |
| --- | --- | --- |
| [Machine Learning Cookbooks](full-machine-learning-cookbooks/) | Linear algebra, calculus, PCA, regression, trees, KNN, Naive Bayes, perceptrons, backpropagation, Q-learning, sentiment analysis, preprocessing, relational data workflows, and scikit-learn. | [Collection guide](full-machine-learning-cookbooks/README.md) |
| [Generative AI Cookbooks](generative-ai-cookbooks/) | Federated learning with Flower plus six progressive notebooks on LLM pre-training. | [Collection guide](generative-ai-cookbooks/README.md) |

### Suggested learning paths

| Goal | Recommended route |
| --- | --- |
| Build ML foundations | Start with [mathematics for machine learning](full-machine-learning-cookbooks/mathematics-for-machine-learning/), then work through preprocessing, regression, trees, KNN, and Naive Bayes. |
| Understand neural-network mechanics | Explore the perceptron and backpropagation notebooks, then the multivariate-calculus exercises. |
| Work with data systems | Use the relational query playbooks under [data engineering](full-machine-learning-cookbooks/data-engineering/relational-query-playbooks/). |
| Learn distributed ML | Follow the five [federated-learning](generative-ai-cookbooks/federated-learning/) notebooks in order. |
| Learn the LLM pre-training lifecycle | Follow [pre-training-llm](generative-ai-cookbooks/pre-training-llm/) from data preparation through evaluation. |

## Start here

Clone the repository and launch Jupyter from the collection you want to explore:

```bash
git clone https://github.com/jayanth-mkv/ai-cookbooks.git
cd ai-cookbooks
python -m venv .venv
# Windows PowerShell: .\.venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
python -m pip install jupyterlab
jupyter lab
```

Install additional libraries only after inspecting the selected notebook. Some exercises require packages such as NumPy, pandas, scikit-learn, Flower, or a local PostgreSQL service; the repository does not claim a tested global dependency set.

## Repository layout

```text
ai-cookbooks/
├── full-machine-learning-cookbooks/  # classical ML, mathematics, data, and RL
└── generative-ai-cookbooks/           # federated learning and LLM pre-training
```

The folder names intentionally preserve the source collection identities. They are organizational boundaries, not separately deployed applications.

## Reproducibility status

| Area | Status |
| --- | --- |
| Notebook source | Available in both collections. |
| Shared root environment | Not provided; dependencies differ by notebook. |
| Dataset and service access | Required by selected notebooks; inspect code before execution. |
| Automated notebook execution | Not configured. |
| Production readiness | Out of scope; this is a learning repository. |

## Responsible use

- Run notebooks in an isolated environment.
- Do not commit local credentials, datasets with restricted terms, or generated training artifacts.
- Check source licenses and course acknowledgements inside individual tracks before reusing material.
- Treat historical notebook outputs as examples, not proof of compatibility with current libraries.
