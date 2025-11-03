# 🤖 AI-Learning-Lab

> 6-month AI/ML learning journey with production-grade workflows

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

## 📋 Overview

AI-Learning-Lab is a comprehensive 6-month learning environment focused on modern AI/ML engineering practices with integrated project management and documentation workflows.

### What You'll Build
- **LLM APIs**: Integration with Anthropic Claude and OpenAI
- **RAG Systems**: Production-grade Retrieval-Augmented Generation
- **Agentic AI**: Autonomous AI agents and multi-agent systems
- **Production ML**: MLOps, experiment tracking, and deployment

### Integrated Workflow
- **GitHub**: Code repository and version control
- **Linear**: Issue tracking and project management
- **Notion**: Experiment documentation and learning journal

## 🚀 Getting Started

### Day 1: Environment Setup

#### 1. Prerequisites
- Python 3.11 or higher
- Git installed
- GitHub account (connected)
- Linear workspace (connected)
- Notion workspace (connected)

#### 2. Clone and Setup
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
# Edit .env with your API keys (Anthropic, OpenAI, etc.)
```

#### 3. Verify Setup
```bash
# Check Python version
python --version  # Should be 3.11+

# Verify Anthropic SDK
python -c "import anthropic; print('Anthropic SDK installed!')"

# Run tests
pytest tests/ -v
```

### Your First Issue (YEP-5: Set up development environment)

#### Step 1: Open in Linear
1. Visit: https://linear.app/yep-learn-ai/issue/YEP-5/set-up-development-environment
2. Read the full issue description
3. Check off completed setup tasks

#### Step 2: Work on It
```bash
# Create a branch
git checkout -b setup/yep-5-dev-environment

# Make any needed configuration changes
# Test your environment

# Commit your work
git add .
git commit -m "chore: Complete development environment setup [YEP-5]"
git push origin setup/yep-5-dev-environment
```

#### Step 3: Document in Notion
1. Create an experiment page in Notion
2. Document what you set up
3. Note any issues you encountered
4. Link back to YEP-5 in Linear

#### Step 4: Mark Complete
- Update YEP-5 status in Linear to "Done"
- Add link to your Notion documentation
- Move on to YEP-6!

### Your First Experiment (API Quickstart)

#### Step 1: Start YEP-6 in Linear
Visit: https://linear.app/yep-learn-ai/issue/YEP-6/complete-quick-start-guide

#### Step 2: Create Experiment Branch
```bash
git checkout -b experiment/yep-6-api-quickstart
```

#### Step 3: Code and Learn
```python
# Try the Anthropic API
import anthropic

client = anthropic.Anthropic()

message = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=1024,
    messages=[
        {"role": "user", "content": "Hello, Claude!"}
    ]
)

print(message.content)
```

#### Step 4: Commit Your Experiments
```bash
git add .
git commit -m "feat: Complete API quickstart experiments [YEP-6]"
git push origin experiment/yep-6-api-quickstart
```

#### Step 5: Document in Notion
- Create "API Quickstart Experiments" page
- Add your code snippets
- Document what you learned
- Note any interesting observations
- Link to GitHub commit and Linear issue

#### Step 6: Close Issue
- Mark YEP-6 as "Done" in Linear
- Add links to GitHub and Notion

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
├── docs/                 # Documentation
│   ├── WORKFLOW.md      # Daily workflow guide
│   └── SETUP.md         # Detailed setup instructions
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

## 🔧 Daily Workflow

See [WORKFLOW.md](docs/WORKFLOW.md) for detailed workflow documentation.

### Quick Reference
```bash
# Morning: Check what to work on
# Visit Linear: https://linear.app/yep-learn-ai

# Create branch for your issue
git checkout -b feature/yep-X-description

# Work, commit frequently
git add .
git commit -m "feat: Description [YEP-X]"

# Push and document
git push origin feature/yep-X-description
# Document in Notion
# Update Linear issue
```

### Commit Message Format
```
<type>: <description> [YEP-X]

Types: feat, fix, docs, test, refactor, chore
Always include [YEP-X] to link to Linear issue
```

## 🔗 System Links

### GitHub
- **Repository**: https://github.com/fordjes/AI-Learning-Lab
- **Issues**: Use Linear instead
- **Pull Requests**: Review and merge here

### Linear
- **Workspace**: https://linear.app/yep-learn-ai
- **Current Sprint**: Check active issues
- **Roadmap**: https://linear.app/yep-learn-ai/roadmap

### Notion
- **Workspace**: [Your Notion Workspace]
- **Experiments**: Document all your learnings
- **Journal**: Reflect on progress weekly

## 🎯 Learning Path

### Phase 1: LLM Foundations (Weeks 1-8)
- ✅ YEP-5: Development environment setup
- 🔄 YEP-6: Complete quick start guide
- ⏳ YEP-7: Complete Anthropic API quickstart
- ⏳ YEP-8: Build CLI chat application
- ⏳ YEP-9: Implement conversation memory
- ⏳ YEP-10: Week 4 checkpoint
- ⏳ YEP-11: Week 8 checkpoint (Phase 1 complete)

### Phase 2: RAG Systems (Weeks 9-16)
- ⏳ YEP-12: Week 12 checkpoint
- ⏳ YEP-13: Week 16 checkpoint (Phase 2 complete)

### Phase 3: Agentic AI (Weeks 17-24)
- ⏳ YEP-14: Week 20 checkpoint
- ⏳ YEP-15: Week 24 checkpoint (Program complete!)

## 🧪 Experiments

All experiments should be documented in Notion with:
- **Code snippets** from GitHub
- **Results and observations**
- **What worked / didn't work**
- **Next steps**
- **Links** to Linear issues and GitHub commits

Track code experiments using MLflow:

```python
import mlflow

with mlflow.start_run():
    mlflow.log_params({"learning_rate": 0.001})
    # Your training code
    mlflow.log_metrics({"accuracy": 0.95})
```

View experiments: `mlflow ui`

## 🔍 Troubleshooting

### Environment Issues

**Problem**: Python version too old
```bash
# Solution: Install Python 3.11+
# Visit: https://www.python.org/downloads/
```

**Problem**: Package installation fails
```bash
# Solution: Upgrade pip
pip install --upgrade pip
pip install -r requirements/base.txt
```

**Problem**: API key not working
```bash
# Solution: Check .env file
# Ensure ANTHROPIC_API_KEY is set correctly
# Restart your terminal
```

### Git Issues

**Problem**: Can't push to GitHub
```bash
# Solution: Check remote
git remote -v
# If needed, update remote URL
```

**Problem**: Merge conflicts
```bash
# Solution: Pull latest changes first
git checkout main
git pull
git checkout your-branch
git merge main
# Resolve conflicts manually
```

### Linear Integration

**Problem**: Commits not linking to issues
- **Solution**: Ensure commit message includes `[YEP-X]` format
- Example: `feat: Add feature [YEP-6]`

**Problem**: Can't find issues in Linear
- **Solution**: Check filters - make sure "All" is selected
- Visit: https://linear.app/yep-learn-ai/team/YEP/all

### Notion Documentation

**Problem**: Can't find experiment template
- **Solution**: Create a new page in Experiments database
- Include: Date, Title, Issue Link, GitHub Link, Code, Results, Insights

## 📚 Learning Resources

### Anthropic / Claude
- [Anthropic Documentation](https://docs.anthropic.com)
- [Prompt Engineering Guide](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)
- [API Reference](https://docs.anthropic.com/en/api/getting-started)

### RAG Systems
- [LangChain Documentation](https://python.langchain.com)
- [Vector Databases Guide](https://www.pinecone.io/learn/vector-database/)

### MLOps
- [MLflow Documentation](https://mlflow.org/docs/latest/index.html)
- [DVC Documentation](https://dvc.org/doc)

## 🤝 Contributing

This is a personal learning project, but feedback and suggestions are welcome!

1. Open an issue for bugs or feature requests
2. Follow the PR template for contributions
3. Ensure all tests pass before submitting
4. Document your changes in Notion

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ✅ Quick Verification Checklist

Before starting your learning journey, verify:

- [ ] Python 3.11+ installed
- [ ] Repository cloned
- [ ] Virtual environment activated
- [ ] Dependencies installed
- [ ] API keys configured in .env
- [ ] GitHub repository accessible
- [ ] Linear workspace accessible
- [ ] Notion workspace ready
- [ ] First issue (YEP-5) opened in Linear
- [ ] Workflow documentation read

**All set?** Start with YEP-5 in Linear! 🚀

---

**Status**: 🚧 Active Development | **Started**: November 2025 | **Duration**: 6 months

**Need Help?** Check [WORKFLOW.md](docs/WORKFLOW.md) or create an issue in Linear.
