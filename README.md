# 🤖 AI-Learning-Lab

> 6-month AI/ML learning journey with production-grade workflows

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

## 📋 Overview

AI-Learning-Lab is a comprehensive learning environment focused on modern AI/ML engineering practices, with emphasis on:

- **LLM APIs**: Integration with OpenAI, Anthropic, and open-source models
- **RAG Systems**: Retrieval-Augmented Generation pipelines
- **Agentic AI**: Building autonomous AI agents and workflows
- **Production ML**: MLOps, experiment tracking, and deployment

## 🚀 Quick Start

### Prerequisites

- Python 3.11 or higher
- Git
- Virtual environment manager (venv, conda, or poetry)

### Installation

```bash
# Clone the repository
git clone https://github.com/fordjes/AI-Learning-Lab.git
cd AI-Learning-Lab

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements/base.txt
pip install -r requirements/ml.txt
pip install -r requirements/dev.txt  # For development

# Set up environment variables
cp .env.example .env
# Edit .env with your API keys
```

## 📁 Project Structure

```
AI-Learning-Lab/
├── .github/              # GitHub workflows and templates
│   ├── workflows/        # CI/CD pipelines
│   ├── ISSUE_TEMPLATE/   # Issue templates
│   └── pull_request_template.md
├── data/                 # Data storage (gitignored)
│   ├── raw/             # Original, immutable data
│   ├── processed/       # Cleaned, transformed data
│   └── external/        # External datasets
├── src/                  # Source code
│   ├── data/            # Data loading and processing
│   ├── features/        # Feature engineering
│   ├── models/          # Model definitions
│   ├── evaluation/      # Model evaluation utilities
│   ├── visualization/   # Plotting and visualization
│   └── utils/           # Utility functions
├── tests/               # Test suite
│   ├── unit/           # Unit tests
│   └── integration/    # Integration tests
├── experiments/         # Experiment tracking
├── notebooks/          # Jupyter notebooks for exploration
├── scripts/            # Standalone scripts
├── configs/            # Configuration files
├── requirements/       # Dependency specifications
├── reports/            # Generated analysis and reports
└── models/             # Trained models (gitignored)
```

## 🔧 Development Workflow

### 1. Create a Branch

```bash
git checkout -b feature/your-feature-name
```

### 2. Make Changes

Follow the coding standards:
- Use `black` for formatting: `black src/`
- Use `ruff` for linting: `ruff check src/`
- Type hints with `mypy`: `mypy src/`
- Run tests: `pytest tests/`

### 3. Commit Changes

```bash
git add .
git commit -m "feat: add your feature description"
```

Commit message conventions:
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `test:` Test additions or changes
- `refactor:` Code refactoring
- `chore:` Maintenance tasks

### 4. Push and Create PR

```bash
git push origin feature/your-feature-name
```

Then create a Pull Request on GitHub.

## 🧪 Experiments

All experiments are tracked using MLflow:

```python
import mlflow

with mlflow.start_run():
    mlflow.log_params({"learning_rate": 0.001})
    # Your training code
    mlflow.log_metrics({"accuracy": 0.95})
```

View experiments: `mlflow ui`

## 🔗 Integration Links

- **Project Management**: [Linear Board](https://linear.app)
- **Documentation**: [Notion Workspace](https://notion.so)
- **Experiments**: MLflow UI (local)

## 📚 Learning Resources

- [Anthropic Documentation](https://docs.anthropic.com)
- [OpenAI API Reference](https://platform.openai.com/docs)
- [LangChain Documentation](https://python.langchain.com)
- [MLflow Documentation](https://mlflow.org/docs/latest/index.html)

## 🤝 Contributing

This is a personal learning project, but feedback and suggestions are welcome! Please:

1. Open an issue for bugs or feature requests
2. Follow the PR template for contributions
3. Ensure all tests pass before submitting

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎯 Learning Goals

- [ ] Master LLM API integration patterns
- [ ] Build production-ready RAG systems
- [ ] Implement autonomous AI agents
- [ ] Establish MLOps best practices
- [ ] Deploy models to production
- [ ] Create comprehensive documentation

---

**Status**: 🚧 Active Development | **Started**: November 2025 | **Duration**: 6 months
